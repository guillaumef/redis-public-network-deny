# redis-public-network-deny
Patch against redis to deny public networks - allow only private.
Connection is closed after 'accept'.


Move in redis sources directory:
```shell
  cd redis-XXX
```

Apply patch:
```shell
  curl -s https://raw.githubusercontent.com/guillaumef/redis-public-network-deny/main/redis-accept-ip.patch | \
    patch -p1
```
