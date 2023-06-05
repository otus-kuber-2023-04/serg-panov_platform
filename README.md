# serg-panov_platform
serg-panov Platform repository
# Выполнено ДЗ №1
- Настроена среда разработки на базе minikube и kind, настроена утилита kubectl
- Создан Dockerfile на базе nginx с рабочей директорией /app, запускаемый на порту 8000 под пользователем UID 1001
- Из Dockerfile собран образ контейнера, который опубликован https://hub.docker.com/repository/docker/spanov1980/otus-hw-02-nginx
- Создан манифест web-pod.yaml c init контейнером и общим томом
- Из Dockerfile собран образ контейнера, для микросервиса frontent приложения Hipster Shop, который опубликован https://hub.docker.com/repository/docker/spanov1980/microservices-demo-frontend
- Создан манифест frontend-pod.yaml из команды 'kubectl run frontend --image spanov1980/microservices-demo-frontend --restart=Never --dry-run -o yaml'
- В манифест frontend-pod.yaml добавлены параметры переменного окружения, позволяющие запустить Pod
