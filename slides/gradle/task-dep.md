## Task dependency

A task can depend on another task

```groovy
task both(dependsOn: hello) << {
    println 'Jocelyn'
}
```

