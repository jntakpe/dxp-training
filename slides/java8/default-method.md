## Default method

**We can put code in interfaces**

```java
public interface Iterable<T> {
    default void forEach(Consumer<? super T> action) {
        Objects.requireNonNull(action);
        for (T t : this) {
            action.accept(t);
        }
    }
}
```

* New java 8 concept
* Allows to change old interfaces without breaking existing implementations
* Works with static methods too
