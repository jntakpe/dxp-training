## Functional interfaces

The type of a lambda is a functional interface.

A functional interface is an interface with one abstract method like :

```java
public class Main {
    public interface Runnable {
        void run();
    }

    public interface Comparator<T>{
        int compare(T t1, T t2);
    }

    public interface FileFilter {
        boolean accept(File pathname);
    }
}

```
