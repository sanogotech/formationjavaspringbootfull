##  Architecture monolithique vs Microservice

## Heroku  CLI

```
* create new application on heroku
mvn  clean install -Dmaven.test.skip=true
git push heroku master
cd target
heroku login
heroku plugins:install java
heroku buildpacks:clear --app APP_NAME
heroku run java -version --app  APP_NAME
heroku deploy:jar  my-app.jar --app APP_NAME
heroku logs --tail
```

##  Web

** application.properties
** replace  server.port=8080  with :
server.port=${PORT:8080}

- http://javaformation.herokuapp.com/

