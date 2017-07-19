## Collectors

* Another type of reduction called "mutable reduction"
* Instead of aggregating elements, this reduction put them in a container

```java
public class Main {
    public static void main(String args[]) {
        List<Person> persons = Stream.of(
                new Person().setEmail("jntakpe@gmail.com").setFirstname("Jocelyn").setLastname("NTAKPE").setAge(30),
                new Person().setEmail("cbarillet@gmail.com").setFirstname("Cyril").setLastname("BARILLET").setAge(34),
                new Person().setEmail("smaitre@gmail.com").setFirstname("Sebastien").setLastname("MAITRE").setAge(38)
        ).collect(Collectors.toList());
        Function<Person, String> fullName = p -> p.getFirstname() + " " + p.getLastname();
        String names = persons.stream()
                .map(fullName)
                .collect(Collectors.joining(", "));
        ///
        List<String> nameList = persons.stream()
                .map(fullName)
                .collect(Collectors.toList());
    }
}
```

