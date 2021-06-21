# CRUD

## Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

    100’s = The informational status codes.

    200’s = The success codes.

    300’s = The redirection codes.

    400’s = The client error codes

    500’s = The server error codes.

2. What is a status code 202?

   Accepted code It is used for asynchronous processing, This code tells the client that the request was valid, but its processing will finish sometime in the future.

3. What is a status code 308?

    Permanent Redirect code This tells the client to use another URL to access the resource and not use the current URL anymore.

4. What code would you use if an update didn’t return data to a client?
   
   204 No Content

5. What code would you use if a resource used to exist but no longer does?

    410 Gone

6. What is the ‘Forbidden’ status code?

   The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.
