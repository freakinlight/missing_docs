### z_delete

Deletes a value associated with a key expression in Zenoh.

Typical usage:

```bash
z_delete
```

or

```bash
z_delete -k demo/example/delete
```

### z_formats

Explores how Zenoh formats key expressions using different formatting options.

Typical usage:

```bash
z_formats
```

or

```bash
z_formats -k demo/example/formats -v '{"x":1,"y":2}'
```

### z_forward

Shows how to use Zenoh's forwarding capability to redirect traffic through a forwarder node.

Typical usage:

```bash
z_forward
```

or

```bash
z_forward -e tcp/forwarder_address:7447
```

### z_get_shm

Sends a query and receives a shared-memory reply.

Typical usage:

```bash
z_get_shm
```

or

```bash
z_get_shm -s demo/example/queryable
```

### z_posix_shm_provider

Demonstrates how to provide SHM buffers using the POSIX SHM API.

Typical usage:

```bash
z_posix_shm_provider
```

or

```bash
z_posix_shm_provider -k shm/path
```

### z_put_float

Publishes a float value to a Zenoh key expression.

Typical usage:

```bash
z_put_float
```

or

```bash
z_put_float -k demo/example/float -p 3.1415
```

### z_queryable_shm

Declares a queryable that uses shared-memory transport when replying, ideal for local high-speed data retrieval.

Typical usage:

```bash
z_queryable_shm
```

or

```bash
z_queryable_shm -k demo/example/queryable -p 'Result via shm'
```

### z_sub_shm

Subscribes to key expressions and receives data using shared-memory transport.

Typical usage:

```bash
z_sub_shm
```

or

```bash
z_sub_shm -k demo/example/**
```


