# Tutorial Docker GetStartedLab

Prerequisite
- you have to create data directory to store visit counting and change mounting volume of Redis in docker-compose.yml
> $ mkdir ./data

- To change mounting volume of Redis in docker-compose.yml
> $ vi docker-compose.yml

- And then edit in volumes:
> volumes:
>      - /{running directory}/docker-tutorial-getstarted/data:/data


How to run this GetStartedLab

> $ docker stack deploy -c docker-compose.yml getstartedlab

Check stack is running

> $ docker stack ls

> $ docker stack ps getstartedlab
