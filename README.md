# Banking Operations Service

## Реализовано

- **Управление пользователями:**
    - Создание новых пользователей с уникальными логином, email и номером телефона.
    - Обновление и удаление номера телефона и email (при наличии хотя бы одного из них).

- **Управление счетами:**
    - Создание банковского аккаунта с начальным балансом.
    - Обновление баланса с учетом процентной ставки (5% каждую минуту, до максимума в 207% от начального депозита).
    - Защита от отрицательного баланса.

- **Перевод денег:**
    - Перевод средств между счетами пользователей.
    - Проверка на достаточность средств и потокобезопасность.

- **Поиск пользователей:**
    - Поиск с фильтрацией по дате рождения, телефону, email и ФИО.
    - Пагинация и сортировка результатов поиска.

- **Аутентификация:**
    - JWT-аутентификация для защиты API (за исключением создания новых пользователей).

- **Документация API:**
    - OpenAPI/Swagger для удобного взаимодействия и тестирования API.

- **Логирование:**
    - Подробное логирование операций для аудита и отладки.

## Тестирование

- Тесты для проверки функциональности перевода денег между счетами.

## Технологический стек

- Java 17
- Spring Boot 3
- PostgreSQL
- Maven
- REST API
- JWT для аутентификации

---

Этот проект предоставляет функционал для управления банковскими счетами, переводов средств и начисления процентов, а также включает в себя поиск пользователей и защищен JWT-аутентификацией.
