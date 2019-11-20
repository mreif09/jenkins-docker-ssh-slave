# Jenkins Docker in Docker SSH slave

A Jenkins SSH slave for running containers on the docker daemon of its host.

## Run

```bash
docker run -d -v /var/run/docker.sock:/var/run/docker.sock jenkins-docker-ssh-slave "<public key>"
```

The slave is reachable as SSH agent with username "jenkins" and the private key for the given public key.
