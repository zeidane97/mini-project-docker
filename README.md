    cloner le repertoire
    se positioner dans mini-project-docker/simple_api
     - builder l'image 
        docker build -t simple-api:1 .
        docker run -it -d -p5000:5000 --name=simple-api simple-api:1  
    retourner dans le repo mini-project-docker
        docker-compose up -d
    accedez à l'appli via le port 8080
