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
# Conection PostgresSQL

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
