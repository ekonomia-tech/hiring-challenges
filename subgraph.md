# Subgraph Coding Challenge
## Challenge 1
### Summary
Write an AAVE V2 subgraph from scratch for the AAVE V2 deployment on the Ethereum Network.
#### Requirements
- [Use data source templates](https://thegraph.com/docs/en/developer/create-subgraph-hosted/#data-source-templates-for-dynamically-created-contracts) to load all the AAVE markets/reserves into the Subgraph.
- Create a market entity in your schema. Fill in the following information:
  - The total underlying tokens deposited for each market/reserve.
  - The total aTokens in existance for each market/reserve.
  - The current variable deposit rate for each markets/reserve.
  - The current variable borrow rate for each markets/reserve.
  - Any other fields you think are relevant.
- Feel free to add in any other entities you need.
- [Use `startBlock` in the manifest](https://thegraph.com/docs/en/developer/create-subgraph-hosted/#start-blocks).
- Deploy the subgraph to [The Graph Hosted Service](https://thegraph.com/hosted-service/).
## Challenge 2
### Summary
In the same repository, write a simple script in order to directly query the subgraph for the `aDAI` markets total tokens, and `console.log()` the result.

#### Requirements
- Querying the subgraph you deployed.
- Use any of the following packages to write the script:
  - Hardhat, ethers.js, etc. (javascript)
  - Brownie, Web3.py, etc (python)
  - Foundry (built in rust, high performance)

## Goals of the challenges
- Challenge 1
  - Test ability to read smart contracts and turn it into actionable data with a subgraph.
- Challenge 2
  - Test writing a graphql query.
  - Test simple script writing.
## Hints
- The address of AAVE-V2s `LendingPoolAddressesProviderRegistry` is `0x52D306e36E3B6B02c153d0266ff0f85d18BCD413`. This is the main contract address for an entry point for the manifest. It is the only contract address you will need to use. All others will be added through the data source templates.
- Feel free to borrow code you find online. But make sure you understand it. In the interview, you should state what you borrowed and why you chose it.

## Useful resources:
- The Graph Docs: https://thegraph.com/docs/quick-start
- Ask the graph discord for help - https://discord.com/invite/vtvv7FP
- Solidity Docs: https://docs.soliditylang.org/en/v0.8.4
- AssemblyScript Docs (Subgraph mapping handlers are written in AS): https://www.assemblyscript.org/introduction.html
- Educational Resource: https://github.com/austintgriffith/scaffold-eth


## Submission
You can work on a private GitHub repo and then share it with **davekaj** GitHub user. Feel free to send any question while doing the exercise.