# lft-jenkins-demo  

## How To Use

### Build the Dockerfile
```shell
docker build -t lft-jenkins-demo:latest .
```

### Run the Docker Image created from above Dockerfile
```shell
docker run -p 8080:8080 -p 50000:50000 lft-jenkins-demo:latest
```