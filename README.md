# Spring Boot Demo Project

Это небольшой демонстрационный проект на Spring Boot.  
В проекте реализована регистрация, авторизация с JWT, защита эндпоинтов и работа с базой H2.

## Что умеет проект
- Регистрация пользователей (/register)
- Логин с выдачей JWT токена (/login)
- Защита эндпоинтов (например, /users)
- Подключение к встроенной базе H2 (удобно тестировать)

## Как запустить
1. Скачайте проект или клонируйте:
git clone https://github.com/EmaJhinVirtuoso/springboot-demo.git

2. Перейдите в папку проекта:
cd springboot-demo

3.Запустите:
./mvnw spring-boot:run
или если установлен Maven:
mvn spring-boot:run

4. Откройте в браузере:
http://localhost:8080/
Для H2 Console:
http://localhost:8080/h2-console

(логин: `sa`, пароль пустой)

## Полезные эндпоинты

- POST `/register` → регистрация
- POST `/login` → авторизация, получение JWT
- GET `/users` → список пользователей (нужен JWT)
