# WRRC and Java

## Review: High-level HTTP

The HTTP Request Lifecycle:

* Local Processing
* Resolve an IP
* Establish a TCP Connection
* Send an HTTP Request
* Tearing Down and Cleaning Up

## Java HTTP Request example

To create a Simple HTTP Request in Java we used HttpUrlConnection class.

**HttpUrlConnection:** this class allows us to perform basic HTTP requests without the use of any additional libraries. 

Steps to create HTTP Request:

* Creating a Request

    We can create an HttpUrlConnection instance using the openConnection() method of the URL class.
    ```
    ex:
    URL url = new URL("http://example.com");
    HttpURLConnection con = (HttpURLConnection) url.openConnection();
    con.setRequestMethod("GET");
    ```

    HttpUrlConnection class is used for all types of requests:(GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE)

* Adding Request Parameters

    we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream.

* Setting Request Headers

    Adding headers to a request can be achieved by using the setRequestProperty() method:

* Configuring Timeouts
* Handling Cookies
* Handling Redirects
* Reading the Response
