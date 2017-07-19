## Optional create

```java
public class Main {
    public static void main(String args[]) {
        Optional<String> opt = Optional.of("non_null_value");
        opt = Optional.ofNullable("possible_null_value");
        opt = Optional.empty();
    }
}
```
