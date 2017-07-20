## Partial date and time

```java
public class Main {
    public static void main(String[] args) {
        LocalDate.of(2014, Month.MARCH, 18);
        LocalTime.of(12, 0); // same that LocalTime.NOON
        DayOfWeek.of(2);// DayOfWeek.TUESDAY
        Month.of(3); // same that Month.MARCH
        MonthDay.of(Month.MARCH, 18);
        YearMonth.of(2014, Month.MARCH);
        Year.of(2014);
    }
}
```
