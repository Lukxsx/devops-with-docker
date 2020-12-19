FROM openjdk:11-buster
EXPOSE 8080
RUN apt-get -y install git
RUN git clone https://github.com/docker-hy/spring-example-project.git
WORKDIR /spring-example-project 
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar
