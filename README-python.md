### z_advanced_pub

Publishes data using the Advanced Publisher feature of Zenoh, which adds reliability mechanisms like sample caching, miss detection, and publisher discovery.

Typical usage:

```bash
   python3 z_advanced_pub.py
```

or

```bash
   python3 z_advanced_pub.py -k demo/example/zenoh-python-pub -p 'Hello World' --history 10
```

### z_advanced_sub

Subscribes using the Advanced Subscriber feature of Zenoh. Supports late publisher detection, recovery, and detection of missed samples.

Typical usage:

```bash
   python3 z_advanced_sub.py
```

or

```bash
   python3 z_advanced_sub.py -k demo/example/**
```

### z_bytes

Demonstrates how to handle raw bytes, strings, JSON, protobuf, and Python objects using `ZBytes` and `z_serialize`/`z_deserialize`.

Typical usage:

```bash
   python3 z_bytes.py
```

### z_delete

Deletes resources in Zenoh matching the given key expression.

Typical usage:

```bash
   python3 z_delete.py
```

or

```bash
   python3 z_delete.py -k demo/example/zenoh-python-put
```

### z_get_liveliness

Queries all currently alive liveliness tokens that match a given key expression.

Typical usage:

```bash
   python3 z_get_liveliness.py
```

or

```bash
   python3 z_get_liveliness.py -k group1/** -o 5.0
```

### z_liveliness

Declares a liveliness token on a given key. The token stays alive while the process is running.

Typical usage:

```bash
   python3 z_liveliness.py
```

or

```bash
   python3 z_liveliness.py -k group1/zenoh-py
```

### z_ping

Measures round-trip latency between ping and pong using Zenoh pub/sub. Sends data and waits for response.

Typical usage:

```bash
   python3 z_ping.py 1024
```

Optional:

```bash
   python3 z_ping.py --warmup 1.0 --samples 100 1024
```

### z_pong

Receives data from z_ping and replies back, completing the round-trip latency loop.

Typical usage:

```bash
   python3 z_pong.py
```

or

```bash
   python3 z_pong.py --express True
```

### z_pull

Implements a pull-based subscriber using a ring buffer to retrieve recent samples.

Typical usage:

```bash
   python3 z_pull.py
```

or

```bash
   python3 z_pull.py -k demo/example/** --size 5 --interval 2
```

### z_put_float

Publishes a floating-point number using Zenoh's typed serialization.

Typical usage:

```bash
   python3 z_put_float.py
```

or

```bash
   python3 z_put_float.py -k demo/example/zenoh-python-put -p 3.1415
```

### z_sub_liveliness

Subscribes to changes in liveliness tokens (alive or dropped) over a given key expression.

Typical usage:

```bash
   python3 z_sub_liveliness.py
```

or

```bash
   python3 z_sub_liveliness.py -k group1/** --history True
```

### z_sub_queued

Receives samples with a queued subscriber and prints notifications for each message.

Typical usage:

```bash
   python3 z_sub_queued.py
```

or

```bash
   python3 z_sub_queued.py -k demo/example/**
```
