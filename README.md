<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

---
# Тестовый проект на Laravel + PostgreSQL + Vue

## Запуск проекта
Открываем командную строку и вводим команду
```
./vendor/bin/sail up
```
Можно настроить псевдоним, чтобы сделать команду короче
```
alias sail='bash vendor/bin/sail'
```
После этой команды будет достаточно ввода такой команды для старта проекта
```
sail up
```
Этой командой запускаем контейнеры в фоновом режиме
```
sail up -d
```
Остановить можно любой из двух команд
```
sail down
sail stop
```
При запуске artisan, composer и npm команд sail должен предшествовать командам

Вместо
```
php artisan migrate
```
Пишем
```
sail artisan migrate
```
Вместо
```
composer require laravel/sanctum
```
Пишем
```
sail composer require laravel/sanctum
```
