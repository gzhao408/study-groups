# P2P

*Note that this section depends on reviewing the network propagation resources of the mining and network propagation study group. If you are doing these out of order, please take a look at that section first.*

## Reading

| Content                                                                                       | Time  | Tags                    |
|-----------------------------------------------------------------------------------------------|-------|-------------------------|
[Attack the p2p layer of Bitcoin Core with Amiti Uttarwar (until min 41)](https://youtu.be/H-wH6mY9pZo?t=257) | 35 min | p2p attacks |
[Bitcoin Peer-to-Peer Network with John Newbery](https://youtu.be/eVerdR2hOMw) | 51 min | P2P, video |
[The Bitcoin Network (start at network discovery section)](https://github.com/bitcoinbook/bitcoinbook/blob/f8b883dcd4e3d1b9adf40fed59b7e898fbd9241f/ch08.asciidoc#network-discovery) | 15 min | P2P |
[Network partition resistance](https://gist.github.com/sdaftuar/c2a3320c751efb078a7c1fd834036cb0) | 15 min | P2P |
[Deanonymization in the Bitcoin P2P Network](https://papers.nips.cc/paper/6735-deanonymization-in-the-bitcoin-p2p-network.pdf) | 15 min | P2P, privacy |
[Eclipse Attacks on Bitcoin’s Peer-to-Peer Network](https://eprint.iacr.org/2015/263.pdf) | 60 min | eclipse Attacks, P2P |
[Network partitioning & network level privacy attacks](https://youtu.be/StnOVBbIpD8) | 60 min | eclipse Attacks, privacy, P2P, video |
[Dandelion: Redesigning the Bitcoin Network for Anonymity](https://arxiv.org/pdf/1701.04439.pdf) | 20 min | P2P, privacy |
[Researching P2P privacy attacks](https://youtu.be/qKNEUfnYue0) | 90 min | P2P, privacy, video |


## Discussion Questions

### P2P Connections
1. What is reasoning behind the max inbound and max outbound defaults? For which type of user would they be considered ideal and when might they be optimized?
1. What is the rationale behind the "new"/"tried" table design? Were there any prior inspirations within the field of distributed computing?
1. How does a fixed set of 4 outbound peers get chosen? In what circumstances would you evict/change them?
1. What are feeler connections and when are they used?
1. How are the default values affect the throughput of the whole network? Has anyone ever tried to analyze how much data the bitcoin P2P network can handle both in bandwidth and latency?

### De-anonymization
1. How does "diffusion" message spreading work and why is it ineffective against de-anonymization?

### Dandelion
1. How are routes chosen (in the stem phase)? What happens if a malicious (or faulty) node doesn't propagate your transaction in the stem phase?
1. When a transaction is going to bloom depends on a weighted coin toss at each hop- how is that weight determined? Could an adversarial node overwrite that weight to ensure bloom?
1. Dandelion++ is meant to address the assumptions from the original Dandelion paper. How is that achieved?
  - Assumptions:
    a) All nodes obey the protocol
    b) Each node generates precisely one transaction
    c) All Bitcoin nodes run Dandelion
