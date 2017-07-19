## Method reference

Just another syntax to write a lambda.

```java
public class Main {
    public static void main(String[] args) {
        Consumer<String> consumer  = s -> System.out.println(s);
        Consumer<String> consumer2  = System.out::println;
        
        Comparator<Integer> comparator = (i1, i2) -> Integer.compare(i1, i2);
        Comparator<Integer> comparator2 = Integer::compare;
    }
}
```
