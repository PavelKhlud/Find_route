# Проект Find Route

## Описание

Cайт Find Route, «Помощник в поиске пути». На этом сервисе зарегистрированные пользователи смогут находить маршруты и
сохранять их также редактивировать и добавлять города и маршруты. Незарегистрированные пользователи смогуть лишь
находить маршруты без возможности сохранения

Ознакомиться с уже развёрнутым проектом можно по адресу: <br/> 
[pkhludyw.beget.tech](http://pkhludyw.beget.tech).

Тестовый пользователь:
- login: test
- password: 12345

Возможности сервиса:

- Регистрация пользователей.
- Создание, Изменение, Удаление городов, маршрутов и поездов.
- Нахождение маршрутов по критериям: отправной город и город прибытия, промежуточные города и время в пути

- ### Установка

- Клонируйте репозиторий к себе на компьютер командой:

```
git clone https://github.com/DamageHunter/Find_route
```

Перейдите в каталог проекта:

```
cd Find_route
```

Создайте файл окружений

```
python3 -m venv env
```

Активируйте его:

```
source env/bin/activate
```

Загрузите все пакеты из requirements.txt:

```
pip3 install -r requirements.txt
```
Создайте миграции для бд:

```
python3 manage.py migrate
```

Загрузка начальные данные (фикстуру):

```
python3 manage.py loaddata initial_data.json
```

Запустите сервер
```
python3 manage.py runserver
```

После этого сайт будет доступен по адресу http://127.0.0.1:8000/
