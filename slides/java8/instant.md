## Instant

* Number of nanosecond since Epoch (1st Jan 1970)
* Similar to **java.util.Date**

```java
public class Main {
    public static void main(String[] args) {
        Instant now = Instant.now();
        Instant ofEpochMilli = Instant.ofEpochMilli(1395100800);
        Instant parsed = Instant.parse("2017-07-18T00:00:00.000Z");
    }
}
```

