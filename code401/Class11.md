# Spring

## Spring App Basics
Steps To build a basic Spring app 

* For Gradle, visit the Spring Initializr to generate a new project with the required dependencies (Spring Web, Thymeleaf, and Spring Boot DevTools). 
* Create a Web Controller
  
    In Spring HTTP requests are handled by a controller.

    We can identify the controller by the @Controller annotation.

    A View is responsible for rendering the HTML content.

    Controllers handles GET requests  by returning the name of a View.
    ```
    Web Controller Example:
    package com.example.servingwebcontent;

    import org.springframework.stereotype.Controller;
    import org.springframework.ui.Model;
    import org.springframework.web.bind.annotation.GetMapping;
    import org.springframework.web.bind.annotation.RequestParam;

    @Controller
    public class GreetingController {

        @GetMapping("/greeting")
        public String greeting(@RequestParam(name="name", required=false, defaultValue="World") String name, Model model) {
            model.addAttribute("name", name);
            return "greeting";
        }

    }
    ```

* Spring Boot Devtools it is used To speed up the refresh cycle by:
   
    * Enables hot swapping.

    * Switches template engines to disable caching.

    * Enables LiveReload to automatically refresh the browser.

    * Other reasonable defaults based on development instead of production.

* Run the Application

    The main() method uses Spring Boot’s SpringApplication.run() method to launch an application.

## Spring MVC and Thymeleaf:how to access data from templates

In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered. This model map allows for the complete abstraction of the view technology and, in the case of Thymeleaf, it is transformed into a Thymeleaf context object (part of the Thymeleaf template execution context) that makes all the defined variables available to expressions executed in templates.

* Spring model attributes

    Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.
    ```
    Example of adding model attributes to a view in Spring MVC iva method:
    @RequestMapping(value = "message", method = RequestMethod.GET)
            public String messages(Model model) {
                model.addAttribute("messages", messageRepository.findAll());
                return "message/list";
            }
    ```        
* Request parameters
   
   Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server like:

   ```
   https://example.com/query?q=Thymeleaf+Is+Great!
   ```
* Session attributes

    add mySessionAttribute to session:
    ```
    @RequestMapping({"/"})
        String index(HttpSession session) {
            session.setAttribute("mySessionAttribute", "someValue");
            return "index";
        }
    ```
    


