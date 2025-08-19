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

### sha256

Compute the SHA-256 hash of the given input string.
Return the hash as a hexadecimal string.

