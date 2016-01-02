# ilkka/httpd-ssl

Official Apache httpd image modified to have SSL turned on. Copy cert
and key into image or mount them as volumes:

```
$ docker run -d -e SERVER_NAME=foobar.example.com \
-v /path/to/server.crt:/usr/local/apache2/conf/server.crt \
-v /path/to/server.key:/usr/local/apache2/conf/server.key \
ilkka/httpd-ssl
```
