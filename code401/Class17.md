# Spring Authorization

## Spring Boot and OAuth2

To create a minimal application that uses GitHub for authentication:
1. Creating a New Project

   go to `https://start.spring.io` and generate an empty project. 

2. Add a Home Page

   create index.html in the src/main/resources/static folder.

3. Securing the Application with GitHub and Spring Security

   add Spring Security as a dependency. 

4. Add a New GitHub App
   
   * Select "New OAuth App" and then the "Register a new OAuth application"
   * Enter an app name and description.
   * Then, enter your app’s home page
   * Indicate the Authorization callback URL as http://localhost:8080/login/oauth2/code/github and click Register Application.
5. Configure application.yml

   to make the link to GitHub, add the following to your `application.yml`: 
   ```
   spring:
   security:
    oauth2:
      client:
        registration:
          github:
            clientId: github-client-id
            clientSecret: github-client-secret
   ``` 
6. Boot Up the Application
7. Making the Home Page Public
8. Add a Logout Button
9. Adding a Logout Endpoint   
10. Login with GitHub:

    * Initial setup.
    * Setting the redirect URI.
    * Adding the Client Registration.
    * Adding the Login Link 
11. Adding an Error Page for Unauthenticated Users

