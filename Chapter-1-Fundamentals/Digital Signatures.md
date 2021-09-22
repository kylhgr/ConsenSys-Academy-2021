# Digital Signatures

blockchain uses private keys as a decentralized form of identity

hashing is used as a decentralized form of file

Digital signature use aa combination of key signing and hashing to create a decentralized intent

---
a signature is made when a hash of the message is signed by the private key of the account holder, the encryption process is also apart of the hashing process.

signed transaction can be thought of as a "hash of a hash"
*the digital signature will look like a normal hash, but it can only be decrypted by the origins owners public key to confirm identity*

the digital signature acts as a protective casing around transaction daata

---
### Layers of Digital Signature

1. the unsigned hash is formed by making a cryptographic hash of the `Sender`, `Receiver`, `Amount`, `hash` data and signing each field.

by creating 2 successive hashes, a seried of protective wrapping are created
- first is the message that has valid digital signatures on it provides 3 different confirmations
    1. origin: if a private key digital signature is valid, then the signed message did come from the account associated with the public key
    2. message integrity: the message has not been tampered with by anyone else due to matching hashes/public key de-cryption.
    3. intent: signing the first hash, the owner of the private key is signalling their intent to execute the commands or agreements that are contained in the message

**Capturing Intent**: the power of digital signatures
- bits of code when signed and validaated can be executed automatically by the blockchain protocol


the decentralizaiton of intent is the last piece of cryptographic primitibes, capturing intent is important and it relies on two primitves (public key cryptography and hash functions).

digital signatured are emergent in this way


##### Additional resources
- https://medium.com/mycrypto/the-magic-of-digital-signatures-on-ethereum-98fe184dc9c7
