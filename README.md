Angular 2 Quickstart seed project

Reference
https://angular.io/docs/ts/latest/guide/setup.html

#Git
Get git docker container if you don't have git locally
docker build -f Dockerfile_git -t kuldeeparyadotcom/git:snapshot .

Run a container to run Git (Mind volume that you're mounting)
docker run --rm -it -v /Users/KD/quickstart:/data kuldeeparyadotcom/git:snapshot

#Node
Image Creation
docker build -f Dockerfile_node -t kuldeeparyadotcom/node:snapshot .

Run a container to run node (Mind volume that you're mounting)
docker run -it --name quickstart_node -p 3000:3000 -p 3001:3001  -v /Users/KD/quickstart/quickstart:/data kuldeeparyadotcom/node:snapshot

Get in to quickstart_node container to execute node commands
docker exec -it quickstart_node /bin/bash
