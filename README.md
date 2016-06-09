# phpstorm-on-docker
run phpstorm inside a docker container sharing X11 socket

# Create docker container
```bash
$ docker build -t gerardorf/phpstorm .
```

# Start containter
```bash
$ docker-compose up
```

# Troubleshooting
- cant open display
```bash
$ xhost +
```
- uid problems
  - modify Dockerfile setting current user uid and gid.
  - how to get uid and gid
```bash
$ id -u
$ id -g
```
