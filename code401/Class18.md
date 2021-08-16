# Hibernate Many to Many

## Many to Many relationship:
Example: Let's take the many-to-many association between two entities employee and project:
an employee can be assigned to multiple projects and a project may have multiple employees working for it.

To make Many to Many relationship we should make A join table between employee and project,
The join table require the primary keys of the two tables to connect both sides.

## Database Setup:
We  need to create the employee and project tables along with the employee_project join table with employee_id and project_id as foreign keys.

## The Model Classes:
The model classes Employee and Project need to be created with JPA annotations:
```
@Entity
@Table(name = "Employee")
public class Employee { 
    // ...
 
    @ManyToMany(cascade = { CascadeType.ALL })
    @JoinTable(
        name = "Employee_Project", 
        joinColumns = { @JoinColumn(name = "employee_id") }, 
        inverseJoinColumns = { @JoinColumn(name = "project_id") }
    )
    Set<Project> projects = new HashSet<>();
   
    // standard constructor/getters/setters
}
@Entity
@Table(name = "Project")
public class Project {    
    // ...  
 
    @ManyToMany(mappedBy = "projects")
    private Set<Employee> employees = new HashSet<>();
    
    // standard constructors/getters/setters   
}
```
**Both the Employee class and Project classes refer to one another, which means that the association between them is bidirectional.**
