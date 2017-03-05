Reference
https://angular.io/docs/ts/latest/guide/setup.html

Get git docker container if you don't have git locally
docker build -f Dockerfile_git -t kuldeeparyadotcom/git:snapshot .

Run a container to run Git
docker run --rm -it -v /Users/KD/quickstart:/data kuldeeparyadotcom/git:snapshot
