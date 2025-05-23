---
title: Setup Testnet Wallets
description: How to create and fund testnet wallets to use for developing Celo dApps.
---

# Testnet Wallets

How to create and fund testnet wallets to use for developing Celo dApps. Make sure to never use the same wallet for development, where you hold your real-life funds.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

## Getting Started

While developing and deploying dApps on Celo, it’s helpful to have a wallet prepared with funds to pay for any transactions you make on the blockchain. These can be set up using either real or test funds, and this allows application developers and users to interact with Celo applications more easily.

:::tip

This guide will focus on funding an account on MetaMask with Celo ([Alfajores testnet](/network) tokens). You can also use the [Celo Extension Wallet](/wallet/) if you prefer. Additionally, you can fund your wallet with real Celo if you would like to deploy to the Celo Mainnet.

:::

## Download a Wallet

When deploying a dApp, you will need to pay for transactions that write data to the Celo blockchain. This is done using a wallet funded with Celo on your preferred network.

- Download [MetaMask](https://metamask.io/) for your browser
- If using MetaMask, [Connect MetaMask to Celo](/wallet/metamask/use) ([video](https://www.youtube.com/watch?v=JLHeCb01fzs)) to access Celo network options from your wallet

## Create your Account

You are now able to fund an account that you can access using your browser extension wallet. You can do this using accounts you create with the wallet or from the [Celo CLI](/cli/).

### Using a wallet

MetaMask allows you to easily create and manage accounts. This provides you with a quick way to create and fund an account to use when interacting with your dApp.

- From your MetaMask extension, select **Celo (Alfajores Tesnet)**

<!-- ![select alfajores network in MM](/img/doc-images/testnet-wallet/image1.png) -->

- Choose wallet **Settings**, select **Create Account**, name your account, and select **Create**

<!-- ![select create account MM](/img/doc-images/testnet-wallet/image2.png) -->

- View your account details and copy your account address from the top center of the user interface

<!-- ![new account MM](/img/doc-images/testnet-wallet/image3.png) -->

:::tip

Skip to [this step](#fund-your-account) to fund your account.

:::


### Using Celo CLI

Install `celocli` by running

```bash
npm install -g @celo/celocli
```

#### Create an Account

```bash
celocli account:new
```

Creating an account will return its account details as shown below (details will be specific to your account).

```shell
mnemonic: turtle cash neutral drift brisk young swallow raw payment drill mail wear penalty vibrant entire adjust near chapter mistake size angry planet slam demand
accountAddress: 0x5986ac413fA0C4A0379A674Cb986A59a962FC84e
privateKey: 8cab22c2bb08f0d20bd9e1109a156e87219d63a2c0b40b027483decf194bd787
publicKey: 024baaae61bab2a6e16ccb008c78dddb7132fc48d082e2a6166f8cc52d8d7a5289
address: 0x5986ac413fA0C4A0379A674Cb986A59a962FC84e
```

:::tip

Skip to [this step](#import-account-to-wallet-for-options-2--3) to connect your account to your wallet.

:::

## Import Account to Wallet (for Options 2 & 3)

If you created an account using option 2 or 3, you can now import these accounts to your wallet.

- Open your wallet browser extension from your browser
- Select **Settings** > **Import Account**
- Copy the **private key** from your local account, paste it into the window provided, and select **Import**

<!-- ![import account to metamask](/img/doc-images/testnet-wallet/image5.png) -->

## Fund your Account

No matter where you created your accounts, you can send them testnet funds using your **Account Address** and the testnet faucet.

- Navigate to the [Alfajores Testnet Faucet](https://faucet.celo.org)
- Copy your address from your terminal or wallet
- Paste this address into the **Testnet Faucet**, complete the **Captcha**, and click **Get Started**

![alfajores faucet](/img/doc-images/testnet-wallet/image6.png)

Wait for the transaction to process to view the funds in your account.
