## Wrapper

Run Gradle without Gradle installed. It downloads Gradle as shell or bash script.

```groovy
task wrapper(type: Wrapper) {
    gradleVersion = '1.11'
}
```

To initialize run :

```./gradlew build```
