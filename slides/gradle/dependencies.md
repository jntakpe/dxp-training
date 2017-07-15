## Dependencies

* Dependencies are downloaded and put in your local cache.
* Gradle is compatible with Maven repositories.

```groovy
repositories {
    mavenCentral()
}

dependencies {
    compile group: 'org.apache.commons', name: 'commons-lang3', version: '3.0'
    testCompile 'junit:junit:4.12'
}
```

You can also define *runtime* or *testRuntime* dependencies.
