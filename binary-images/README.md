# Docker images including binary file

## make dummy binary

```bash
# 8MB x 32 = 256MB
dd if=/dev/urandom of=dummy_binary bs=8388608 count=32
```

## build image

```bash
sudo docker build -t foo/bar:tag -f Dockerfile.512m .
```
