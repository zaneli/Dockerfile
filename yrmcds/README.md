# [yrmcds](https://github.com/cybozu/yrmcds)

## Getting Started

```
> docker pull zaneli/yrmcds

> docker run -d -p 11211:11211 zaneli/yrmcds
```

## Access From Host Machine

### on boot2docker

```
> telnet $(boot2docker ip) 11211
```

### on CoreOS

```
> telnet <CoreOS's IPAddress> 11211
```
