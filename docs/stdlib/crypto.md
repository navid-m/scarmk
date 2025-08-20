# crypto

*Source: `crypto.scar`*

## Imports

- `std/strings`
- `std/random`

## Functions

### xor_cipher

Apply XOR cipher to a given text using the provided key.
Return the raw string result of XOR between text and key characters.

### xor_cipher_hex

Apply XOR cipher to a given text using the provided key.
Return the result as a hexadecimal string.

### vigenere_encrypt

Encrypt a given text using the Vigenère cipher with the provided key.
Return the encrypted text as a string.

### vigenere_decrypt

Decrypt a given text using the Vigenère cipher with the provided key.
Return the decrypted text as a string.

### random_salt

Generate a random salt of the specified length.
Return the generated salt as a string.

### aes128_encrypt

Encrypt data using AES-128 in ECB mode.

Takes plaintext and a 16-byte (128-bit) key.

Returns encrypted data as hexadecimal string.

### aes128_decrypt

Decrypt data using AES-128 in ECB mode.

Takes hexadecimal encrypted data and a 16-byte (128-bit) key.

Returns decrypted plaintext as a string.

### chacha20_encrypt

Encrypt data using ChaCha20 stream cipher.

Takes plaintext, a 32-byte (256-bit) key, and a 12-byte (96-bit) nonce.

Returns encrypted data as hexadecimal string.

### chacha20_decrypt

Decrypt data using ChaCha20 stream cipher.

Takes hexadecimal encrypted data, a 32-byte (256-bit) key, and a 12-byte (96-bit) nonce.

Returns decrypted plaintext as a string.

