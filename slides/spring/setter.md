## Setter injection

```java
@Service
public class ConsentService {
    private static final Logger LOGGER = LoggerFactory.getLogger(ConsentService.class);

    private ConsentRepository consentRepository;

    public Single<Consent> create(Consent consent) {
        LOGGER.info("Creating consent {}", consent);
        return Single.just(consentRepository.insert(consent))
                .doOnSuccess(c -> LOGGER.info("Consent {} successfully created", c));
    }

    @Autowired
    public void setConsentRepository(ConsentRepository consentRepository) {
        this.consentRepository = consentRepository;
    }
}
```
