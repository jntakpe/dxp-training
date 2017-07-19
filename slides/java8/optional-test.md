## Testing optional

Classic version

```java
public class Main {
    public static void main(String args[]) {
        PersonService personService = new PersonService();
        Person toto = personService.findByLogin("toto");
        if (toto != null) {
            toto.setAge(18);
        }
    }
}
```

Optional version

```java
public class Main {
    public static void main(String args[]) {
        PersonService personService = new PersonService();
        Optional<Person> opt = personService.findByLogin("toto");
        opt.ifPresent(p -> p.setAge(18));
        //or
        if (opt.isPresent()) {
            opt.get().setAge(18);
        }
    }
}
```
