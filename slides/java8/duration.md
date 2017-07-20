## Duration

* Duration between couple instant
* Duration in days/hours/minutes/seconds/milliseconds/nanoseconds

```java
public class Main {
    public static void main(String[] args) {
        Duration fiveDays = Duration.ofDays(5);
        long seconds = Duration.between(Instant.parse("1986-09-25T00:00:00.000Z"), Instant.now()).getSeconds();
    }
}
```
