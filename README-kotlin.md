### ZAdvancedPublisher

Declares a publisher using the advanced Pub/Sub API, which adds reliability mechanisms on top of the basic pub/sub.

Usage:

```bash
java -jar ZAdvancedPublisher.jar
```

or

```bash
java -jar ZAdvancedPublisher.jar -k demo/example/advanced-pub -v "Advanced Pub from Kotlin"
```

---

### ZAdvancedSubscriber

Creates a subscriber using the advanced Pub/Sub API, which enables more control and reliability in message delivery.

Usage:

```bash
java -jar ZAdvancedSubscriber.jar
```

or

```bash
java -jar ZAdvancedSubscriber.jar -k demo/example/advanced-sub
```

---

### ZQuerier

Continuously sends queries for a selector.
The queryables with a matching path or selector (for instance [ZQueryable](#zqueryable))
will receive the queries and respond with paths/values, which will be handled by the querier.

Usage:

```bash
java -jar ZQuerier.jar
```

or

```bash
java -jar ZQuerier.jar -s demo/example/query
```

---

### ZBytes

Demonstrates how to work with raw binary data using Zenoh.
This example serializes and deserializes data using byte arrays to and from Zenoh.

Usage:

```bash
java -jar ZBytes.jar
```

or

```bash
java -jar ZBytes.jar -k demo/example/bytes -v "0xDEADBEEF"
```

---

### ZInfo

Displays information about the current Zenoh session and configuration.

Usage:

```bash
java -jar ZInfo.jar
```
