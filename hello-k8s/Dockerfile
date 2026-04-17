# java 17을 실행할 수 있는 가벼운 런타입 환경
FROM eclipse-temurin:17-jdk-alpine

# Gradle로 빌드된 Spring Boot Jar 파일을 컨테이너 내부로 복사
COPY build/libs/*.jar app.jar

# 컨테이너가 구동될 때 이 JAR 파일을 실행하도록 명령을 내린다.
ENTRYPOINT ["java", "-jar", "/app.jar"]