This is an example of how to use the JPA framework, but loading the files from the resource directly.
<br/>

An example of this is:
</br>
spring:<br/>
  &ensp;datasource:<br/>
    &ensp;&ensp;username: *********<br/>
    &ensp;&ensp;password: *********<br/>
    &ensp;&ensp;url: jdbc:mysql://localhost:3306/dog_rescue<br/>
    <br/>
  &ensp;jpa:<br/>
    &ensp;&ensp;hibernate:<br/>
      &ensp;&ensp;&ensp;ddl-auto: none // This means the entity scanning will not work.<br/>
    &ensp;&ensp;show-sql: true<br/>
    &ensp;&ensp;defer-datasource-initialization: true<br/>
    <br/>
  &ensp;sql:<br/>
    &ensp;&ensp;init:<br/>
      &ensp;&ensp;&ensp;mode: always // This means it will always read the sql files in the resource directory.<br/>
