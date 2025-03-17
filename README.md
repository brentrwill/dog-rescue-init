This is an example of how to use the JPA framework, but loading the files from the resource directly.
<br/>

An example of this is:
</br>
spring:<br/>
  datasource:<br/>
    username: *********<br/>
    password: *********<br/>
    url: jdbc:mysql://localhost:3306/dog_rescue<br/>
    <br/>
  jpa:<br/>
    hibernate:<br/>
      ddl-auto: none // This means the entity scanning will not work.<br/>
    show-sql: true<br/>
    defer-datasource-initialization: true<br/>
    <br/>
  sql:<br/>
    init:<br/>
      mode: always // This means it will always read the sql files in the resource directory.<br/>
