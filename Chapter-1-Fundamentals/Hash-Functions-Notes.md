# Hashing
**Cryptographic Hash Functions**: provides 3 critical componenets of building decentralized protocols.
1. Unqiueness
2. Avalanche Effect
3. Speed

[Cryptographic Hash Function Sandbox](https://emn178.github.io/online-tools/sha256.html)

The abovve 3 components combines to estlabish decentralized file integrity.

### Hashing in Blockchains

*refernce*: Bitcoin White Paper: The double spend problem

- The Problem: "*the payee cant verify that one of the owners did not double spend the coin*"
- Proposed Solutions
    1. trusted central authority aka "Mint": checks every transaction for double spending
        - "*after each transaction the coin must be returned to the mint to issue a new coin*"
        - "*only coins issued from the mint are trusted to not be double-spent*"
        
        fault in the proposed solution --> fate of entire ecosystem/monetary system depends on the organization/people operating the mint

- Considerations
    - payee needs to know the previous owner did not sign an earlier transaction, how do we accomplish this without a trusted party? --> transaction must be publically accessible & an agreed upon single source of truth for the history of transaction. *(a collection of nodes will agee & verify the first recieved transaction)
    
    - how do we know the transactions have not been manipulated, which record is true?

#### Satoshi on Hasing & how it helps solve double spending
**Using Hashing to create a "timestamp server"**

- What is a Timestamp Server?: takes a hash of a block of items to be time stampped and widely publishing the hash
    - the timestamp proves that the data existed at a specific time, in logical order .. each timestamp will include the previous time stamp in its hash, forming a chain with each additional time stamp reinforcing the previous stamp. 

- How does the Timestamp Server work?
    - leverages hash functions by including the hash of the previous block into the hash of the current block
        - historical data is any of the previous blocks are alters, the changes will cascade throughout all the blocks after it
        - blocks of transaction data are chained together to form a blockchain

Considerations:
    - the chaining can only be effective in a large system *(ref back to the 3 characteristics)*
        1. Uniqueness --> one string matches one hash
        2. Avalanche Effeect --> one change in an input string created effects on the output
        3. Speed --> hashes can be securly computed quickly at scale

### Hash Chains as General Data Structures
Hash chains has utility outside of the timestamp server

- Examples
    1. Git uses a hash chain called **Directed Acyclic Graph** to track changes of software versions over time
    2. Challenge-Response schemes are used for user validation, also use hash chains

Hash functions and hash chaining are foundational for power data structure and programming data primitives like hash table

##### Hashing Resources
1. https://emn178.github.io/online-tools/sha256.html
2. https://web.archive.org/web/20201026010255/https://privacycanada.net/cryptanalysis/why-is-2-256-secure/
3. https://www.youtube.com/watch?v=b4b8ktEV4Bg
4. https://www.youtube.com/watch?v=DMtFhACPnTY
5. https://www.metamorphosite.com/one-way-hash-encryption-sha1-data-software
6. https://simple.wikipedia.org/wiki/Cryptographic_hash_function


##### Blockchain Hashing Resources
1. https://youtu.be/QJ010l-pBpE
2. https://medium.com/@ConsenSys/blockchain-underpinnings-hashing-7f4746cbd66b
3. https://observablehq.com/@consensys-academy/cryptographic-hash-functions
4. https://www.khanacademy.org/economics-finance-domain/core-finance/money-and-banking/bitcoin/v/bitcoin-cryptographic-hash-function

##### Advanced Hashing Resources
1. https://github.com/cooganb/bitcoin-whitepaper-exercises/blob/master/hashing/README.md
2. https://github.com/cooganb/bitcoin-whitepaper-exercises