## Timezones

```java
public class Main {
    public static void main(String[] args) {
        ZonedDateTime.ofInstant(Instant.now(), ZoneId.of("Europe/Paris"));
        OffsetDateTime.ofInstant(Instant.now(), ZoneId.of("GMT+1"));
        OffsetDateTime.ofInstant(Instant.now(), ZoneOffset.of("+01:00"));    }
}
```

* Similar to *GregorianCalendar*
