## Stream creation

```java
public class Main {
    public static void main(String args[]) {
        List<Person> persons = new ArrayList<>();
        Stream<Person> stream = persons.stream();
        stream.forEach(System.out::println);
    }
}
```
