### z_advanced_pub

Publishes data using the **Advanced Publisher** API with support for reliability features such as history and heartbeat-based sample miss detection.

Typical usage:

   ```bash
   z_advanced_pub
   ```

or

   ```bash
   z_advanced_pub -k demo/example/advanced -p 'Hello World' --history 5
   ```

### z_advanced_sub

Subscribes using the **Advanced Subscriber** API with features like late publisher detection and sample recovery, and detects any missed samples via heartbeat tracking.

Typical usage:

   ```bash
   z_advanced_sub
   ```

or

   ```bash
   z_advanced_sub -k demo/example/**
   ```

### z_delete

Deletes resources from Zenoh that match the specified key expression.

Typical usage:

   ```bash
   z_delete
   ```

or

   ```bash
   z_delete -k demo/example/delete-me
   ```

### z_get_shm

Performs a Zenoh `get` query using **shared-memory transport**, when available, for high-throughput local communication.

Typical usage:

   ```bash
   z_get_shm
   ```

or

   ```bash
   z_get_shm -s demo/example/**
   ```

### z_non_blocking_get

Issues a Zenoh `get` query in a **non-blocking** way using a polling mechanism on the response channel.

Typical usage:

   ```bash
   z_non_blocking_get
   ```

or

   ```bash
   z_non_blocking_get -s demo/example/**
   ```

### z_ping_shm

Measures **roundtrip latency** using Zenoh's **shared-memory transport**. Sends a `put` on one key and expects an echo on another.

Typical usage:

   ```bash
   z_ping_shm 1024
   ```

### z_queryable_shm

Declares a **queryable** that uses **shared-memory** transport when replying, ideal for local high-speed data retrieval.

Typical usage:

   ```bash
   z_queryable_shm
   ```

or

   ```bash
   z_queryable_shm -k demo/example/queryable -p 'Result via shm'
   ```

### z_queryable_with_channels

Declares a **queryable** that responds using **Zenoh channels**, supporting multiple simultaneous replies over the same query.

Typical usage:

   ```bash
   z_queryable_with_channels
   ```

or

   ```bash
   z_queryable_with_channels -k demo/example/channel-queryable -p 'Streaming reply'
   ```
