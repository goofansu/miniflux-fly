# miniflux-fly

[Miniflux](https://github.com/miniflux/v2) self-hosted on [Fly](https://fly.io).

## Install

### Configure the Fly app
Edit the `fly.toml` file and adjust the `app` and `BASE_URL` values to match your environment.

### Create login credential for Miniflux
```shell
fly secrets set ADMIN_USERNAME='<username>'
fly secrets set ADMIN_PASSWORD='<password>'
```

### Create database
```shell
fly postgres create
fly postgres attach <postgres-app>
```

### Deploy
```shell
fly deploy
```
