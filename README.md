# Java DevOps jenkins

##  Technologies Used
- Java 17
- Maven
- Docker
- Jenkins

##  Build Steps

mvn clean package

##  Docker Build

docker build -t java-devops-app .

##  Jenkins Pipeline
This project uses Jenkins Pipeline as Code to automate:
- Code checkout
- Build
- Docker image creation
- Container deployment
