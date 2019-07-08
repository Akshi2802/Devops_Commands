# Devops_Notes
ls
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
docker rmi $(docker images -q) --force
docker info
docker build -t devopsdemo/javaapp-demo:${BUILD_NUMBER} .
docker tag devopsdemo/javaapp-demo:${BUILD_NUMBER} devopsdemo/javaapp-demo:latest
docker images
docker run -it -p 8081:8080 devopsdemo
