# Дипломная работа

## Документация:
[План автоматизации](https://github.com/plo-vi/aqaDiploma/blob/master/Plan.md)

[Отчет о тестировании](https://github.com/plo-vi/aqaDiploma/blob/master/Report.md)

[Отчет по итогам автоматизации](https://github.com/plo-vi/aqaDiploma/blob/master/Summary.md)

### Запуск тестов:
#### Работа с базой данных MySQl
1. 'docker-compose up -d' - *запуск контейнеров*
2. 'java -jar ./artifacts/aqa-shop.jar' - *запуск приложения*
3. 'gradlew clean test' - *запуск автотестов*
4. 'gradlew allureReport', 'gradlew allureServe' - *создание отчета Allure*

#### Работа с базой данных PostgreSQL
1. 'docker-compose up -d' - *запуск контейнеров*
2. 'java -jar ./artifacts/aqa-shop.jar --spring.datasource.url=jdbc:postgresql://localhost:5432/app' - *запуск приложения*
3. 'gradlew clean test -Ddb.url=jdbc:postgresql://localhost:5432/app'- *запуск автотестов*
4. 'gradlew allureReport', 'gradlew allureServe' - *создание отчета Allure*
