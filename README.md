This is an example of how to use the JPA framework, but loading the files from the resource directly.

An example of this is:

spring:
  datasource:
    username: *********
    password: *********
    url: jdbc:mysql://localhost:3306/dog_rescue
    
  jpa:
    hibernate:
      ddl-auto: none // This means the entity scanning will not work.
    show-sql: true
    defer-datasource-initialization: true
    
  sql:
    init:
      mode: always // This means it will always read the sql files in the resource directory.
