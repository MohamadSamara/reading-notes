# Read Class 12

**How are query methods defined when using Spring Data JPA?**

- Query methods are defined by using keywords inside method names that follow a certain syntax. For example, `findByLastname(String lastname)` is a query method that finds entities with a specific last name.

**Which dependencies will you need in order to complete the Spring guide?**

- If you are using Gradle, you will need the following dependencies in your `build.gradle` file: `spring-boot-starter-data-jpa`, `spring-boot-starter-web`, `com.h2database:h2`, and `org.springframework.boot:spring-boot-starter-test`.

**What annotations are used to specify an auto generated identification number for an Entity?**

- You can use the annotations `@Id` and `@GeneratedValue` to specify an auto generated identification number for an Entity. For example, `@Id @GeneratedValue Long id`.

**Which of the Spring Data Repositories covered in the readings has the most methods available to it?**
  
- The JpaRepository interface has the most methods available to it, as it extends both PagingAndSortingRepository and CrudRepository interfaces.

**Name a downside of a Spring Data Repository.**

- A possible downside of a Spring Data Repository is that it may not be able to handle complex queries or custom logic that require more flexibility and control.

**How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?**

- You could define an operation to find a student based on their name by using the keyword `findByName` in the method name. For example, `Student findByName(String name)`.
