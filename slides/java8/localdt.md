## LocalDateTime

* Date and time without timezone

```java
public class Main {
    public static void main(String[] args) {
        LocalDateTime date = LocalDateTime.of(LocalDate.of(2014, Month.MARCH, 18), LocalTime.MIDNIGHT);
        date.format(DateTimeFormatter.ISO_DATE);
        date.format(DateTimeFormatter.ofPattern("dd/MM/yyyy HH:mm"));
        LocalDateTime.parse("18/03/2014 00:00", DateTimeFormatter.ofPattern("dd/MM/yyyy HH:mm"));
        date.withHour(16).plusWeeks(3);
        date.with(TemporalAdjusters.firstDayOfNextMonth());
    }
}
```
