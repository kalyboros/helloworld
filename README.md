# CT360 Maven assignment

Second week, maven task

## Task explanation

1. Create a Java - Maven Project :heavy_check_mark:
2. Add some dependencies (check pom.xml) :heavy_check_mark:
    * added commons-io
    * added mail api
3. Add two child projects (check pom.xml) :heavy_check_mark:
   * child1
   * child2
4. Add dependencies to them(check their pom.xml) :heavy_check_mark:
    * child1 has gson lib
    * child2 has joda time
5. Specify version :heavy_check_mark:
    * in child2 i changed the version of that particular dependency from latest stable to previous rolling in 2021

6. Specify some plugins :heavy_check_mark:
   * Added plugins for build

7. Build project :heavy_check_mark:


## Answers to questions
1. m2 
   * what is? A local repository of dependencies, libraries and projects
   * Where it is? Usually can be found in C:\Users\USERNAME\.m2
   * What is it for? More or less for local storing of dependencies, libs and projects, specifically their builds, packaging, etc.
   
2. Settings xml
   * How does it know where to get jars from?
   * We can specify everything ourselves in the settings, but the protocol works as following:
      1. We add a dependency to pom.xml
      2. It either takes it locally from .m2/repositories or downloads it externally
      3. Now that it is provided, we can depend on it in our app
   * Of course, we can provide custom deps that we create (i believe companies use some custom deps) and we manually add those directly to repos or set it up in such a way that it downloads from company server

3. Which command should you use to build all projects?
   * mvn clean install and we should execute it where parent pom resides
4. Which command should you use if you only want to execute tests?
   * mvn test as it will only execute the test classes
   * it will also execute pre-steps clean,validate and compile
5. Where is the jar file stored?
   * They are all stored inside of ~/.m2/repository and here you can find specific dependencies and jars inside them
6. How are jars called after changing version?
   * First it was helloworld-1.0-SNAPSHOT







## Authors

Contributors names and contact info

* Dalibor Veselinovic
