# configuration

This is just a git repo where we can add all the different properties for different Micro services. These properties can be pulled by the config server
and provided to the required microservice. The file pulled is based on the name of the application.

e.g if the value of spring.application.name=app in the application properties of the application. The config file from this repo with name 
app.properties, app.yml and aplication.properties will be layered over and returned. Below is the sequence/
application.properties -> app.properties-> app.yml
