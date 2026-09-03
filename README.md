# California Data Broker Registry, September 2026 snapshot

A clean CSV export of the [California Data Broker Registry](https://cppa.ca.gov/data_broker_registry/), pulled from the California Privacy Protection Agency (CPPA) on 2026-09-01. Published so that researchers, journalists and privacy tools can work from the same file without re-scraping the state site.

Maintained by [Delist My Data](https://delistmydata.com), a Seattle data removal service that publishes [free opt-out guides](https://delistmydata.com/opt-out-guides) for the people-search sites in this registry.

## What is in the file

`ca_data_broker_registry_2026-09-01.csv`: one row per registered data broker, 77 columns, exactly as disclosed by each broker under California's Delete Act (SB 362) registration requirements. Field names are the registry's own labels, kept verbatim so they can be matched against the CPPA site.

Column groups:

| Columns | What they hold |
|---|---|
| 1–10 | Identity: broker name, DBA, primary website, contact email, phone, street address, city, state, zip, country |
| 11 | URL of the broker's own page describing how Californians exercise CCPA rights |
| 12–22 | Yes/no self-disclosures of what is collected: minors' data, account logins, government ID numbers, citizenship or immigration status, union membership, sexual orientation, gender identity, biometrics, precise geolocation, reproductive health data |
| 23–27 | Yes/no self-disclosures of who data was shared with or sold to in the past year: a foreign actor, the federal government, other state governments, law enforcement (outside subpoena or court order), a developer of a generative AI system |
| 28–47 | Whether the broker or a subsidiary is regulated by FCRA, GLBA, California IIPPA, CMIA, or HIPAA, and for each: the personal information, products and share of activity covered |
| 48–77 | 2024 consumer-request metrics, in five families (delete, know what is collected, know what is sold or shared, opt out of sale or sharing, limit sensitive PI): requests received, complied in whole, complied in part, denied, mean and median days to respond |
| 77 | Free-text comments |

## Headline counts from this snapshot

| Registered data brokers | 603 |
| collect personal information of minors | 18 |
| collect consumers' precise geolocation | 115 |
| shared or sold data to a foreign actor in the past year | 26 |
| shared or sold data to the federal government in the past year | 55 |
| shared or sold data to law enforcement (outside subpoena/court order) | 28 |
| shared or sold data to a GenAI developer in the past year | 32 |
| regulated (in part) by the FCRA | 17 |

Top states (US rows): CA 126, NY 84, FL 48, TX 32, IL 32, MA 29, VA 23, GA 21

Countries: UNITED STATES 564, UNITED KINGDOM 12, CANADA 10, GERMANY 3, SINGAPORE 2, ISRAEL 2

Counts are of brokers that answered "Yes" to the relevant disclosure. Blank and "No" are both counted as not-yes. State names were normalised (for example "California" and "CA") for the state tally only; the CSV itself is untouched.

## Caveats

- These are the brokers' own declarations. The CPPA does not verify them at registration.
- Registration is required of brokers meeting California's definition of a data broker, regardless of where they are based. Being absent from the registry is not evidence a company is not a data broker.
- Many people-search brands are separate storefronts of the same operator. The registry lists the registrant, not every consumer-facing brand.
- A snapshot. The registry changes as brokers register, amend, or are removed. Check the date in the filename.

## Licence

The data is a public record published by the State of California. This README and any scripts in this repository are released under CC0 1.0; do what you like with them, attribution appreciated but not required.
