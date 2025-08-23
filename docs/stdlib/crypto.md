# crypto

*Source: `crypto.scar`*

## Imports

- `std/strings`
- `std/random`

## Functions

### xor_cipher

`xor_cipher(string text, string key) -> string`

Return the raw string result of XOR between text and key characters.

### xor_cipher_hex

`xor_cipher_hex(string text, string key) -> char*`

Apply XOR cipher to a given text using the provided key.
Return the result as a hexadecimal string.

### random_salt

`random_salt(i32 length) -> string`

Generate a random salt of the specified length.
Return the generated salt as a string.

### aes128_encrypt

`aes128_encrypt(string plaintext, string key) -> string`

Encrypt data using AES-128 in ECB mode.

Takes plaintext and a 16-byte (128-bit) key.

Returns encrypted data as hexadecimal string.

### aes128_decrypt

`aes128_decrypt(string ciphertext_hex, string key) -> string`

Decrypt data using AES-128 in ECB mode.

Takes hexadecimal encrypted data and a 16-byte (128-bit) key.

Returns decrypted plaintext as a string.

### chacha20_encrypt

`chacha20_encrypt(string plaintext, string key, string nonce) -> string`

Encrypt data using ChaCha20 stream cipher.

Takes plaintext, a 32-byte (256-bit) key, and a 12-byte (96-bit) nonce.

Returns encrypted data as hexadecimal string.

### chacha20_decrypt

`chacha20_decrypt(string ciphertext_hex, string key, string nonce) -> string`

Decrypt data using ChaCha20 stream cipher.

Takes hexadecimal encrypted data, a 32-byte (256-bit) key, and a 12-byte (96-bit) nonce.

Returns decrypted plaintext as a string.

