# Docker version
- docker v.19.03.12
- docker-compose v.1.27.2

# How to start
`docker-compose up -d`

If you go to `localhost:8080/` you will see the index page with phpinfo.

# Ports
- NGINX: 8080
- app: 9000

# App
- PHP v. 7.4.10-fpm
- Dockerfile is located at `/app/Dockerfile`

# Xdebug
- v.2.9.8
- config file is located at `app/xdebug.ini`
- remote log file is located at `/tmp/xdebug/xdebug_remote.log`
- remote host is `172.17.0.1` (check this with `ifconfig docker0` -> 'inet' field)
- profiler dir is located at `/tmp/xdebug/`

# Webserver
- v. nginx:latest
- root folder is `/var/www/public`
- config file is located at `web/app.conf`
