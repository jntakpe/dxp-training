## Optional if empty

```java
public class Main {
    public static void main(String args[]) {
        PersonService personService = new PersonService();
        Person toto = personService.findByLogin("toto")
                .orElse(new Person().setFirstname("Toto").setLastname("toto").setEmail("toto@mail.com").setAge(18));
        toto = personService.findByLogin("toto")
                .orElseGet(() -> new Person().setFirstname("Toto").setLastname("toto").setEmail("toto@mail.com").setAge(18));
        toto = personService.findByLogin("toto")
                .orElseThrow(() -> new IllegalStateException("toto is not found"));
    }
}
```
