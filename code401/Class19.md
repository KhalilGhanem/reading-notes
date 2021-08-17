# Real time messaging with websockets

websocket:is a thin, lightweight layer above TCP. This makes it suitable for using “subprotocols” to embed messages.

STOMP: which stand for `Simple (or Streaming) Text Oriented Message Protocol` is a subprotocol operating on top of the lower-level WebSocket.

We use STOMP messaging with Spring to create an interactive web application.
## Steps to make an interactive web application using WebSocket. 
* Generate a new project using Spring Initializr with Websocket dependency.
* Adding Dependencies.
  ```
  Gradle user:
    implementation 'org.webjars:webjars-locator-core'
    implementation 'org.webjars:sockjs-client:1.0.2'
    implementation 'org.webjars:stomp-websocket:2.3.3'
    implementation 'org.webjars:bootstrap:3.3.7'
    implementation 'org.webjars:jquery:3.1.1-1'
  ```
* Create a Resource Representation Class.
  ```
  package com.example.messagingstompwebsocket;

  public class HelloMessage {

  private String name;

  public HelloMessage() {
  }

  public HelloMessage(String name) {
    this.name = name;
  }

  public String getName() {
    return name;
  }

  public void setName(String name) {
    this.name = name;
   }
  }
  ```
* Create a Message-handling Controller
  ```
  package com.example.messagingstompwebsocket;

    import org.springframework.messaging.handler.annotation.MessageMapping;
    import org.springframework.messaging.handler.annotation.SendTo;
    import org.springframework.stereotype.Controller;
    import org.springframework.web.util.HtmlUtils;

    @Controller
    public class GreetingController {


    @MessageMapping("/hello")
    @SendTo("/topic/greetings")
    public Greeting greeting(HelloMessage message) throws Exception {
        Thread.sleep(1000); // simulated delay
        return new Greeting("Hello, " + HtmlUtils.htmlEscape(message.getName()) + "!");
     }

    }
  ```  
* Configure Spring for STOMP messaging.
* Create a Browser Client.
* Make the Application Executable.