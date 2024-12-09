# Рубежный контроль №2. Разработка Restful-сервиса на Golang

Рубежный контроль пишется очно на паре лобораторных работ.

В рамках данного РК необходимо разработать RESTful-сервис на Golang, реализующий некоторую бизнес-логику в рамках заданной предметной области

Принципиальное отличие от РК1 заключается в том, что задания будут в большей степени формулироваться в парадигме "Бизнес-требований", а не "Технического задания", соотвественно, необходимо будет самостоятельно спроектировать API и внутренние алгоритмы функционирования, опираясь на постановку и ответы заказчика на уточняющие вопросы (прям как на реальной айтишной работе).

## Шаблон

Шаблоном для написания РК является данный репозиторий. В качестве подготовки к РК желательно заблаговременно склонить данный репозиторий и проверить, что сервис корректно запускается, а клиентские запросы обрабатываются в соответствии с заданием в демонстрационном билете.

## Демонстрационный билет №1. Микросервис хранения пользователей

Реализовать микросервис на golang, реализующий логику хранения пользователей.

Должны поддерживаться следующие операции:
- создание нового пользователя
- получение списка пользователей
- получение пользователя по id пользователя
- обновление пользователя по id пользователя
- удаление пользователя по id пользователя

У пользователя при создании, как минимум, должно быть 2 поля: email и name. Поле email должно представлять собой валиднй адрес электронной почты, а поле name должно быть в пределах 3-30 символов. Оба поля должны быть уникальными.

Требования к пагинации при выводе списка пользователей не предъявляются

Сервис должен быть конфигурируемым с использованием конфиг файлов и/или флагов командной строки

Реализация хранилища в слое provider допускается как с использованием СУБД (рекомендуется), так и с использованием хранения непосредственно в оператинвной памяти приложения в виде глобальных переменных.

## Защита

Защита РК (как и написание) проходит очно на паре лабораторных работ. Во время защиты РК необходимо показать код на golang и продемонстрировать правильность обработки http-запросов c использованием какого-нибудь из клиентов из перечня: Postman, Insomnia, Curl

## Отчёт

Отчёт оформляется **ПОСЛЕ** защиты рубежного контроля и должен содержать:

1. Титульный лист
2. Задание
3. Решение

Получившийся отчёт наобходимо запушить в личный форк данного репозитория

## Примечание

Поскольку второй рубежный контроль проводится исключительно по Back-End составляющей, для успешного написания РК2 рекомендуется к 15-16 неделе семестра выполнить следующие лабораторные работы:
8. Golang & PostgreSQL
9. Golang & Echo
10. Golang & Clean Architecture

Требования к аутентификации ни в одном билете РК2 предъявляться не будут