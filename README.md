## blake2sum

Compute BLAKE2(b|s) checksum

```txt
Usage: blake2sum [OPTIONS] [FILE [FILE …]]

positional arguments:
  FILE                  file to calculate digest for

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show version information and exit
  -c, --copyright       show copying policy and exit
  -a ALGO, --algo ALGO  hash algorithm (blake2b is default): [blake2b|blake2s]
  -l LENGTH, --length LENGTH
                        digest length in bits
  -t, --tag             create a BSD-style checksum

With no FILE, or when FILE is -, read standard input.

blake2b is optimized for 64-bit platforms and NEON-enabled ARMs,
        produces digests of any size between 1 and 64 bytes.

blake2s is optimized for 8 to 32-bit platforms, produces digests
        of any size between 1 and 32 bytes.

Digest length must not exceed the maximum for the selected algorithm
and must be a multiple of 8.
```

Tested with Python 3.6.
