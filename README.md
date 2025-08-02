# Blogging-application
Blogging application with spring boot

Blogging application: 

Reat time rest apis for blogging application using SpringBoot, Spring Security , JWT Spring Data JPA(Hibernate) and MYSQL.

Creating Respoints, JPA Entities, Role Based Authentication, Handling Exceptions
Using DTO for data Transfer,
Swagger (providing ducumentation for data) 

Client-Server Architecture : clint request and in server api will execute those api will communicate with dataBase(Creating objects, data) and lter sends back to client.
Data exchange: JSOn or XML
Client: Consumer
Server: Provider

REST: Representation State Transfer: Created by Roy Fielding to guide the design of Archietecture. for the web
Tranfer data beween parties(Clint and Transfer)
State: DataRepresentaitional: XML, JSOn

REST Guideline:
Client Server Archietecture: 
Server Stateless
Cachaeble: For same data (reuse data)
Layered Archietecture
Uniform interface
Code on Demand

REST Concepts:
Resource, Sub Resource, URI,, HTTp methods, Http response codes
Resource: anything we want to expose to outside world Like library book inside library mangement system is resource
Uniform Resource Identifier: Identify resource like get , post , put , delete. With the help of url we identify which resource we are pointing to inside sttp url.

HTTP defines the set of requests method to indicate the desired action to be performed. for a given resourceSTTP status code detects if specific request has been completed or not.
 200 ok: Request is Successful.
 201 Created Request is succesful and new resource created
 401 unauthorized
 404 not found
 500 Internal server error
 
 Requirements: Clients wants blogging application where he can write blogs and articles.
 user can comment on the blogs/articles
 
 1. User can create update delete and list posts.
 2. User Should add update delete comments on posts.
 3. Categorizes the post according to Categories.
 4. New User should able to register on our application
 5. Post include one picture too.

Needs:
Proper login and register api
posts api includes pagination and sorting
Proper user input validation handling
Proper Exception handling
Role based authentication based security with apis
Document all rest apis so that consumer can easily understand
deploy backend application (AWS cloud)

Framework: SpringBoot Java Framework
Java8+ , Maven, STS, apache tomcat, MySqL Database, postman , Swagger(Documentation)

Resources of application: User: login and logout
Categories:
Post Resource: Articles
Comments:

Postman: Request-> Controllers: -> Services(logic execute) -> Repositiories(DAO) -> Database
         Response<--  
		 Api layers, Business logic and DAO layer
		 
		 User ke paas: id, name, email, password or about (1 user can create multiple posts)
		 Post: post_id, title, content, image, user_id (post can have many commentsb), userId, categoryid
		 Comment: user_id, comment_id, comment, post_id (1 to msny user can have multiple comments)
		 1 category can allow multiple post. Category id 
		 
		  
		  Creating enpoints:
		  Complex db structures(JPA entities)
		  Role based authentication
		  Handling exception
		  Using DTO for data transfer
		  swagger
		  Add profiles for different enviornments
		  deploy spring boot in productions(Amazon aws)
		  
		 # Java Bean validated with JSR 380 as Bean validation 2.0.JSR 380 is specification for the java api for bean validation
		 For validation different annotation is used like @NotNull, @Min,@Size etc. Hibernate Validator is implementation of Bean validation Api.
		 
		 @NotNull: 
		 
		 210620688
		  

