## Optional operations

```java
public class Main {
    public static void main(String args[]) {
        PersonService personService = new PersonService();
        Optional<Person> opt = personService.findByLogin("toto");
        opt.map(Person::getFirstname)
                .map(String::trim)
                .filter(n -> n.length() > 0)
                .flatMap(personService::findAddressByStreet)
                .ifPresent(System.out::println);
    }
}
```
