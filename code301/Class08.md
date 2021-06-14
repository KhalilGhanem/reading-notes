# APIs

1. What does REST stand for?

    Representational State Transfer.

2. REST APIs are designed around a resources.

3. What is an identifer of a resource? Give an example.

    A URI that uniquely identifies that resource. EX:``` https://adventure-works.com/orders/1```

4. What are the most common HTTP verbs?

     GET, POST, PUT, PATCH, and DELETE

5. What should the URIs be based on?

    URIs should be based on nouns (the resource) 

6. Give an example of a good URI.

    ```https://adventure-works.com/orders```

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    * "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.
    * It's a bad thing and we should avoid using it.

8. What status code does a successful GET request return?

    HTTP status code 200 (OK).


9. What status code does an unsuccessful GET request return?

    HTTP status code 404 (Not Found).


10. What status code does a successful POST request return?

    HTTP status code 201 (Created).


11. What status code does a successful DELETE request return?

    HTTP status code 204.


