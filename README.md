# Laboratory One of ARSW

Make a practice for create a project MAVEN and use of gitHub

## Getting Started

For clone this repository you use this command:
 ```
 git clone https://github.com/JffMv/Lab_1_ARSW
 ```

### Prerequisites

Have installed:
maven 3.9.6
[Install Maven](https://maven.apache.org/download.cgi#Installation)


git 2.44 
[Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

java
[Install Java](https://www.oracle.com/co/java/technologies/downloads/)


## Running the tests

For Run Test you need the command:
```
 mvn test
```

## Deployment

The process were building project maven whit the command:

```
mvn archetype:generate -DgroupId=edu.escuelaing.arsw.ASE.app -DartifactId=miprimera-app -DarchetypeArtifactId=maven-archetype-quickstart -
DinteractiveMode=false

```

Then we have verify the class App.java and the pom.xml, run the project with: 

```
mvn package
```
Run the class seen console with:


```
java -cp target/mi-primera-app-1.0-SNAPSHOT.jar
edu.escuelaing.arsw.ASE.app.App
```
and result print "Hello Workd!"

For generate documentation update the pom.xml add and later use "mvn package":


```
<reporting>
    <plugins>
    <plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-javadoc-plugin</artifactId>
    <version>2.10.1</version>
    <configuration>
    </configuration>
    </plugin>
    </plugins>
</reporting>
```

and the use in order this commands for run documentation:

```
mvn javadoc:javadoc
mvn javadoc:jar
mvn javadoc:aggregate
mvn javadoc:aggregate-jar
mvn javadoc:test-javadoc
mvn javadoc:test-jar
mvn javadoc:test-aggregate
mvn javadoc:test-aggregate-jar
```

if you want see this documentation go to file located


```
...\target\apidocs\index.html

```



## Built With

* [Java](https://www.java.com/es/) - The language used
* [Maven](https://maven.apache.org/) - Dependency Management



## Authors

* **Yeferson Mesa**

## License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details

