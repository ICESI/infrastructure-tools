# Tools

- apt
- curl
- unzip
- awscli v2
- python3 and pip3
- python server + prometheus metrics endpoint

# Build, test and deploy commands

```
docker build -t d4n13lbc/all-tools-ubuntu:0.0.1 .
docker run -d -p 5000:5000 d4n13lbc/all-tools-ubuntu:0.0.1
curl localhost:5000/metrics
docker login
docker push d4n13lbc/all-tools-ubuntu:v0.0.1
```

# References
- https://github.com/jwilder/docker-squash