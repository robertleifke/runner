# Runner 🏃

An arbitrageur for Numo Engine to keep the discount factors in check with real world forex markets.

## Build

First, make sure the following are installed: 
1. [Anvil](https://github.com/foundry-rs/foundry/tree/master/crates/anvil#installing-from-source)

In order to build, first clone the github repo: 

```sh
git clone https://github.com/paradigmxyz/artemis
cd artemis
```

Next, run tests with cargo: 

```sh
cargo test --all
```

In order to run the opensea sudoswap arbitrage strategy, you can run the following command: 

```sh
cargo run -- --wss <INFURA_OR_ALCHEMY_KEY> --opensea-api-key <OPENSEA_API_KEY> --private-key <PRIVATE_KEY> --arb-contract-address <ARB_CONTRACT_ADDRESS> --bid-percentage <BID_PERCENTAGE>
```

where `ARB_CONTRACT_ADDRESS` is the address to which you deploy the [arb contract](/crates/strategies/opensea-sudo-arb/contracts/src/SudoOpenseaArb.sol).
