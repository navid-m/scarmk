# hash

*Source: `hash.scar`*

## Functions

### fnv1a

`fnv1a(string data) -> i32`

FNV-1a hash algorithm

### fnv1a_64

`fnv1a_64(ref string data) -> void`

FNV-1a hash with 64-bit output (returns as string to avoid overflow)

### djb2

`djb2(string data) -> i32`

DJB2 hash algorithm

### simple_hash

`simple_hash(string data) -> i32`

Basic polynomial rolling hash

### sdbm

`sdbm(string data) -> i32`

SDBM hash algorithm
Used in SDBM database and GNU AWK

### crc32

`crc32(string data) -> i32`

CRC32 hash implementation
Cyclic redundancy check with good error detection

### hash_int

`hash_int(i32 value) -> i32`

Hash function for integers

### combine_hash

`combine_hash(i32 hash1, i32 hash2) -> i32`

Combine two hash values

### murmur3

`murmur3(string data, i32 seed) -> i32`

Murmur3 hash (32-bit version)
High-quality non-cryptographic hash

### base64_encode

`base64_encode(string data) -> string`

Base64-encode a string and return the encoded text.

### base64_decode

`base64_decode(string b64) -> string`

Decode a Base64-encoded string and return the decoded text.

### sha256

`sha256(string input) -> string`

Compute the SHA-256 hash of the given input string.
Return the hash as a hexadecimal string.

