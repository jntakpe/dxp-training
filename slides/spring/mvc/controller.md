## Controllers

Can display views (HTML pages) or just expose API

* Annotation based @Controller (supports views and APIs) or @RestController (only for APIs)
* Mapping done by @RequestMapping annotation

```java
@RestController
@RequestMapping("/api/tpps")
public class TPPResource {
    private final TPPService tppService;

    public TPPResource(TPPService tppService) {
        this.tppService = tppService;
    }

    @GetMapping("/{name}")
    public TppApiDTO findByName(@PathVariable String name) {
        return tppService.findByName(name).get();
    }
}
```
