# Sentry on premise docker

This project is a shortcut to prepare a minimal Sentry on premise environment. It will prepare a Sentry server and its dependencies to execute locally.

## Dependencies
- Docker
- Docker composer

## Run
### First execution
```
docker-compose up -d postgres
docker-compose up -d redis 
docker-compose run sentry sentry upgrade
```

When the user prompt is displayed, fill with user (email) and password. This will be the root credentials.

### Next executions
```
docker-compose up -d
```
