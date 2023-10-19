# Moralis Token API

With [Moralis' Token API](https://moralis.io/api/token/), you can get information on specific tokens such as metadata, balances, etc. Access token metadata, cross-chain capabilities, and streamline smart contract event tracking, all while enjoying many use cases like live price feeds, portfolio management, transaction monitoring, and ownership verification.

In this article, you will explore the Moralis Token API and how it can help you while developing dapps.

## Quick Start to Wallet API

1. [Get an API key](https://docs.moralis.io/web3-data-api/evm/get-your-api-key)
2. Explore the [documentation guides](https://docs.moralis.io/web3-data-api/evm/token-api)
3. Explore the [full list of endpoints](https://docs.moralis.io/web3-data-api/evm/reference)

## Advanced Spam Detection

Security is paramount in the world of cryptocurrencies. Moralis Token API enhances your project's security by supporting advanced spam detection. Flag suspicious tokens or known scam tokens with confidence, protecting your users from potential threats.

Our cutting-edge spam detection feature is a game-changer for ERC20 tokens. Designed to fortify your tokens journey, this feature introduces a `possible_spam` field that promptly identifies potential spam, phishing, or suspicious contracts.

But that's not all - you can actively participate in enhancing ERC20 security. Head over to our comprehensive tutorial on reporting ERC20 spam at [https://docs.moralis.io/web3-data-api/evm/report-erc20-spam](https://docs.moralis.io/web3-data-api/evm/report-erc20-spam).

This functionality is available on all Ethereum Virtual Machines (EVMs), but our initial classification specifically covers contracts on the Ethereum mainnet, Polygon mainnet, and Binance mainnet.

To identify which endpoints support spam detection, you can refer to the next section.

Select what you want to achieve:

- [Get Tokens](#get-tokens)
- [Get Price](#get-price)
- [Get Balance](#get-balance)
- [Get Transfers](#get-transfers)
- [Get Pairs & Liquidity](#get-pairs--liquidity)
- [Get Token Stats](#get-token-stats)

### Get Tokens

Discover a world of tokens and their details with Moralis.

| No. | Method                                   | Description                                 | API Reference                                                                                                                     | URL                                                                       | Spam Detection |
|-----|------------------------------------------|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|----------------|
| 1   | `getWalletTokenBalances`                 | Get ERC20 token balance by wallet           | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-wallet-token-balances) | [https://deep-index.moralis.io/api/v2.2/:address/erc20](https://deep-index.moralis.io/api/v2.2/:address/erc20)                     | ✅             |
| 2   | `getTokenMetadataBySymbol`              | Get ERC20 token metadata by symbols         | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-metadata-by-symbol) | [https://deep-index.moralis.io/api/v2.2/erc20/metadata/symbols](https://deep-index.moralis.io/api/v2.2/erc20/metadata/symbols)                   | ✅  |
| 3   | `getTokenMetadata`                       | Get ERC20 token metadata by contract        | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-metadata) | [https://deep-index.moralis.io/api/v2.2/erc20/metadata](https://deep-index.moralis.io/api/v2.2/erc20/metadata) | ✅ |

### Get Price

Stay updated with real-time token prices using Moralis.

| No. | Method                                   | Description                | API Reference                                                                                                       | URL                                                                       | Spam Detection |
|-----|------------------------------------------|----------------------------|---------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|----------------|
| 4   | `getTokenPrice`                          | Get ERC20 token price      | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-price) | [https://deep-index.moralis.io/api/v2.2/erc20/:address/price](https://deep-index.moralis.io/api/v2.2/erc20/:address/price)                     |
| 5   | `getMultipleTokenPrices`                 | Get prices for multiple tokens  | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-multiple-token-prices) | [https://deep-index.moralis.io/api/v2.2/erc20/prices](https://deep-index.moralis.io/api/v2.2/erc20/prices)                   |

### Get Balance

Check token balances effortlessly.

| No. | Method                                   | Description                                 | API Reference                                                                                                                      | URL                                                                       | Spam Detection |
|-----|------------------------------------------|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|----------------|
| 6   | `getWalletTokenBalances`                 | Get ERC20 token balance by wallet           | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-wallet-token-balances) | [https://deep-index.moralis.io/api/v2.2/:address/erc20](https://deep-index.moralis.io/api/v2.2/:address/erc20)                     | ✅             |
| 7   | `getTokenAllowance`                      | Get ERC20 token allowance                   | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-allowance) | [https://deep-index.moralis.io/api/v2.2/erc20/:address/allowance](https://deep-index.moralis.io/api/v2.2/erc20/:address/allowance)                   |

### Get Transfers

Track token transfers with ease.

| No. | Method                                   | Description                                 | API Reference                                                                                                                     | URL                                                                       | Spam Detection |
|-----|------------------------------------------|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|----------------|
| 8   | `getWalletTokenTransfers`                | Get ERC20 token transfers by wallet         | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-wallet-token-transfers) | [https://deep-index.moralis.io/api/v2.2/:address/erc20/transfers](https://deep-index.moralis.io/api/v2.2/:address/erc20/transfers)                     | ✅             |
| 9   | `getTokenTransfers`                      | Get ERC20 token transfers by contract       | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-transfers) | [https://deep-index.moralis.io/api/v2.2/erc20/:address/transfers](https://deep-index.moralis.io/api/v2.2/erc20/:address/transfers)                   | ✅             |

### Get Pairs & Liquidity

Explore token pairs and liquidity data.

| No. | Method                                   | Description                                | API Reference                                                                                                     | URL                                                                       |
|-----|------------------------------------------|--------------------------------------------|-------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|
| 10  | `getPairReserves`                        | Get DEX token pair reserves                | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-pair-reserves) | [https://deep-index.moralis.io/api/v2.2/:pair_address/reserves](https://deep-index.moralis.io/api/v2.2/:pair_address/reserves)                     |
| 11  | `getPairAddress`                         | Get DEX token pair address                 | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-pair-address) | [https://deep-index.moralis.io/api/v2.2/:token0_address/:token1_address/pairAddres](https://deep-index.moralis.io/api/v2.2/:token0_address/:token1_address/pairAddres)                   |

### Get Token Stats

Access essential token statistics.

| No. | Method             | Description            | API Reference                                                                                                 | URL                                                                       |
|-----|--------------------|------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|
| 12  | `getTokenStats`    | Get ERC20 token stats  | [Method Documentation](https://docs.moralis.io/web3-data-api/evm/reference/get-token-stats) | [https://deep-index.moralis.io/api/v2.2/erc20/:address/stats](https://deep-index.moralis.io/api/v2)

## Rich Metadata

Access comprehensive ERC20 token metadata effortlessly. Retrieve essential details such as token names, symbols, logos, and more.

## Cross-Chain Functionality

Moralis Token API is not bound by a single blockchain. Enjoy the freedom of cross-chain functionality, seamlessly fetching ERC20 tokens across over 10 EVM chains. Covering testnets and mainnets, our API ensures that you have access to tokens wherever you need them.

## Smart Contract Events

Track and monitor smart contract events with ease. Keep an eye on token swaps, mints, burns, approvals, allowances, and trades. Moralis Token API simplifies event tracking, helping you stay informed and responsive.

## Versatility for Your Use Cases

The Moralis Token API is incredibly flexible, accommodating a wide range of use cases. Here are just a few examples:

### Live Price Feeds

Integrate real-time token price feeds into your dApp, ensuring your users have access to the latest market data. Build crypto wallets, portfolio trackers, or trading platforms with ease.

### Portfolio Apps

Create comprehensive portfolio apps that allow users to manage their crypto holdings efficiently. Display token balances, track transactions, and provide valuable insights.

### Transaction Monitoring

Monitor token transfers and contract events in real time. Receive instant notifications when specific events occur, enabling timely responses and user engagement.

### Ownership Verification

Implement ownership verification features in your dApp. Allow users to verify their token holdings and track their assets across chains.

## EVM Chains Supported

The Moralis Toke API is your go-to solution, providing support across all major EVM chains, including Ethereum, Binance Smart Chain, Polygon, and more.

Moralis Token API seamlessly integrates with top decentralized exchanges like Uniswap v2, Uniswap v3, SushiSwap, PancakeSwap, and many others. Whether you're tracking token liquidity or active pairs, our API provides you with the most up-to-date information. Stay ahead of the game by knowing where the action is.

## ⭐️ Star us

If this Token API helps you - please star this project, every star makes us very happy!

## 🤝 Need help?

If you need help with using the Token API or have other questions - don't hesitate to write in our community forum and we will check asap. [Forum link](https://forum.moralis.io/). We are answering questions 24/7
