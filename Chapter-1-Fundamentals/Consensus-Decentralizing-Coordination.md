# What are Consensus Mechanisms ?

**The Goal of Concensys Mechanisms**: Facilitate the agreement process among participants of a distributed data system to guarantee data consistency.
    - Coming into consensus around the state of data --> *everyone must have the same ledger and agree on its validity* 
    - Designed to incentivize honest participation in the network
Consensus Mechanism is the economic mechanism that is implemented to achieve the goal of data consistency!

*"The Consensus Algorithm allows secure updates of a state according to specific state transition rules, where the right to perform the state transition is distributed among some economic set"* - Vitalk 

## Implementing Consensus Mechanisms
**Different Approaches**
    1. PBFT: practical byzantine fault tolerance
        - high performance, state machine replication algorithm: allows distributed computing systems to reach consensus 
    2. Proof of Work --> Secure State Machine Replication
        - currently used by Bitcoin and Etheruem to maintain consensus
    3. Proof of Stake --> Secure Stata Machine Replication
        - Etheruem is moving from Proof of Work to Proof of Stake
