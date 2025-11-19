FROM ubuntu AS builder
RUN apt-get update && apt-get install -y maven openjdk-17-jdk
COPY . /
RUN mvn package

FROM ubuntu
COPY --from=builder /target/words.jar /words.jar
CMD ["java", "-jar", "/words.jar"]
