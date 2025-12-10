# phasezero-catalog-service
A Spring Boot–based Project Product Catalog Microservice built using Java 8 and 17, Spring web, Spring Boot, Spring Data JPA, and H2 in-memory database.
And we can run it on our localhost (url :- http://localhost:8080/h2-console )
PhasezeroCatalogServiceApplication is the main class which is the starting or entry point of the project.
In this project, I have make 7 layers which are, Entity layer, Dao layer, Service layer, Controller layer, Dto layer, Exception layer.
I have make use of the following endpoints :-
1.  /products
2.  /products/search/{partName}
3.  /products/filter/{category}
4.  /products/sort
5.  /products/inventory/value
    where /products is the base url for all the api which is written in @RequestMapping("/products") as class level annotation.
    /products/search/{partName} in this url /products is the base url and rest /search/{partName} is define in the @GetMapping(/search/{partName}) which is a method level annotation.
    I use @RequestBody for bind HttpRequestBody with method parameter in the controller, helps to read the JSON object sent over the request and converts it into Java Object.
    I use @PathVariable forextract value from the path of the url.

Here are some Assumptions
1. All product names normalized to lowercase
2. H2 resets data every restart
3. Category filter is case-insensitive
4. and many more which is good for the basic project

In future I will update this project by adding 
1. Pagination
2. delete
3. add list of products at a time
4. authentication
5. and many more

Thank you for visiting my profile
Keep in touch I will update this project in the future by adding some more features.

    
    

