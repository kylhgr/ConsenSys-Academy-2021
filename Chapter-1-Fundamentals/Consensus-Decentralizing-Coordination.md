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
    - depends on the fault tolerance of a system
        - mathmatical verification of messages
        - can tolerate 1/3 dishonest or absent participation
        - functioning network with 1:4 faulty nodes = PBFT 
    - ensure a minimum number of nodes reaches consensus before appending to the shared ledger
        - once an agreement is verified, the ledger is updated
    2. Proof of Work --> Secure State Machine Replication
        - currently used by Bitcoin and Etheruem to maintain consensus
    3. Proof of Stake --> Secure Stata Machine Replication
        - Etheruem is moving from Proof of Work to Proof of Stake

Each mechanism includes rules to determine what is a valid block

---
### Additional Materials

- how do we agree on things that have happened in the past?
- how do actors in a network we coordinate and agree on a series of events that have lead to the current state of the network?
- how do we know someone really does have digital money they can send, and not making it up
- how do all the actors in the network then maintain that knowledge in a secure way?

#### Development of Distributed Computing

**Distributed Computing**

Origin: 1970s, airplans moved to electron control systems, manufactuers wanted to make sure that if a certain part of the electronics gave out while the plane is airborne, the whole plane wouldnt shut down.
    - early works: non-adversarial systems: any faults that happened in a computer network, where the result of a natural system error, not hacking or active attacks

consensus protocols are used to allow computers to work together, and let different servers agree on the state of a system!, *good consensus protocols would continue to function with some errors*
    - the ability of a consensus protocol to adapt to failure = resillience

consensus protocols help systems maintain historical information = state
    - state: set of variables describing a certain system at a specific time, when the variables are together they paint a picture of the architecture.

