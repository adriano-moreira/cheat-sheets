Quarkus provides mechanism to migrate code to next version

with QuarkusCLI:
```
quarkus update --stream=3.0
```

with Maven:
```
mvn io.quarkus.platform:quarkus-maven-plugin:3.0.1.Final:update -N -Dstream=3.0
```

with Gradle:
```
gradle -PquarkusPluginVersion=3.0.1.Final quarkusUpdate --stream=3.0
```
