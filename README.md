## Server Config configuration

NOTE: yml/properties file name for the configuration should match the name of spring service, which is specified in
bootstrap.yml file

### Config Server 

Example of yml/properties files on GitHub:

```
heroku-scheduler-app.yml
```

### Client Server

Example of Client Server configuration:

```
spring:
  application:
    name: heroku-scheduler-app 
  cloud: 
    config:
      uri: ${CONFIG_SERVER_URI:http://127.0.0.1:8888}
```