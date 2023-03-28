
## Howto Run

- Download and install intellij IDE here: https://www.jetbrains.com/idea/
- Clone this git repo 
  ```
  >> git clone git@github.com:epocolis/graphdb_example.git
  ```
  
- Open the project using Intellij 
- You will also have to install maven see: https://maven.apache.org/install.html

All GraphDB programming examples are provided as a Maven project.

Since GraphDB is not available from Maven Central (the public Maven repository),
you have to install the GraphDB runtime jar into your local Maven repository.

To do that, go to the examples/maven-installer subdirectory of the distribution and run:

  mvn install

Note that the Maven executable, mvn, must be in your path.

This will cause and error, you can find the missing libray here https://maven.apache.org/install.html. 
You will need to search for it. Download the jar file and copy it to the location specified in the error. 

In order to run the example, change the *myrepo* to point to a repo in that exists in your local graphdb instance. 
```
>> HTTPRepository repository = new HTTPRepository("http://localhost:7200/repositories/myrepo");
```

You can now right click on the **FamilyRelationsApp.java** and click the "run". 

Good Luck :-)
