# Supported tags

- [`2.4`, `2`, `latest` (*Dockerfile*)](https://github.com/ilkka/docker-httpd-ssl/blob/master/Dockerfile)

# What is this?

Official Apache httpd image modified to have SSL turned on. Copy cert
and key into image or mount them as volumes.

# How to use this image

```
$ docker run -d -e SERVER_NAME=foobar.example.com \
-v /path/to/server.crt:/usr/local/apache2/conf/server.crt \
-v /path/to/server.key:/usr/local/apache2/conf/server.key \
ilkka/httpd-ssl
```
