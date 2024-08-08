### Проект KITTY_SERVICE

KITTY_SERVICE - это веб-приложение для обмена фотографиями домашних питомцев. Пользователи могут добавлять данные о своих котах, такие как фотографии, имя, цвет и год рождения, а также просматривать профили котов других пользователей.

Ознакомиться с KITTY_SERVICE можно тут: https://foodgraming.ddnsking.com
### Статус CI/CD:

[![CI/CD Status](https://github.com/bignikkk/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/bignikkk/kittygram_final/actions/workflows/main.yml)


### Автор:
Автор: Nikita Blokhin
GitHub: github.com/bignikkk

### Технологии:

Python
PostgreSQL
Django REST Framework
Docker Hub
GitHub Actions

### Как заполнить файл .env:

Укажите следующие переменные среды в файле .env:

   - POSTGRES_DB: название базы данных PostgreSQL для проекта Kitty_service.
   - POSTGRES_USER: имя пользователя базы данных PostgreSQL.
   - POSTGRES_PASSWORD: пароль пользователя базы данных PostgreSQL.
   - DB_HOST: хост базы данных PostgreSQL.
   - DB_PORT: порт базы данных PostgreSQL (обычно 5432).

Присвойте каждой переменной необходимое значение, учитывая настройки вашей среды и конфигурации вашего сервера.Сохраните файл .env.

Клонировать репозиторий и перейти в него в командной строке:

### Как развернуть проект локально:

```
git clone https://github.com/bignikkk/kitty_service
```

```
cd backend
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
