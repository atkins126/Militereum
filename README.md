# ![image](icon_150x150.png) Militereum&nbsp;&nbsp;[![GitHub release](https://img.shields.io/github/release/svanas/Militereum)](https://github.com/svanas/Militereum/releases/latest) [![macOS](https://img.shields.io/badge/os-macOS-green)](https://github.com/svanas/Militereum/releases/latest/download/macOS.zip) [![Windows](https://img.shields.io/badge/os-Windows-green)](https://apps.microsoft.com/store/detail/militereum/9MVF9Z4SWKDR)

* simulates your transactions, and
* shows you exactly what tokens are about to exit your wallet BEFORE a transaction leaves your device, and
* blocks suspicious transactions, and
* works with every EVM-compatible wallet, including browser-based (eg. [MetaMask](https://metamask.io/), [Trust](https://trustwallet.com/)) and native desktop (eg. [Frame](https://frame.sh/), [Zerion](https://link.zerion.io/a11o6IN0jqb)) wallets, and
* non-custodial, 100% uptime. you do not depend on our infrastructure because there isn't any, and
* supports Ethereum and many other chains, including [Polygon](https://polygon.technology/) and [Arbitrum](https://arbitrum.io/) and [Optimism](https://optimism.io/), and
* available for [Windows](https://apps.microsoft.com/store/detail/militereum/9MVF9Z4SWKDR) and [macOS](https://github.com/svanas/Militereum/releases/latest/download/macOS.zip), and
* auditable open source code

## Setup

1. Download Militereum for [Windows](https://apps.microsoft.com/store/detail/militereum/9MVF9Z4SWKDR) or [macOS](https://github.com/svanas/Militereum/releases/latest/download/macOS.zip)
2. Launch Militereum. The following window appears. Click on `Copy`

![image](assets/main.png)

3. Unlock MetaMask in your web browser
4. Navigate to _Settings_ > _Networks_ > _Add a network manually_
5. The following tab appears. Paste Militereum's network URL in `New RPC URL`. Click on `Save`

![image](assets/MetaMask.png)

Click [here](networks.md) for more info on how to configure Militereum.

## Running

As soon as your wallet has connected to Militereum, the firewall gets minimized and keeps running in the background.

Every raw transaction passes through Militereum and if it is suspicious, Militereum will block the transaction and prevent it from leaving your device.

Here's an example. Navigate to [Uniswap](https://app.uniswap.org/) or [Balancer](https://app.balancer.fi/). Initiate a swap from one of your tokens to another. Before Uniswap or Balancer can swap your token, you'll need to sign a so-called _token allowance_.

Every time you approve a token allowance, you are potentially exposing your wallet to an exploit. Uniswap and Balancer are very reputable, but any other dapp can potentially phish you for an allowance and drain your tokens from your wallet.

After your crypto wallet has approved the allowance, Militereum will intercept the transaction and prompt you with this window. From here, you can allow the transaction to happen, or prevent it from leaving your device.

![image](assets/approve.png)

Besides token allowances, Militereum will block...
1. monetary transfers above $5k [➹](assets/limit.png), and
2. transactions to a sanctioned address [➹](assets/sanctioned.png), and
3. transactions to a smart contract that has not been [etherscan](https://etherscan.io/)-verified [➹](assets/unverified.png), and
4. transactions to an address you have not transacted with before [➹](assets/firsttime.png), and
5. transactions to a smart contract that lies about its own token supply [➹](assets/spam.png), and
6. transfers of honeypot tokens that are designed to pump but you cannot sell [➹](assets/honeypot.png), and
7. deposits to a [metamorphic smart contract](https://0age.medium.com/the-promise-and-the-peril-of-metamorphic-contracts-9eb8b8413c5e) that could be updated to divert your money elsewhere.

Militereum's dialogs are provided for informational purposes only and should not be taken as financial advice. Remember to always do your own research before interacting with tokens.

## License

Distributed under the [GNU AGP v3.0](https://github.com/svanas/Militereum/blob/master/LICENSE) with [Commons Clause](https://commonsclause.com/) license.

## Sponsors

This project received a [WAGBI grant](https://www.alchemy.com/developer-grant-program) from alchemy.com and is featured in [Alchemy’s Dapp Store](https://www.alchemy.com/dapps/militereum).

<img style="width:240px;height:53px" src="https://static.alchemyapi.io/images/marketing/badgeLight.png"/>

## Disclaimer

Militereum is provided free of charge. There is no warranty. The authors do not assume any responsibility for bugs, vulnerabilities, or any other technical defects. Use at your own risk.
