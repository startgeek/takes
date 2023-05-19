**NEAR**

# Generic Characteristics

## consensus:
 A regular POS based on 2/3 + 1 with some extra new concepts:

 large pool of participants (we call them “witnesses”) to be elected to make decisions during a specific interval of time (we default to one day). Each interval is split into a large number of block slots (we default to 1440 slots, one every minute) with a reasonably large number of witnesses per each block (default to 1024). With these defaults, we end up needing to fill 1,474,560 individual witness seats.

 Each witness seat is defined by the stake of all participants that indicated they want to be signing blocks. For example, if 1,474,560 participants stake 10 tokens each, then each individual seat is worth 10 tokens and each participant will have one seat. Alternatively, if 10 participants stake 1,474,560 tokens each, individual seat still cost 10 tokens and each participant is awarded with 147,456 seats. Formally, if X is the seat price and {Wi} are stakes by each individual participant

Validators validate all shards.
Chunk-Only Producers are solely responsible for producing chunks (parts of the block from a shard, see Nightshade for more detail) in one shard (a partition on the network)

## sharding:

just imagine sharding as multiple parallel blockchains now near uses Async sharding there are methods to make sure each shard doesnt include bad block 

1.neighbor shard gossip (neighbors check their neighbor shards)
2.fisherman: there is a time period that an honest actor can submit A challenge to bad block
3.cryptographically proof of a shard is correct like zk-SNARKs, zk-STARKs but these are slow and expensive. and SNARKS can be build on turing compatible VM's


### how to write smart contracts while keeping sharding satisfied:



nonces are associated with access keys