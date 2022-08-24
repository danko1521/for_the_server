Команды для запуска сервера

docker build --tag=docker-django .

docker run -d -p 8000:8000 --name=dd docker-django