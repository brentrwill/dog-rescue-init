# Dog Rescue using Init
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

<br /><br />
Steps to import the project.<br /><br />

1- Download the zip file to your local computer and make sure the zip is for sure on your local computer.<br />
2- Extract the zip file into a location that you will remember.<br />
3- From Eclipse, choose the option to import a project, and select "Existing Projects into Workspace".<br />
4- Navigate to where you unzipped the file and it should show the src directory in your Select window.<br />
5- Once have it imported, you should have all the code imported into Eclipse.<br />
6- Once imported, you will want to create a user or re-use the same user from MySQL that you have setup.<br />
7- Edit the application.yaml file and change the username and password.<br />
8- Open DBeaver and create the petparks database.<br />
9- You can then startup the application and hit the controller to see if everything is working.<br />
<br /><br />
If you run into any issues, let me know and I will be happy to assist.
