# CRUD

## Status Codes Based On REST Methods

**In your own words, describe what each group of status code represents:**

100’s = the request has been recieved from the client and waiting the server to comply .
200’s = success request , tells the client that the request has been accepted.
300’s = redirection , which means that the request that have been srnt to the server is invalid.
400’s = client error , invalid request.
500’s = server errors

**What is a status code 202?**

the request has been accepted for processing, but the processing has not been completed.

**What is a status code 308?**

indicates that the resource requested has been definitively moved to the URL given by the Location headers.

**What code would you use if an update didn’t return data to a client?**

204 No Content

**what code would you use if a resource used to exist but no longer does?**

410

**What is the ‘Forbidden’ status code?**

403 Forbidden client error status response code indicates that the server understood the request but refuses to authorize it.

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

to be access in heroku.

**What is middleware?**

Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. 
Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

**What does app.use(express.json()) do?**

recognize the incoming Request Object as a JSON Object.

**What does the /:id mean in a route?**

It's mean a key of object which you are shown in the database and declared by default.


**What is the difference beween PUT and PATCH?**

when you want to update a resource with PUT request, you have to send the full payload as the request whereas with PATCH ,
you only send the parameters which you want to update. Related: Suppose we have a resource that holds the first name and last name of a person.

**How do you make a default value in a schema?**

Make mongoose string schema type default value as blank and make the field optional. 
testschema = mongoose. Schema({ name:{ type:String, required:true, unique:true }, image:{ type:String, required:true }, category:{ type:String }, })/

**What does a 500 error status code mean?**

Internal Server Error server error response code

**What is the difference between a status 200 and a status 201?**

Successful. The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed.
A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

## Things I want to know more about

CRUD