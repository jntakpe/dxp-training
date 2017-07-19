## Stream lazy

What does this code do ?

```java
public class Main {
    public static void main(String args[]) {
        List<Person> persons = Stream.of(
                new Person().setEmail("jntakpe@gmail.com").setFirstname("Jocelyn").setLastname("NTAKPE").setAge(30),
                new Person().setEmail("cbarillet@gmail.com").setFirstname("Cyril").setLastname("BARILLET").setAge(34),
                new Person().setEmail("smaitre@gmail.com").setFirstname("Sebastien").setLastname("MAITRE").setAge(38)
        ).collect(Collectors.toList());
        List<Person> grandpas = new ArrayList<>();
        Stream<Person> stream = persons.stream();
        Predicate<Person> predicate = p -> p.getAge() > 35;
        stream
                .peek(System.out::println)
                .filter(predicate)
                .peek(grandpas::add);
        //What does this code do ?
    }
}
```


