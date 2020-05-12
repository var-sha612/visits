# Docker build
docker build .
docker build -t visits:latest .

# Docker cleanup
docker rm -vf $(docker ps -a -q)
docker rmi -f $(docker images -a -q)\n

# List container/images
docker images
docker container ls

# Docker run
docker run redis
docker run visits

# Docker Compose commands
docker-compose
docker-compose up
docker-compose up --build
docker-compose ps
