# Secret Network Grant Delivery Report

### `Milestone 1` — Smart Contract Development

| Length | Deliverable | Specification |
|-|-|-|
| 1 month | Smart Contracts | 0. We have researched the Secret Network [standards](https://scrt.network/about/secret-nfts) and other factors & [protocols](https://docs.scrt.network/dev/privacy-model-of-secret-contracts.html) that distinguish it from other chains<br/>We have developed the smart contracts that can:<br/>1. [Handle SC requests](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L574-L595)<br/>2. [Freeze](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L348-L405)/[Unfreeze](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L224-L244) single `Native` NFTs and [Freeze](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L406-L473)/[Unfreeze](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L245-L280) in batches<br/>3. [Mint](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L281-L306)/[Burn](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L474-L517) single and [Mint](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L307-L347)/[Burn](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L518-L572) in batches `wrapped` NFTs<br/>4. [Withdraw](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L199-L218) the TX fees on the target chain in native tokens|

### `Milestone 2` — Smart Contract Development

| Length | Deliverable | Specification |
|-|-|-|
| 0.5 month | Smart Contracts | We have developed the smart contracts that can:<br>5. [Trust/verify](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L53-L127) the multisig of the bridge oracle validators<br/>6. [Whitelist](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L219-L223) NFT smart contracts<br/>7. [Pause/Unpause](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L184-L189) for maintenance or if compromised<br/>8. [Reset the Frost Group Key](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/contract.rs#L190-L198) the bridge validators their expenses|

### `Milestone 3` — Testing & Documenting

| Length | Deliverable | Specification |
|-|-|-|
| 0.5 month | Tests & Documentation | 1. [Inline documentation of the code](https://github.com/XP-NETWORK/secret-bridge/commit/2ff8f610a8b905796a5d8fc626e26dd322b4de76)<br/>2. [SC Functional tests](https://github.com/XP-NETWORK/secret-bridge/blob/master/src/tests.rs)<br/>3. [Basic tutorial](https://github.com/XP-NETWORK/testing-secret_network) that can [interact](https://secretnodes.com/secret/chains/pulsar-2/contracts/secret146snljq0kjsva7qrx4am54nv3fhfaet7srx4n2) with the deployed [smart contracts](https://github.com/XP-NETWORK/xpjs/blob/secretjs/src/factory/factories.ts#L267-L280) and backend service.<br/>4. [Testing the contracts in the testnet environment](https://github.com/XP-NETWORK/testing-secret_network#minting-an-nft-on-secret)|

## TODO ================================================== >

### `Milestone 4` — Integrating into the Live Bridge
| Length | Deliverable | Specification |
|-|-|-|
| 1 month | Validators, Backend, Frontend | 1. Developing validation logic relevant for the Secret Network part of the bridge<br/>2. Adding Secret Network to the Bridge NFT-Indexer<br/>3. Integrating TX fee estimation<br/>4. Plugging Secret Network in the heartbeat<br/>5. Integrating with a Secret Network rpc node<br/>6. Integrating Secret Network in the bridge UI<br/>7. Deploying smart contracts<br/>8. Adding Secret Network to the bridge JS library<br/>9. Adding access to Secret Network from the REST API<br/>10. Adding Secret Network to the bridge widget|