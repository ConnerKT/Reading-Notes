# CRUD Notes

This topic is important to me because I want to learn how to implement a persistent storage app.

## [Retrospective 12](https://connerkt.github.io/Reading-Notes/301/Class12/Retro12)

## References

[Status Codes for REST](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/).

[Building A REST API with Node,Express,and Mongo](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw).

## Status Code Based On REST Methods

**HTTP Status Codes** is from 100-600 that is part of a HTTP response. The first digit defines the class of the status. Understanding the class behind a code helps us locate problems.

100-199: Informational status codes, usually tell the client that the header part of the request has been received and the server will try to comply wit ha transmission demand of the client.

200-299: Success Codes.

300-399: Redirection Codes, they tell the client that the resource they are requesting isn't available at the expected location anymore.

400-499: Client Error Codes, all about invalid requests a client sent to a server.

500-599: Server Error Codes, Overwhelmed server, or unreachable servers.

Anything above 599 is a custom class but aren't permitted but people use them anyways. (beware)

**CRUD** (Create, Read, Update, Delete)

They make up the lions-share of API endpoints.

**Create** implemented via HTTP's post method, used to create new resources or access tokens.

**Read** Get method, and used to fetch resource representations.

**Update** Put or Patch method,
PUT requires the client to send an entire representation of a resource to update it. (Replace the old one with the new one).

PATCH requires the client only send parts of the representation of the resource to update it. (Add, update or delete these parts in the old version).

**Delete** delete method from http, to delete...

### Status Code Based On REST Methods Questions

1. In your own words, describe what each group of status code represents:

100’s =
200’s =
300’s =
400’s =
500’s =

2. What is a status code 202?
3. What is a status code 308?
4. What code would you use if an update didn’t return data to a client?
5. What code would you use if a resource used to exist but no longer does?
6. What is the ‘Forbidden’ status code?

### Status Code Based On REST Methods Answers

1. Below
100’s =Used to inform the request has been received.
200’s = Used to tell you your request succeeded.
300’s = To tell you the request is redirected, and to use a different location.
400’s = This is given when the client makes a mistake, usually wrong URI or missing auth.
500’s = This is a server issue, usually with a bad link, or unreachable.

2. This means it was accepted/
3. This tells the user to use a another URL.
4. 204
5. 404
6. 403

## Build A REST API With Node.js, Express, & MongoDB

[Video](https://www.youtube.com/watch?v=fgTGADljAeg&t=538s)

### Build A REST API With Node.js, Express, & MongoDB Questions

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
2. What is middleware?
3. What does app.use(express.json()) do?
4. What does the /:id mean in a route?
5. What is the difference between PUT and PATCH?
6. How do you make a default value in a schema?
7. What does a 500 error status code mean?
8. What is the difference between a status 200 and a status 201?

### Build A REST API With Node.js, Express, & MongoDB Answers

1. To keep our database information hidden when deployed.
2. Code that runs when the server the server is requested.
3. It lets our server accept json as a body.
4. It lets us access data from a database with that id.
5. Patch is to update but put can change a resource but also upload.
6. The default property
7. It means theres an internal problem with the server.
8. 200 means successful request, 201 means successful creation.

## Things I want to know more about

I want to understand more about building fullstack applications.

I want to understand all the different status codes for REST Methods so I can debug my code and understand what's going on.

