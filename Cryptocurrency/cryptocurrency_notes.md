## What is Bitcoin

- 3 layers of technology
  1. Technology: like blockchain
  2. Protocol/Coin: a set of rules that guides how a set of users interact with eachother, Bitcoin, TCP/IP, HTTP
    - The Coin: a single coin that is attached to a protocol, it is an innate asset of the protocol which facilates interaction of users
      - Bitcoin: a set of rules on how participants in the bitcoin network will communicate with eachother, like coming to consensus, updates, etc.
      - Ethereum and Ripple are both other protocols
  3. Token: tokens rely on smart contracts and are built ontop of a protocol, typically associated with an idea that somebody is building
     1. ICO refers to a token offering, not a coin

  - What is Bitcoin all about?
    - removing an intermediary for when people transact
  - Who are in the bitcoin ecosystem
    - Nodes
    - Miners
    - Large Mins
    - Mining Pools

  - Bitcoins Monetary Policy
    - The halving: the number of bitcoins released into the system is every 4 years is halved. roughly every 210k blocks that are mined, the rewards to the miner is halved: 50, 25, 12.5. 6.25 ... etc.
      - Transaction fees will then replace the block rewards as mining rewards end in 2140
    - Block Frequency: how often do blocks get mined: every 10 minutes for bitcoin

- Understanding mining difficulty
  - for every leading zero that we add to the required hash, we reduce the number of allowed nonces decreases by 16
  - Assuming the winning hash has 18 leading zeros, the probability of 0.000000000000000000002%
  - How is Mining difficulty calculated?
    - Difficulty is adjusted every 2016 blocks
    - Difficulty = current target / max target
      - max target: the ultimate most challenging target
    - difficulty is decided by an algorithm that looks at the last 2 weeks based on the average hashing power deployed by miners
  - How do mining pools work?
    - multiple computers are working together in a pool to solve for the right nonce, the pool tells computers which nonces to search for so that there is no double work
  - what is Nonce Range?
    - must be between 0-4billion, a 32bit unsigned number
    - The timestamp keeps constantly updated, resetting the hash, so our 4bn difference nonces can be retried every second
    - It is possible to try all 4bn nonces with the timestamp and not have an answer, so as the timestamp moves forward we get more chances to solve the puzzle
  - How do miners pick transactions
    - a mempool is a list of all the transactions that are yet to be added to a block
    - the miner will typically choose transactions with th ehighest fees and add them into the block that he is going to mine
    - miners could all pick different transactions, which means that miners are searching for different nonces
    - If a miner goes through all 4bn nonces before the second timer comes up, then they could add or remove transactions to change what the output hash will look like, by changing the block configuration
    
