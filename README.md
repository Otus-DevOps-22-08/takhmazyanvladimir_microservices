# takhmazyanvladimir_microservices
takhmazyanvladimir microservices repository

В рамках ДЗ docker-2 сделано следующее:
Приложение reddit завёрнуто в docker-образ
Данный образ запушен в Docker Hub
Проверено, что данный образ корректно скачивается, запускается, и приложение работает в локальном docker (curl 0.0.0.0:9292)

В рамках ДЗ docker-3 сделано следующее:
Приложение разбито на отдельные сервисы
Проверена корректность работы приложения
Подключён volume к контейнеру mondodb
Проверено, что посты сохраняются в контейнере после перезапуска

В рамках ДЗ docker-4 сделано следующее:
В сценарии docker-compose разделены сети для front и back
Параметризованы имя проекта, имя пользователя, порты, маски подсетей и тэги
Проверена работа параметризованного сценария
Ответ на вопрос: базовое имя проекта по умолчанию берётся из имени файла, параметризуется через ENV-переменную COMPOSE_PROJECT_NAME

В рамках ДЗ monitoring-1 сделано следующее:
Создан сценарий docker-compose для запуска приложения reddit, сбора метрик prometheus в т.ч. с использованием node exporter.
Образы микросервисов запушены в docker hub: 
https://hub.docker.com/r/takhmazyanvladimir/prometheus
https://hub.docker.com/r/takhmazyanvladimir/ui
https://hub.docker.com/r/takhmazyanvladimir/post
https://hub.docker.com/r/takhmazyanvladimir/comment

