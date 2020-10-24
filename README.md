##  Architecture monolithique vs Microservice

## Heroku  CLI

```
* create new application on heroku
mvn  clean install -Dmaven.test.skip=true
cd target
heroku login
heroku heroku plugins:install java
heroku buildpacks:clear --app APP_NAME
heroku deploy:jar  my-app.jar --app APP_NAME
heroku logs --tail
```