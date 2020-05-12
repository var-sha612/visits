# Docker build
docker build .
docker build -t visits:latest .

# Docker cleanup
docker rm -vf $(docker ps -a -q)
docker rmi -f $(docker images -a -q)\n

# List container/images
docker images
docker container ls

# Run - wont work because there is not network
docker run redis
docker run visits

# Services - Different containers in Docker compose file

# Docker Compose commands
docker-compose
docker-compose up
docker-compose up --build
docker-compose ps
