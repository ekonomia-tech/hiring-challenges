# Smart Contract Challenge
## Setup a project and create a contract
### Summary
ETHPool provides a service where people can deposit ETH and they will receive rewards proportional to their deposits in the pool. Users must be able to take out their deposits along with their portion of rewards at any time. New rewards are deposited manually into the pool by the ETHPool team using a contract function.

### Requirements
- Only the team can deposit rewards.
- The team can deposit rewards at any time.
- Deposited rewards go to the pool of users, not to individual users.
- Users should be able to withdraw their deposits along with their share of rewards considering the time when they deposited. They should not get rewards for the ones distributed before their deposits.

Example:

> Let say we have user **A** and **B** and team **T**.
>
> **A** deposits 100, and **B** deposits 300 for a total of 400 in the pool. Now **A** has 25% of the pool and **B** has 75%. When **T** deposits 200 rewards, **A** should be able to withdraw 150 and **B** 450.
>
> What if the following happens? **A** deposits then **T** deposits then **B** deposits then **A** withdraws and finally **B** withdraws.
> **A** should get their deposit + all the rewards.
> **B** should only get their deposit because rewards were sent to the pool before they participated.

### Goal
Design and code a contract for ETHPool, take all the assumptions you need to move forward. Bonus points for thinking about the most gas-efficient implementation you can.

You can use any development tools you prefer: Hardhat, Foundry, Truffle, Brownie, Solidity, Vyper, etc.

Useful resources:
- Solidity Docs: https://docs.soliditylang.org/en/v0.8.4
- Educational Resource: https://github.com/austintgriffith/scaffold-eth
- Project Starter: https://github.com/abarmat/solidity-starter (not necessary but recommended to use to help setup your repo so that you can just code the solidity)

## Deploy your contract
Deploy the contract to any Ethereum testnet of your preference. Keep record of the deployed address.

Bonus:
- Verify the contract in Etherscan

# Front End Challenge
Write a simple front end application to support the ETHPool contract. The application should:
- Allow the user to connect their wallet
- Deposit ETH into the pool
- Reflect the user’s current deposit in the pool
- Reflect the user’s current state of rewards
- Allow the user to claim his deposit + rewards
- You can deploy the front end to a website like AWS or heroku and provide the link in the submission. Or you can provide instructions to deploy to localhost so we can pull it down locally and test the code ourselves. Your choice.

Stack:
- Framework - React\Preact
- Any other library you need - ethers.js, web3,js, etc.cd
- Try and keep the bundle size as small as possible
- Feel free to design the page(s) and components as you please, we leave the design open on purpose. It is okay to make it very simple, or to make it beautiful, it is up to you based on home much time you have.

# Submission

You can work on a private GitHub repo and then share it with dave@ekonomia.tech