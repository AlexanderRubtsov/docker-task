FROM bellsoft/liberica-openjdk-alpine:11
# Делаем сперва gradlew build, потом копируем из папки и переименовываем в service.jar
COPY build/libs/admin-server-0.0.1-SNAPSHOT.jar admin-service.jar
# Начальная команда при запуске контейнера
ENTRYPOINT ["java", "-jar", "/admin-service.jar"]
# CMD - похожа на ENTRYPOINT, но указывает на дефолт аргументы для той утилиты,
# что мы использовали в ENTRYPOINT
# маркер порта, в котором указываем, что данный порт можно пробросить.
EXPOSE 9003