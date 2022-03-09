task_1
docker build . -t de_frontend
docker run -p 8080:3000 -d -it --name de_frontend de_frontend