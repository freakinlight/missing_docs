### z_advanced_pub & z_advanced_sub

   Advanced pub/sub example using Zenoh's advanced publisher and subscriber APIs.
   These allow for reliable publication and detection of sample losses via caching, heartbeats, and detection mechanisms.

   Typical Subscriber usage:

   ```bash
   z_advanced_sub -k demo/example/**
   ```

   Typical Publisher usage:

   ```bash
   z_advanced_pub -k demo/example/test -v 'Hello World'
   ```

### z_get_shm

   Queries a shared-memory-based queryable resource and receives responses directly via shared memory,
   allowing for zero-copy high-performance communication.

   Typical usage:

   ```bash
   z_get_shm -s 'demo/**'
   ```

### z_ping_shm

   Performs a roundtrip time measurement between a shared-memory publisher and subscriber,
   leveraging shared memory for ultra-low-latency communication.

   Typical usage:

   ```bash
   z_ping_shm 1024
   ```

### z_queryable_shm

   Declares a shared-memory queryable resource that responds to queries with payloads using the shared memory feature,
   ideal for high-performance data access.

   Typical usage:

   ```bash
   z_queryable_shm -k demo/example/queryable -v 'This is the SHM result'
   ```

### z_sub_shm

   Declares a shared-memory subscriber that listens for publications sent via shared memory.
   This allows fast, zero-copy notification of new values published on a key expression.

   Typical usage:

   ```bash
   z_sub_shm -k demo/example/**
   ```
