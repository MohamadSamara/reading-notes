**What database engine is Room wrapped around?**
Room is wrapped around SQLite, a lightweight, embedded database engine that is widely used in mobile development. SQLite is a good choice for Room because it is efficient, reliable, and easy to use. It also has a small footprint, which is important for mobile devices.

**Do you think this is a good choice? Why or why not?**
I think SQLite is a good choice for Room because it is a well-established and proven database engine. It is also a good choice for mobile development because of its small footprint and efficiency. Additionally, SQLite is supported by all major mobile platforms, which makes it a good choice for developers who want to create cross-platform applications.

**Do Rooms have any similarities to JPA?**
Yes, Room and JPA are both object-relational mapping (ORM) frameworks. ORMs allow developers to map Java or Kotlin objects to database tables, simplifying the process of storing and retrieving data.

**Describe a DAO in your own words**
A DAO, or Data Access Object, is a design pattern that provides an abstraction layer for accessing database data. DAOs allow developers to interact with the database without having to know the underlying SQL code. This makes it easier to write and maintain database code.

In Room, DAOs are used to define the methods that can be used to interact with database entities. For example, a DAO for the `House` entity might have methods for creating, reading, updating, and deleting houses.

Here is an example of a DAO in Room:

```
@Dao
interface HouseDao {
    @Insert
    fun insertHouse(house: House)

    @Update
    fun updateHouse(house: House)

    @Delete
    fun deleteHouse(house: House)

    @Query("SELECT * FROM houses")
    fun getAllHouses(): List<House>
}
```

To use the `HouseDao`, a developer would simply call the appropriate method. For example, to insert a new house into the database, they would call the `insertHouse()` method.

DAOs can be used to simplify the process of interacting with databases and make database code more maintainable.
