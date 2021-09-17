# Fundamentals

---
## Working w/ Private & Public Keys

**Public Key Cryptography**
    Public Key Cryptography can create an asymetric power imbalance
        - TLDR: difficul to access an individual private key due to the power of cryptography

    PKC allows blockchains to prove peer-to-peer transactions & establish identitites from the private key
        - mathematically proves a person holds a certain key


**Consequences**
1. there is no way to determine who actually holds the key
    - private key does not equal = owner of the assets
2. training users to self-manage private keys w/out support


**Keys & the sections of public key cryptography**
1. General public keys
2. Blockchain/ETH specific public keys
3. Advanved public keys

General Public Keys Resources
    - [KEYPAIR-ETH.BUILD](https://www.youtube.com/watch?v=9LtBDy67Tho)
    - [WIKIPEDIA-PKC](https://en.wikipedia.org/wiki/Public-key_cryptography)
    - [E2EE](https://www.youtube.com/watch?v=jkV1KEJGKRA)
    - [RSA-ENCRYPTION](https://www.youtube.com/watch?v=vgTtHV04xRI)
    - [What Is Asymmetric Encryption?](https://dzone.com/articles/what-is-asymmetric-encryption-understand-with-simp-1)
    - [Keeping Secrets](https://www.rigb.org/christmaslectures08/html/activities/keeping-secrets-secret.pdf#page=5)
    - [Secret Key Exchange](https://www.youtube.com/watch?v=NmM9HA2MQGI)
    - [Elliptic Curves](https://www.youtube.com/watch?v=NF1pwjL9-DE)

Blockchain & Etheruem Specific Resources
*How cryptography is used with Blockchains & Ethereum*
    - how pricate keys are used to generate ETH accounts: 
    - all ETH accounts start with the prefix `0x`: coded in hexadecimal format
        - [Book Excerpt: Keys and Addresses (Mastering Ethereum](https://github.com/ethereumbook/ethereumbook/blob/develop/04keys-addresses.asciidoc)
        - [How are ethereum addresses generated?](https://ethereum.stackexchange.com/questions/3542/how-are-ethereum-addresses-generated)

Advanced Public Key Resources
    - [the cryptopals crypto challenges](https://cryptopals.com/)

    

Next Sections: Chatper 1.4

# Hashing
**Cryptographic Hash Functions**: provides 3 critical componenets of building decentralized protocols.
1. Unqiueness
2. Avalanche Effect
3. Speed

[Cryptographic Hash Function Sandbox](https://emn178.github.io/online-tools/sha256.html)

The abovve 3 components combines to estlabish decentralized file integrity.