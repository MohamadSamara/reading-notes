# Read Class 13

## One-to-Many Relationships

- Name a few real life examples of “One To Many” relatioships.

  - A **one-to-many** relationship is a type of association where one entity can be related to many other entities, but the other entities can only be related to one entity. Some real life examples of one-to-many relationships are:
    - A **mother** and her **children**. A mother can have many children, but each child can only have one biological mother.
    - A **country** and its **cities**. A country can have many cities, but each city can only belong to one country.
    - A **teacher** and his or her **students**. A teacher can teach many students, but each student can only have one teacher for a specific subject.

- Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

  - If we wanted to create a one-to-many relationship with Player and Team entities, we would make **Team** the **one** and **Player** the **many**. This means that a team can have many players, but each player can only belong to one team at a time.

- Explain one to many relationships to a non-technical friend.

  - A one-to-many relationship is a way of describing how different things are connected to each other. For example, imagine you have a collection of books and each book has an author. You can say that there is a one-to-many relationship between authors and books, because one author can write many books, but each book can only have one author. Another example is your family tree. You can say that there is a one-to-many relationship between your parents and your siblings, because your parents can have many children, but each child can only have one pair of parents.

## Spring Integration Testing

- Describe the difference between a unit test and an integration test.

  - A unit test is a type of testing that checks the functionality of a single component or unit of code, such as a method or a class. A unit test is usually written by the developer who wrote the code and it is used to verify that the code works as expected and does not have any bugs or errors. An integration test is a type of testing that checks how different components or units of code work together as a whole system, such as an application or a service. An integration test is usually written by a tester who uses the code and it is used to verify that the system meets the requirements and specifications and does not have any compatibility or performance issues.

- What is the object that provides support for Sprin MVC Testing?

  - The object that provides support for Spring MVC Testing is the **MockMvc** object. The MockMvc object allows us to perform requests to the Spring MVC controllers and assert the responses using various methods and matchers. The MockMvc object can be created using the **MockMvcBuilders** class, which provides different ways of configuring and building the MockMvc object.

- What does the “perform()” method do in a Spring integration test?
  
  - The `perform()` method in a Spring integration test is used to execute a request to the Spring MVC controllers using the MockMvc object. The `perform()` method takes a **RequestBuilder** object as an argument, which defines the details of the request, such as the HTTP method, the URL, the parameters, the headers, etc. The `perform()` method returns a **ResultActions** object, which allows us to chain various methods to verify and analyze the response from the controller. For example, we can use methods like `andExpect()`, `andDo()`, `andReturn()`, etc
