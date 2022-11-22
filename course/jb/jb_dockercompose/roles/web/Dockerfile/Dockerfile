FROM yanivomc/alpine-oraclejdk8:slim
WORKDIR /app
COPY /code/spring-music.jar .
EXPOSE 8080
CMD ["java","-jar","-Dspring.profiles.active=none","spring-music.jar"]
