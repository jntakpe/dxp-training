## Stream

**It's an interface**

```java
public interface Stream<T> extends BaseStream<T, Stream<T>> {
}
```

Efficiently process amounts of data :
* by leveraging parallel computing (fork/join)
* by avoiding unnecessary intermediary computation 

