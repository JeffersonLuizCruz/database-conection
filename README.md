# Conection SQL Server
```
spring.datasource.url=jdbc:sqlserver://localhost:1433;databaseName=spring_security
spring.datasource.username=sa
spring.datasource.password=Brasil@123
spring.datasource.driverClassName=com.microsoft.sqlserver.jdbc.SQLServerDriver
server.port=8090

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true

--------------------------------------------------------------------------------------------
spring.application.name=
spring.jpa.hibernate.ddl-auto=update
spring.datasource.url=jdbc:mysql://${MYSQL_HOST:localhost}:3306/nome_base_de_dados
spring.datasource.username=admin
spring.datasource.password=123
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.show-sql=true

```
```
docker-compose.yml:

services:
  mysql:
    image: mysql
    ports:
      - "3306:3306"
    expose:
      - "3306"
    environment:
      - MYSQL_USER=admin
      - MYSQL_PASSWORD=admin
      - MYSQL_DATABASE=nome_base_de_dados
      - MYSQL_ROOT_PASSWORD=admin
    volumes:
      - db_data:/var/lib/mysql

volumes:
  db_data:

 Conection PostgresSQL

```
server.error.include-stacktrace=never
server.port=8080

spring.datasource.driver-class-name=org.postgresql.Driver
spring.datasource.url=jdbc:postgresql://localhost:5432/dio
spring.datasource.username=postgres
spring.datasource.password=root

spring.jpa.hibernate.ddl-auto=validate
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```

# Conection MySql
```
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=jdbc:mysql://localhost:3306/api
spring.datasource.username=root
spring.datasource.password=root

spring.jpa.hibernate.ddl-auto=validate
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```
