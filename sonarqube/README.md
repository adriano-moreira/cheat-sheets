# how-to-use-sonarqube-with-docker


``` sh
docker network create sonar
```

create sonar database container
``` sh
docker run -d --name sonarqube-db \
    --network=sonar \
    -e POSTGRES_USER=sonar \
    -e POSTGRES_PASSWORD=sonar \
    -e POSTGRES_DB=sonar \
    postgres:9.6-alpine
```

``` sh
docker run -d --name sonarqube \
    --network=sonar \
    -p 9000:9000 -p 9092:9092 \
    -e SONARQUBE_JDBC_USERNAME=sonar \
    -e SONARQUBE_JDBC_PASSWORD=sonar \
    -e SONARQUBE_JDBC_URL=jdbc:postgresql://sonarqube-db/sonar \
    sonarqube:alpine
```

the scan
``` sh
docker run \
  --rm \
  --network=sonar \
  -ti -v $(pwd):/root/src  \
  newtmitch/sonar-scanner  sonar-scanner \
  -Dsonar.host.url=http://sonarqube:9000 \
  -Dsonar.projectKey=MyProjectId \
  -Dsonar.projectName="My Project" \
  -Dsonar.projectVersion=1 \
  -Dsonar.projectBaseDir=/root \
  -Dsonar.sources=./src
```

