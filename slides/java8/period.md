## Period

* Human representation of a period

```java
public class Main {
    public static void main(String[] args) {
        Period.ofMonths(3);
        LocalDate birthDate = LocalDate.of(1986, Month.SEPTEMBER, 25);
        Period.between(birthDate, LocalDate.now())
    }
}
```
