# Tutorial Docker GetStartedLab

Prerequisite
- you have to create data directory to store visit counting and change mounting volume of Redis in docker-compose.yml
``` bash
$ mkdir ./data
```

- And then change mounting volume of Redis in docker-compose.yml
> volumes:
>      - /{running directory}/docker-tutorial-getstarted/data:/data


How to run this GetStartedLab
``` bash
$ docker stack deploy -c docker-compose.yml getstartedlab
```

Check stack is running
``` bash
$ docker stack ls
$ docker stack ps getstartedlab
```
