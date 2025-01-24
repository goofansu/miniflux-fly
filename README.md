# miniflux-fly

[Miniflux](https://github.com/miniflux/v2) self-hosted on [Fly](https://fly.io).

## Deploy

### Set Miniflux's username and password
```shell
fly secrets set ADMIN_USERNAME='<username>'
fly secrets set ADMIN_PASSWORD='<password>'
```

### Create PostgreSQL
```shell
fly postgres create
fly postgres attach <postgres-app>
```

### Deploy
```shell
fly deploy
```
