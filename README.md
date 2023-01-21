# Workshop API en Java avec Spark

## Introduction

Java was designed to be easy to use and is therefore easy to write,
compile, debug, and learn than other programming languages. Java is
object-oriented. This allows you to create modular programs and reusable
code. Java is platform-independent.

**Java technology is used by more than 6 million developers and runs on
more than 5.5 billion devices.**

## Installation

What is MAVEN?
- Maven is a built automation tool.
- Maven is a tool that helps us create projects easyly.
### What is built?
- Creating, adding, compiling, testing and deploying a project.
  All of these combined are called a Built.
- Since maven is "built" automation tool, it helps us automate
  all of these steps.
### Similar tools like Maven ?
- ant
- gradle

### Most important file in a Maven project?
- pom.xml is the most important file in a Maven project.

You should install manually of with you favorite package manager Maven :
https://maven.apache.org/install.html

## Compile

To compile this Java program you should run :

```
mvn compile assembly:single
java -jar target/your-amazing-jar-file.jar
```

If it's not work, try to run with the new version or java or directly with
your IDE like Jetbrain IntelliJ.
https://www.jetbrains.com/fr-fr/idea/

PS: Fuck VS Code for Java !

## How to start ?

Module to add in maven: https://mvnrepository.com/artifact/com.sparkjava/spark-core

You can found more help here: https://sparkjava.com/

## exercise

### Exercise 1

Route: /hello-world  
Type: GET  
Description: Make a '/hello' endpoint that display always "Hello World!"  
Status: Always 200

### Exercise 2

Route: /message?message="xxxxx"  
Type: GET  
Description: Make a endpoint that display the message argument  
Status: 200 and message if not return 400 and "Bad request

### Exercise 3

Route: /header  
Type: GET  
Description: Make a endpoint that if the request contains a `message` header  
Status: 200 and message if not return 400 and "Bad request"

### Exercise 4

Route: /body  
Type: POST  
Description: Make a endpoint that if the request contains a `message` body  
Status: 200 and message if not return 400 and "Bad request"

/!\ The body is on json format !  
Tips: use JSON.parse(message)

### Exercise 5

Route: /cookie  
Type: GET  
Description: Make a endpoint that if the request contains a `message` cookie  
Status: 200 and message if not return 400 and "Bad request"

### Exercise 6

Route: /admin  
Type: GET  
Make a '/private' with a middleware that check if the `Authorization` header contain exactly this password: `EPITECH`  and username: `koala`
Status: 200 and message "Welcome to admin page" if not return 400 and "Bad request"