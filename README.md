# Automated Deployment of a Java Web Application
Enabling  continuous  integration  and  continuous  deployment  (CI/CD)  for  a Java-based web application.

#Jenkins pipeline must be built as a script or using Pipeline from SCM.

#Project Directory Structure
NumberGuessGame/
|-- src/
|   |-- main/
|   |   |-- java/com/studentapp/NumberGuessServlet.java
|   |   |-- webapp/WEB-INF/web.xml
|   |   |-- webapp/index.jsp
|-- pom.xml
|-- README.md
|-- .gitignore
# Number Guess Game
A simple Java web application that lets users play a number guessing game.

## How to Run
1. Clone the repository.
2. Build with Maven: `mvn package`
3. Deploy the `NumberGuessGame.war` to Tomcat.
