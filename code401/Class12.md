# Spring RESTful Routing & Static Files

## Spring RequestMapping

We use this @RequestMapping to map web requests to Spring Controller methods.


### RequestMapping Basics

* @RequestMapping — by Path
  ```
  @RequestMapping(value = "/ex/foos", method = RequestMethod.GET)
  @ResponseBody
  public String getFoosBySimplePath() {
    return "Get some Foos";
   }
  ``` 
* @RequestMapping — the HTTP Method
  ```
  @RequestMapping(value = "/ex/foos", method = POST)
  @ResponseBody
  public String postFoos() {
    return "Post some Foos";
  }
  ``` 
* RequestMapping and HTTP Headers

  * @RequestMapping With the headers Attribute
    ```
     @RequestMapping(
     value = "/ex/foos", 
     headers = { "key1=val1", "key2=val2" }, method = GET)
     @ResponseBody
     public String getFoosWithHeaders() {
      return "Get some Foos with Header";
     }  
    ```
  * @RequestMapping Consumes and Produces
     ```
     @RequestMapping(
     value = "/ex/foos", 
      method = GET, 
      headers = "Accept=application/json")
      @ResponseBody
     public String getFoosAsJsonFromBrowser() {
         return "Get some Foos with Header Old";
     }
     ```

## Spring Data Repositories
 
* CrudRepository: provides CRUD functions
* PagingAndSortingRepository:  provides methods to do pagination and sort records
* JpaRepository: provides JPA related methods such as flushing the persistence context and delete records in a batch

### CrudRepository
CRUD functionality
* save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
* findOne(…) – get a single entity based on passed primary key value
* findAll() – get an Iterable of all available entities in database
* count() – return the count of total entities in a table
* delete(…) – delete an entity based on the passed object
* exists(…) – verify if an entity exists based on the passed primary key value

