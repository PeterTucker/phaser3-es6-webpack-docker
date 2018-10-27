# Phaser 3 + Babel ES6 + Webpack + Docker
This project lets you quickly get up and running to develop Phaser3 projects with webpack in a docker container.

## How to run
- 1. cd into node folder.
- 2. Remove, rebuild, and run container/image with docker compose:
docker-compose -f docker-compose.yml rm -f && docker-compose -f docker-compose.yml build --no-cache &&  docker-compose -f docker-compose.yml up 
- 3. If need be, jump into container w/ bash:
docker exec -i -t phaser3-es6-webpack-docker_phaser-proj-node-server_1 bash

## Change from development mode to build mode
In the docker-compose.yml file, simply change 
command: npm run start
to
command: npm run build
then run command "docker-compose build" then "docker-compose up"

## Project based on
https://github.com/tsuriyathep/phaser3-es6-webpack