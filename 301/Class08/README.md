# API Notes

This topic is important to me because I want to utilize API's to create applications that involve a wide variety of data.

## [Retrospective 8](https://connerkt.github.io/Reading-Notes/301/Class08/Retro08)

## References

[Regular Expressions](https://regexr.com/).
[Tutorial for Regex](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285).
[Regex 101](https://regex101.com/).
[API Design Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design).

## API Design Best Practices

Most web applications use API's that clients can use.

A good design practice for these should aim to:
**Platform independence** - Any client should be able to call the API no matter how the API is implemented.

**Service evolution**- It should be able to evolve and add functionality independently from client applications.

**REST** - Proposed by Roy Fielding, its an architectural style for building distributed systems based on hypermedia.

REST isn't bound by specific implementations for API's, allowing variety in use.

REST Api's are designed around resources.

A resource has an identifier, which is a unique to that resource.
Ex. www.google.com/order/1

Clients interact with a service by exchanging representations of resources. Many use JSON.

Rest api's use HTTP verb to perform operations on resources.

The API design should be around the business entities. For example, they should be based on nouns(the resources) and not verbs(our operations.)

Try to limit your API being 'chatty', where your API expose a large number of small resources.

An API like this would require to send multiple request to find all the data that it requires. With a single request, it can lower this.

**API operations**: You have GET, POST, PUT, PATCH, AND DELETE.

**GET**: GETS a representation of the resource at the specified endpoint.
**POST**: Creates a new resource at the specified endpoint.
**PUT**: Either creates or replaces the resource at the specified endpoint.
**PATCH**: performs a partial update of a resource.
**DELETE**: well, it removes at that specified endpoint.

## API Design Best Practices Questions

1. What does REST stand for?
2. REST APIs are designed around a ____.
3. What is an identifier of a resource? Give an example.
4. What are the most common HTTP verbs?
5. What should the URIs be based on?
6. Give an example of a good URI.
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
8. What status code does a successful GET request return?
9. What status code does an unsuccessful GET request return?
10. What status code does a successful POST request return?
11. What status code does a successful DELETE request return?

## API Design Best Practices Answers

1. Representational State Transfer
2. Resources
3. Like a unique ID, www.google.com/account/1020020
4. GET,POST,PUT,PATCH,DELETE
5. Nouns, be predictable
6. www.google.com/account/settings
7. Its bad, it means when you have to target a bunch of different resources to get all the data you want, where you normally want to target one endpoint to get your data in a single request.
8. 200
9. 404
10. 201
11. 204

## Things I want to know more about

I want to know how to apply each operation on a resource, while also receiving it to my frontend.
I want to understand the best practices, so I can create perfect resources.