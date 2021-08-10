# Related Resources and Integration Testing

## Related data in Spring

* One-to-One Relationship

    We can define it using `@OneToOne` annotation.

* One-to-Many Relationship

    We can define it using `@OneToMany` and `@ManyToOne` annotations.

* Many-to-Many Relationship

    We can define it using `@ManyToMany ` annotation.

## Steps to create relationships between entities in Spring
1. Create the Model classes.
2. create the Repositories interfaces for each of classes.
3. Create the Resources
4. Create the Associations

```

One-to-one exampe:
Library Table
@Entity
public class Library {

    @Id
    @GeneratedValue
    private long id;

    @Column
    private String name;

    @OneToOne
    @JoinColumn(name = "address_id")
    @RestResource(path = "libraryAddress", rel="address") //we use it to customize the endpoint.
    private Address address;
    
    // standard constructor, getters, setters
}

Address Table
@Entity
public class Address {

    @Id
    @GeneratedValue
    private long id;

    @Column(nullable = false)
    private String location;

    @OneToOne(mappedBy = "address")
    private Library library;

    // standard constructor, getters, setters
}
//create the Repositories
public interface LibraryRepository extends CrudRepository<Library, Long> {}
public interface AddressRepository extends CrudRepository<Address, Long> {}
```
## Integration Testing in Spring
Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.

### Testing steps:
* Preparation: we need  junit-jupiter-engine, junit-jupiter-api, and Spring test dependencies.
* Test Configuration:

    * Enable Spring in Tests with JUnit 5
    * The WebApplicationContext Object
    * Mocking Web Context Beans
    * Verify Test Configuration

* Writing Integration Tests:   
    
    * Verify View Name
    * Verify Response Body
    * Send GET Request With Path Variable
    * Send GET Request With Query Parameters
    * Send POST Request
    



