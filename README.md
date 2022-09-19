Установка проекта с помощью docker-compose
Склонировать репозиторий с Github

git clone git@github.com:pavel-nesterchuk/Mailing-list-management-service.git

    Перейти в директорию проекта
    В файле .evn заполнить необходимые данные: TOKEN = '<your token>'
    Запустить контейнеры

sudo docker-compose up -d

    Остановка работы контейнеров

sudo docker-compose stop


http://0.0.0.0:8000/api/ - api проекта

http://0.0.0.0:8000/api/clients/ - клиенты

http://0.0.0.0:8000/api/mailings/ - рассылки

http://0.0.0.0:8000/api/mailings/fullinfo/ - общая статистика по всем рассылкам

http://0.0.0.0:8000/api/mailings/<pk>/info/ - детальная статистика по конкретной рассылке

http://0.0.0.0:8000/api/messages/ - сообщения

http://0.0.0.0:8000/docs/ - docs проекта

http://0.0.0.0:5555 - celery flower
