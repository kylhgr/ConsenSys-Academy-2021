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

        considerations: payee needs to know the previous owner did not sign an earlier transaction, how do we accomplish this without a trusted party? --> transaction must be publically accessible & an agreed upon single source of truth for the history of transaction