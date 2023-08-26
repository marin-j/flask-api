
## Save docker image as tar
```bash
sudo docker save --output flask-api:$IMAGE_VERSION.tar flask-api:$IMAGE_VERSION
```

## Import the image into k3s
```bash
sudo k3s ctr images i^Cort flask-api:latest.tar
```

## Image is now available on the cluster
