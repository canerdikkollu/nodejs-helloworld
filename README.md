# nodejs-helloworld

Build image
```sh
docker build . -t canerdikkollu/nodejs-helloworld  
```

Run container
```sh
docker run -p 49160:8080 -d canerdikkollu/nodejs-helloworld
```

Test
```sh
curl -i localhost:49160
```


Ref: https://nodejs.org/en/docs/guides/nodejs-docker-webapp/