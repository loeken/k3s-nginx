# k3s-nginx

## Description

this is an example to create a docker container with nginx to host static websites

```bash
docker build -t test .
```

```bash
docker run -p 80:80 test
```

### Login to Google Container Registry

```bash
gcloud auth login
gcloud config set project internetzme
```

```bash
docker tag test gcr.io/internetzme/test:1.0.0
docker push gcr.io/internetzme/test:1.0.0
```