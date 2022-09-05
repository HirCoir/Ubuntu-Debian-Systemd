# Ubuntu-Debian-Systemd
Ubuntu/Debian funcionando con Systemd (service x start | restart | reload)

## Compilar
```sh
docker build -t ubuntu-systemd .
```

## Ejecutar
```sh
docker run -d --name systemd-ubuntu --tmpfs /tmp --tmpfs /run --tmpfs /run/lock -v /sys/fs/cgroup:/sys/fs/cgroup:ro ubuntu-systemd
```
