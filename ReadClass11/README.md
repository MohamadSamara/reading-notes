# READ Class 11

**Spring App Basics:**

1. **What role do the @Controller classes play in a Spring MVC application?**

- The @Controller classes play the role of handling HTTP requests and returning a view or a model object to the view layer of a Spring MVC application. They are annotated with @Controller to indicate that they are components that belong to the presentation layer.

2. **Explain to a non-technical friend what a GET request is.**

- A GET request is a way of asking a web server for some information. For example, when you type a web address in your browser, you are sending a GET request to the web server to get the web page you want to see. The web server responds by sending back the HTML code of the web page.

3. **What annotation should be placed on your Spring Boot application class?**

- The annotation that should be placed on your Spring Boot application class is @SpringBootApplication. This annotation enables auto-configuration, component scanning, and property support for your application.

**Spring MVC and Thymeleaf:**

1. **What method allows for a variable defined in Java (in your Spring Controller) to be displayed in HTML with the help of Thymeleaf?**

- The method that allows for a variable defined in Java (in your Spring Controller) to be displayed in HTML with the help of Thymeleaf is th:text. This method evaluates the expression inside the attribute and replaces the content of the tag with the result . For example, if you have a variable called name in your controller, you can display it in HTML like this:

```html
<p th:text="${name}">John</p>
```

2. **Explain the role of a @Controller class in a Spring MVC application.**

- A @Controller class in a Spring MVC application is responsible for receiving HTTP requests from the client, processing them, and returning a response. It can also add data to the model that will be used by the view layer to render the output. A @Controller class is usually mapped to a specific URL or a set of URLs that define its scope .

3. **What is a model attribute referred to in Thymeleaf?**

- A model attribute in Thymeleaf is a variable that can be accessed from the template. It can be added to the model by using the @ModelAttribute annotation on a method or a parameter in the controller, or by using the Model object directly. A model attribute can store any kind of data, such as strings, numbers, lists, maps, or custom objects .
