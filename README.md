# opencadc-cadctap

Docker builds that support Python versions:
- 3.14

## Build
```sh
cd docker/3.14
docker build --no-cache --tag at88mph/opencadc-cadctap:3.14-slim .
```

Or setup relevant platforms:
```sh
docker build --no-cache --tag at88mph/opencadc-cadctap:3.14-slim --platform linux/amd64,linux/arm64 .
```
