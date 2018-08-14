# Examples of decomposition in Java

## Association 
> is a relationship loosele coupled between two objects

This example shows the association between a food object and a wine object.

```java
public class Wine{
  public void pair(Food food) {
    execute.pair(food);
  }
}
```

## Aggregation 
> is a "has-a" relashionship where a whole has parts that belong to it. this parts is considered weak. 
> Meaning that altohough parts can belong to the wholes, they can also exist independently. examples:

a. bookshelf - book.
b. petstore -  pet
c. plane - crew.
d. student - courses.

```java
  public class PetStore{
    private ArrayList<Pet> pets;
    
    public PetStore(){
      pets = new Arralist<Pet>();
    }
    
    public void add( Pet pet){...}
  }
```

## Composition 
> Is an exclusive containment of parts, otherwise known as "strong" has-a relationship. 
> Meaning that the whole can't exist without any of his parts.

Example a relationship between a house and a room, if we don't have a house the room doesn't exists.

Example of an employee and his salary
```java
public class Employee{
  private Salary salary;
  
  public Employee(Salary employeeSalary){
    this.salary = employeeSalary;
  }
}
```
