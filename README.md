# Taski
Приложение для планирования своих задач.

# Собрать и запустить контейнер
docker-compose up --build -d

# Запуск миграции базы данных
docker-compose exec web python manage.py migrate

# Открыть
http://localhost:8000