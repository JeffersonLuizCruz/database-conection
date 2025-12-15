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
```
----------------------------------------------------------------------------------------

# Conection PostgresSQL
```
server.port=8080

spring.datasource.driver-class-name=org.postgresql.Driver
spring.datasource.url=jdbc:postgresql://localhost:5432/dio
spring.datasource.username=postgres
spring.datasource.password=root

spring.jpa.hibernate.ddl-auto=validate
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```
-----------------------------------------------------------------------------------------
# Conection MySql

```
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=jdbc:mysql://localhost:3306/nome_banco_de_dados
spring.datasource.username=admin
spring.datasource.password=admin
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```
V2_Conection MySql
```
spring.jpa.hibernate.ddl-auto=update
spring.datasource.url=jdbc:mysql://${MYSQL_HOST:localhost}:3306/nome_banco_de_dados
spring.datasource.username=admin
spring.datasource.password=123
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.show-sql=true
```
Docker-Compose.yml
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
      - MYSQL_PASSWORD=123
      - MYSQL_DATABASE=nome_banco_de_dados
      - MYSQL_ROOT_PASSWORD=123
    volumes:
      - db_data:/var/lib/mysql

volumes:
  db_data:
```

