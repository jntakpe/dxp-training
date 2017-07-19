## First lambda

* Make anonymous classes easier to write
```java
public class Main {
    public static void main(String[] args) {
        FileFilter filter1 = new FileFilter() {
            @Override
            public boolean accept(File pathname) {
                return true;
            }
        };
        FileFilter filter2 = (File file) -> true;
        FileFilter filter3 = file -> true;
    }
}
```
