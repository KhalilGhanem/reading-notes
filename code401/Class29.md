# Room

## Save data in a local database using Room   
The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite. In particular, Room provides the following benefits:
* Compile-time verification of SQL queries.
* Convenience annotations that minimize repetitive and error-prone boilerplate code.
* Streamlined database migration paths.

### Primary components
**There are three major components in Room:**
* The `database class` that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
* `Data entities` that represent tables in your app's database.
* `Data access objects (DAOs)` that provide methods that your app can use to query, update, insert, and delete data in the database.

### Database
The `AppDatabase class` is hold the database. AppDatabase defines the database configuration and serves, The database class must satisfy the following conditions:
* The class must be annotated with a `@Database` annotation that includes an entities array that lists all of the data entities associated with the database.
* The class must be an abstract class that extends `RoomDatabase`.
* For each DAO class that is associated with the database, the database class must define an abstract method that has zero arguments and returns an instance of the DAO class.

## Defining data using Room entities 
When you use the Room persistence library to store your app's data, you define entities to represent the objects that you want to store. Each entity corresponds to a table in the associated Room database, and each instance of an entity represents a row of data in the corresponding table, so we can use Room entities to define your database schema without writing any SQL code.

We define each Room entity as a class that is annotated with `@Entity`. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

### Define a primary key
Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.

### Define a composite primary key
If you need instances of an entity to be uniquely identified by a combination of multiple columns, you can define a composite primary key by listing those columns in the primaryKeys property of `@Entity`.

### Ignore fields
By default, Room creates a column for each field that's defined in the entity. If an entity has fields that you don't want to persist, you can annotate them using `@Ignore`.

## Define relationships between objects 
The most object-relational mapping libraries allow entity objects to reference each other, **Room** explicitly forbids this. 

### Create embedded objects
If we want to express an entity or data object as a cohesive whole in the database logic, even if the object contains several fields. In these situations, we can use the `@Embedded` annotation to represent an object that we like to decompose into its subfields within a table.

### Define one-to-one relationships
 A one-to-one relationship between two entities is a relationship where each instance of the parent entity corresponds to exactly one instance of the child entity, and vice-versa.

### Define one-to-many relationships
A one-to-many relationship between two entities is a relationship where each instance of the parent entity corresponds to zero or more instances of the child entity, but each instance of the child entity can only correspond to exactly one instance of the parent entity.