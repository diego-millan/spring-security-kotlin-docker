#Spring Security using DOCKER

##Docker
Application package:
mvn package

Docker package:
docker build -t application_name -f Dockerfile .
docker build -t forum -f Dockerfile .

Docker run:
docker run -p docker_port:application_port
docker run -p 3080:8080

For more info, check Dockerfile .

##Heroku
heroku login

Create dashboard

heroku create

cd workspace/project

heroku git:remote -a (app-named-by-heroku)

heroku container:login

heroku container:push web

heroku container:release web