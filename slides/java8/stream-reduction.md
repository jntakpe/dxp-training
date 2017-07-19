## Stream reduction

```java
public class Main {
    public static void main(String args[]) {
        List<Integer> ages = Arrays.asList(30, 34, 38);
        Integer sum = ages.stream().reduce(0, (a1, a2) -> a1 + a2);
    }
}
```

** Reductions are terminal operations **

Available reductions :

* max(), min(), count()
* allMatch(), noneMatch(), anyMatch()

