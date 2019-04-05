# Extended to include serving over https
Minimal Node.js application for intro to Docker tutorial: https://www.digitalocean.com/community/tutorials/how-to-build-a-node-js-application-with-docker

### Generate SSL certificates
```sh 
$ cd nginx-certs
```
```sh
$ openssl req -config csr.conf -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx.key -out nginx.crt
```

### Start the application

```sh
$ docker-compose up -d 
```

[Visit site ](https://localhost)