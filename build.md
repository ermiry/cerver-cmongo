# Build Cerver-CMongo Docker Images

## Development

Build development image

```
sudo docker build --build-arg CERVER_VERSION=$(cat cerver.txt) -t ermiry/cerver-cmongo:development -f Dockerfile.dev .
```

## Buildev

Build development builder image

```
sudo docker build --build-arg CERVER_VERSION=$(cat cerver.txt) -t ermiry/cerver-cmongo:buildev -f Dockerfile.buildev .
```

## Builder

Build builder image

```
sudo docker build --build-arg CERVER_VERSION=$(cat cerver.txt) -t ermiry/cerver-cmongo:builder -f Dockerfile.builder .
```

## Production

Build production image

```
sudo docker build --build-arg CERVER_VERSION=$(cat cerver.txt) -t ermiry/cerver-cmongo:latest -f Dockerfile .
```