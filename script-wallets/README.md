# Scripts and Wallets

## Reading

| Content                                                              | Time  | Tags                    |
|----------------------------------------------------------------------|-------|-------------------------|
[Bitcoin Script: Past and Future - until 1:08](https://youtu.be/H-wH6mY9pZo?t=2549) | 25 min | script, video |
[Script: A mini programming language](https://learnmeabitcoin.com/technical/script) | 10 min | script |
[Scripts with John Newbery](https://youtu.be/np-SCwkqVy4) | 30 min | script, video |
[Miniscript: Streamlined Bitcoin Scripting](https://medium.com/blockstream/miniscript-bitcoin-scripting-3aeff3853620) | 11 min | miniscript |
[Taproot and Policy with James Chiang](https://youtu.be/EdRm_mnoCWc) | 26 min | script, video, _optional_ |
[HD Wallets](https://learnmeabitcoin.com/technical/hd-wallets) | 10 min | HD wallets |
[Native Descriptor Wallets](https://gist.github.com/achow101/94d889715afd49181f8efdca1f9faa25) | 10 min | descriptors |
[Coin Selection](https://youtu.be/ZMzVIi1lgyw) | 20 min | coin selection |
[An introduction to Bitcoin Core fee estimation](https://bitcointechtalk.com/an-introduction-to-bitcoin-core-fee-estimation-27920880ad0) | 11 min | fees |
[Fee Bumping and RBF](https://github.com/bitcoinops/scaling-book/blob/add_rbf/1.fee_bumping/fee_bumping.md) | 20 min | fee bumping, RBF |
[PSBT with Andrew Chow - until Q&A](https://youtu.be/H6xZSRDXUiU) | 20 min | PSBT, video _optional_ |
[Wallet Development in Bitcoin Core](https://youtu.be/j0V8elTzYAA) | 35 min | wallets, video, _optional_ |

## Discussion Questions

### SCRIPT
1. John Newbery talks about [verification vs. computation](https://youtu.be/np-SCwkqVy4?t=934), and he bring it up as a big reason why he thinks bitcoin can scale but is skeptical about ethereum. Is there a qualitative difference between verification and computation? And is it the fact that ethereum is capable of performing arbitrary computation that makes the whole thing difficult to scale, or is it that specifically smart contracts that require arbitrary computation won’t be able to scale (as in those contracts would be very expensive to run)?

### Output Descriptors
1. Are there any use cases for p2sh-wsh-p2pkh descriptors?
1. What's about miniscript? Interactions with descriptors?

### HD Wallets
1. What is the difference between child and hardened child addresses?
1. Why is the internal chain not visible outside of the wallet if it uses public derivation?

### Coin Selection
1. Is coin age ever a consideration for coin selection?
1. Coin selection can expose a wallet by observing how the wallet selects its inputs, are there any efforts to standardize coin selection into a library of sorts so there's a standard?
