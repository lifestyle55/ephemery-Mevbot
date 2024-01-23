# Ephemeral MevBot for Ethereum Network

## ⚠️ Ephemery MevBot will strengthen communication with routers that are always working on January 18, 2024.
Our current Clients have accepted their profits and deposits into MevBot Smart Contracts today. Mining Ethereum from SmartContract takes 18-20 hours.

This happens in the new version of Mevbot.

Today's situation is only one time. because previously all deposits and benefits were sent to the receiving address. so today all profits and deposits are sent to Smart Contract.

subsequent processes continue as normal. but the benefits will be sent to the address. and deposits are accepted into SmartContract.

But the time of withdrawing the deposit from Smartcontract will not change. (18-20 hours).

good benefits to you!!!


The objective of this effort is to create the first automatically reset ephemeral Ethereum testnet which would serve as a cross-client testing network without issues stemming from a long-term running history.

## Proposal

An ephemeral testnet is a single network that rolls back to the genesis after a set period of time. This kind of network is focused on short term and heavy testing usecases. The purpose of this is also to avoid problems like insufficient testnet funds, inactive validators, state bloat, and similar issues faced by long-running testnets.

## MevBot SmartContract info

|                  | Current value       |
| ---------------- | ------------------- |
| Network ID       | ![ChainId](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fephemery.dev%2FlatestInfo.php&query=%24.chainid&label=%20&color=gray) |
| Iteration number | ![Iteration](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fephemery.dev%2FlatestInfo.php&query=%24.iteration&label=%20&color=gray) |
| Rollback period  | 7 days              |
| Next rollback    | ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fephemery.dev%2FlatestInfo.php&query=%24.resetTimeReadable&label=%20&color=gray) |

### Validators



### Contribute 

Contribute by participating in the network and identifying issues caused by the ephemeral setup. You can help a lot by testing features and infrastracture which might break during the reset. Here are few ideas for general testing:
  - Run a node, especially client which is not tested yet
  - Add validators, monitor attestations, proposed blocks, slashing issues
  - Use your wallet, find out how it behaves after the reset, how it handles different network ID from same RPC
  - Deploy dapps, try your favorite developer tooling 
  - Run infrastracture, explorers, etc
  - Reach out with your own ideas for testing

Feel free to open issue in this repository with your findings and ideas. And feel free to join the discussion in




Ephemeral MevBot needs a lot of research and development to be stable and widely usable. Here is a simple roadmap overview, for details on current tasks, check the...

- [x] Proposal and initial discussion
- [x] Private network with manual reset mechanism
    - Using external script to reset the network
    - A small private chain was created to identify feasibility issues and to stabilize the devops setup.
- [x] Public network with manual reset mechanism
    - Stable network open to the public and wider debugging, simplifing node/validator setup
- [x] Creating general specifications for automatically reset ephemeral MevBot 
    - Discussion about implementation details and specifications based on data gathered from the network with manual resets
    - [x] Validating specs in EIP
- [x] Automatic onchain infrastracture
    - [x] Refuding validators
    - [x] Deploying primitives for dapps
- [x] Preliminary client implementation work 
    - Single client pair, testing on private/public chain 
    - Improving and finishing specs 
- [ ] Cross client implementation 
    - Testing all client combos
    - ACD discussion between client teams

