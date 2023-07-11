# Delivery.Deploy
1. Склонировать репозиторий Delivery.Deploy
2. Убедиться, что на компьютере установлены docker, docker-compose (для запуска докер-контейнеров через docker-compose.yaml) и minikube (для запуска докер контейнеров через Kubernetes)
3. Запустить докер контейнеры через команду из склонированного репозитория:
```
sudo docker-compose up
```
4. Запустить локальный сервер Kubernetes:
```
minikube start
```
5. Перейти в KubernetesConfigs, применить конфигурационные файлы Kubernetes для создания всех сервисов, подов:
```
minikube kubectl -- apply -f .
```