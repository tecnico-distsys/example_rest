# REST Server example

This is a simple REST Service.

The service runs in a standalone HTTP server, started by the Main class.

The resource is defined by the MyResource class and mapped to HTTP through annotations specified by [JAX-RS (Java API for RESTful Web Services)](https://en.wikipedia.org/wiki/Java_API_for_RESTful_Web_Services).

The service is described by a generated [WADL](https://en.wikipedia.org/wiki/Web_Application_Description_Language) document.

## Instructions using Maven:

To compile:

```
mvn compile
```

To run the tests:

```
mvn test
```

To run using _exec_ plugin:

```
mvn exec:java
```

When running, the REST service awaits connections from clients.  
You can check if the service is running using your web browser.

To call the service, retrieve (GET) the following URL:  
<http://localhost:8080/myapp/myresource>

To see the generated WADL file, go to:  
<http://localhost:8080/myapp/application.wadl>

For a more detailed version, add a detail parameter:  
<http://localhost:8080/myapp/application.wadl?detail=true>

## To configure the Maven project in Eclipse:

'File', 'Import...', 'Maven'-'Existing Maven Projects'

'Select root directory' and 'Browse' to the project base folder.

Check that the desired POM is selected and 'Finish'.

----

[SD Faculty](mailto:leic-sod@disciplinas.tecnico.ulisboa.pt)
