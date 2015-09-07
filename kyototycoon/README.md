# [Kyoto Tycoon](http://fallabs.com/kyototycoon/)

## Getting Started

```
> docker pull zaneli/kyototycoon

> docker run -d -p 1978:1978 zaneli/kyototycoon
```

## Access From Host Machine

### on boot2docker

```
> curl http://$(boot2docker ip):1978/rpc/echo?ping=pong
```

### on CoreOS

```
> curl http://<CoreOS's IPAddress>:1978/rpc/echo?ping=pong
```
