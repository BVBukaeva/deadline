# deadline
## Тестирование входа в интернет банк
### Начало работы
1. Скачайте проект по ссылке: https://github.com/BVBukaeva/deadline.git
2. Установить java 11
3. Скачайте Docker Desktop
### Запуск
1. Запускаем docker контейнер с базой данных MySQL. docker-compose up
2. Запускаем SUT. java -jar artifacts/app-deadline.jar -P:jdbc.url=jdbc:mysql://localhost/mysql -P:jdbc.user=root -P:jdbc.password=qwerty123 .
3. Запускаем автотесты. gradlew clean test.
Должно выводится такое сообщение: BUILD SUCCESSFUL.
