# lft-jenkins-demo  

## How To Use

### Create Docker Volume
```shell
docker volume create lft-jenkins-demo-volume
```

### Build the Dockerfile
```shell
docker build --no-cache -t lft-jenkins-demo:latest .
```

### Run the Docker Image created from above Dockerfile
```shell
docker run -d -p 8080:8080 -p 50000:50000 -v lft-jenkins-demo-volume:/var/jenkins_home lft-jenkins-demo:latest
```

## References
- [Jenkins Base Image](https://hub.docker.com/r/jenkins/jenkins)
- [Official Jenkins Docker image docs](https://github.com/jenkinsci/docker/blob/master/README.md)
- [Set up and use local docker volume](https://rangle.io/blog/running-jenkins-and-persisting-state-locally-using-docker-2/)