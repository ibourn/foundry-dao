# Foundry DAO Governance

This is a section of the Cyfrin Foundry Solidity Course.

_[⭐️ (6:05:45) | Lesson 14 | DAOs & Governance](https://www.youtube.com/watch?v=wUjYK5gwNZs&t=21945s)_

This is a Solidity-based DAO implementation using OpenZeppelin.

Many tools and solutions exist to build a DAO (Tally, Snapshot, Aragon...).
While it's possible to build a DAO from scratch, leveraging well-known solutions like OpenZeppelin can offer several advantages:

- Security: Established solutions have been thoroughly tested and audited, reducing the risk of vulnerabilities.
- Community Support: Using popular tools means access to a wider community for help, resources, and collaboration.
- Time Efficiency: Building on top of existing frameworks can significantly reduce development time and effort.

In this repository, we delve into the creation of a Decentralized Autonomous Organization (DAO) by using OpenZeppelin's smart contract libraries. Through the implementation of a simple test using Foundry, we aim to demonstrate the seamless deployment and execution of a proposal, showcasing the practical application of decentralized governance principles.

_Please note: ERC20 based voting is not always recommended, we should explore other forms of governance like reputation based or "skin-in-the-game" based. [An article on money-based voting being bad](https://vitalik.ca/general/2018/03/28/plutocracy.html)._

- [Foundry DAO Governance](#foundry-dao-governance)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Quickstart](#quickstart)
- [Usage](#usage)
  - [Test](#test)
  - [Deploy](#deploy)
  - [Estimate gas](#estimate-gas)
- [Formatting](#formatting)
- [Thank you!](#thank-you)

# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [foundry](https://getfoundry.sh/)
  - You'll know you did it right if you can run `forge --version` and you see a response like `forge 0.2.0 (816e00b 2023-03-16T00:05:26.396218Z)`

## Quickstart

```
git clone https://github.com/ibourn/foundry-dao
cd foundry-dao
forge install
forge build
```

# Usage

## Test

```
forge test
```

## Deploy

No deployment script for this project, we focus on the implementation of contracts and we have just a test to demonstrate the end-to-end use of the DAO with the life cycle of a proposal from submission to execution.

## Estimate gas

You can estimate how much gas things cost by running:

```
forge snapshot
```

And you'll see and output file called `.gas-snapshot`

# Formatting

To run code formatting:

```
forge fmt
```
