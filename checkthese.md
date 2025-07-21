#C

### z_pub

Demonstrates how to create a basic Zenoh publisher in C that periodically sends data on a specified key expression.

Typical usage:

```bash
z_pub
```

or

```bash
z_pub -k demo/example/zenoh-c-pub -p "Pub from C!" -a "optional-attachment"
```


#Java

### QueueHandler

Demonstrates how to implement a custom Zenoh handler using a queue to receive and store incoming data samples.
Used internally in other examples as a handler to collect `ZenohType` elements into a queue.

### z_info

Retrieves and displays session-related information such as the local `zid`, connected routers, and peers using the Zenoh Java API.

Typical usage:

```bash
java -jar ZInfo.jar
```

or

```bash
java -jar ZInfo.jar -c config.json -e tcp/127.0.0.1:7447 -l tcp/0.0.0.0:7447 --mode peer
```


#Rust

### z_ping_shm

Measures roundtrip latency using Zenoh's shared-memory transport in Rust.  
It publishes a payload on a `ping` key and waits for a `pong` reply to compute latency statistics.

Typical usage:

```bash
z_ping_shm 1024
```

or

```bash
z_ping_shm 2048 -n 200 --warmup 2.5
```
