### ZQuerier

Continuously sends query messages for a selector.  
The queryables with a matching path or selector (for instance [ZQueryable](#zqueryable))  
will receive these queries and reply with paths/values that will be printed by the querier.

Usage:

```bash
java -jar ZQuerier.jar
```

or

```bash
java -jar ZQuerier.jar -s demo/example/query
```

### ZBytesExamples

Demonstrates how to use `ZBytes` for serialization and deserialization of custom data types,  
as well as how to send them over Zenoh and receive them on the subscriber side.

Usage:

```bash
java -jar ZBytesExamples.jar
```

or

```bash
java -jar ZBytesExamples.jar -k demo/example/zbytes
```
