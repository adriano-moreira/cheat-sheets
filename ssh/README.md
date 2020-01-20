# ssh

prefer ed25519

```bash
ssh-keygen -o -a 100 -t ed25519
```


to start ssh-agent
```bash
eval `ssh-agent -s`
```


---
~/.ssh/config file


add alias host
```
Host [aliasHost]
    HostName [realHost]
    User [user]
    IdentityFile [key.pem]
```
