# Run the following commands to initialize the project
docker-compose down &&
sudo chmod o+w ./src/personal-project/storage/ -R &&
docker-compose up -d &&
docker exec -it apache sh -c "npm install && composer install"