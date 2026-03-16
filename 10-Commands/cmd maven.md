Here is a comprehensive Maven (mvn) Cheat Sheet in Markdown format. Maven is a build automation tool primarily used for Java projects to manage dependencies and the build lifecycle. 
Apache Maven
Apache Maven
 +1
🛠️ Basic Maven Lifecycle Commands
Maven commands typically execute a specific "phase" in a sequence. Running a later phase (like install) automatically runs all previous phases (like compile and test). 
DigitalOcean
DigitalOcean
 +3
Command 	Description
mvn clean	Deletes the target directory (removes old build files)
mvn validate	Checks if the project is correct and all info is available
mvn compile	Compiles the source code into .class files
mvn test	Runs unit tests using frameworks like JUnit
mvn package	Packages compiled code into a distributable format (e.g., JAR or WAR)
mvn verify	Runs integration tests and checks the package quality
mvn install	Installs the package into your local repository (~/.m2)
mvn deploy	Copies the final package to a remote repository for others to use
🚀 Common Combined Commands
Command 	Description
mvn clean install	The most common command; cleans old files and rebuilds everything
mvn clean package -DskipTests	Builds the project but skips running tests to save time
mvn clean install -U	Forces an update of all project dependencies
🔍 Dependency & Project Info
Command 	Description
mvn dependency:tree	Displays a visual tree of all project dependencies
mvn dependency:analyze	Identifies unused or undeclared dependencies
mvn help:effective-pom	Displays the final XML of your pom.xml after all inheritance
mvn --version (or -v)	Shows Maven version and Java environment details
📂 Creating a New Project
Command 	Description
mvn archetype:generate	Starts an interactive wizard to create a new project from a template
💡 Pro-Tips for Linux Users
Installation: On Ubuntu/Debian, use sudo apt install maven.
Parallel Builds: Use -T to speed up builds on multi-core CPUs (e.g., mvn -T 4 clean install uses 4 threads).
Debug Mode: Add -X to any command to see detailed debug logs if a build fails.