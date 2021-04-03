# emsonline
Test project

# To compile angular and Spring project
$ myworkspace/emsonline 
mvn clean install

# run backend project which includes frontend/
cd backend/
mvn spring-boot:run

cd frontend/
ng build
ng serve -o

# Steps for testing -
A. start database and restful service 
    1. cd ../emsonline/
    2. docker-compose up -d employee-mysqldb
    3. docker-compose up -d emsonline-service
B. Build, run and test frontend application (hot deployment)
    1. cd ../emsonline/frontend/src/main/web/src/app
    2. ng serve --port=8080
C. opne browser and enter below URL
    http://localhost:8080/