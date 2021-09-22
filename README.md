# cheatsheets

## docker

1. list all containers
    ```docker container ls -a```
1. remove all exited containers
    ```docker rm -v $(docker ps -a -q -f status=exited)```
    
### docker-compose
1. stop all container defined by a docker-compose.yml
    ```docker-compose -f "[filename]" down```
1. build & start all container defined by a docker-compose.yml
    ```docker-compose -f "[filename]" up -d --build```
    > -d : run containers in the background
    > --build : not yet existing image are builds
