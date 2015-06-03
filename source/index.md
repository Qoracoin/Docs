---
title: Qora Wiki


toc_footers:
  - <a href='http://github.com/tripit/slate'>Documentation Powered by Slate</a>


search: true
---

# Introduction

Qora is a second generation peer to peer cryptocurrency aims to solve Bitcoin's biggest problems.

# About Qora

Qora has been reilied on an IPO

## Getting Started

- [Download the client](#downloads)
- Create a Wallet
- Learn the application
- Get some Qora

## Features

- Ed25519 DSA to verify and sign messages.
- 1-5 minute block time depending on the network activity.
- Retargeting every 10 blocks.
- Deterministic and Password protected wallets that can be recovered/generated from seeds.
- New Proof-of-Stake algorithm.
- A REST API to directly communicate with the client.
- Naming Service: allows the user to register a key-value pair which can be used for various purposes (URLS, addresses, …).
- This Naming Service will also include an exchange where users can buy and sell keys.
- Voting System: Allows voting inside the client to make community decisions such as which feature will be implemented next.
- Arbitrary Transactions: a simple feature which allows users to send any payload they want over the network.
- This can be used by third-parties to build additional features on top of Qora (chat, ...).
- Assets: assets with asset/asset trading pairs.

## Source Code

Source code has been first published on 09 of December, 2014 at version 18.Full source code has been published on Mar 14, 2015.

## External Resources

# How To

Here you can find a quick How-To list

- [How to install](#installation)
- [How to create a wallet](#create-a-wallet)
- [How to send payment](#send-payment)
- [How to send message](#send-message)
- [How to register a name](#register-a-name)
- [How to vote](#vote)
- [How to buy an asset](#buy-asset)
- [How to sell an asset](#sell-asset)
- [How to issue an asset](#issue-asset)
- [How to deploy an AT](#deploy-at)
- [How to make an Atomic Cross-Chain transfer](#atomic-cross-chain-transfers)

# Download

- Universal Wallet
- Windows Wallet
- MAC Wallet
- Linux Wallet
- ARM Wallet

## Universal Wallet

## Windows Wallet

## MAC Wallet

## Linux Wallet

## ARM Wallet

# Installation

- Universal Wallet
- Windows Wallet
- MAC Wallet
- Linux Wallet
- ARM Wallet

## Universal Wallet

## Windows Wallet

## MAC Wallet

## Linux Wallet

## ARM Wallet

# Settings

## Basic

## Known Peers

## Access Permission

# Wallet

## Start the application

## Create a Wallet

## Recover wallet from seed

## Create account

## Delete account

## Import account from seed

# Payments

## Send Payment

## Send Name Payment

## Send payment within a message

## Send multi payment

# Messages

## Send message

## Encrypt message

## Decrypt message

## Sign a message

## Verify message

# Naming service

## Register a name

## Update name

## Buy a name

## Sell Name

# Polls

## Vote

## Create a poll

# Assets

## Buy asset

## Sell asset

## Place a buy order

## Place a sell order

## Issue asset

## Transfer asset

## Send multi payment

# Arbitrary Transactions

# Automated Transactions

## Deploy AT

To deploy an AT (smart contract) go to the AT tab and click Deploy AT.

Enter the values accordingly on each field and click deploy.

# Atomic Cross-Chain Transfers

## Initiate ACCT

## Response ACCT

# Services

## Exchanges

# Tools

Here you can find a list of tools

## Block Explorer

Official block explorer of Qora has been created by agran and you can find all the details you might need.

## Blogging Service

Official blogging service of Qora has been created by agran and you can find it here :
This service uses the arbitrary transactions feature of Qora to serve socialized blogging suite.

## Faucet

## HTML Editor

## Multiple Pages Generator

# Developers

## API

Qora uses a REST API to communicate with the wallet.
You can find the entire API documentation here : [http://api.qora.org](http://api.qora.org)

## Import source code to eclipse

You can import the source code to a workspace in Eclipse by following the below steps.

- [Download Eclipse](https://www.eclipse.org/downloads/)

- Create / Select a workspace

![Create / Select a workspace](https://i.imgur.com/cd8JxZb.png "Create / Select a workspace")

- File / Import

![File / Import](https://i.imgur.com/Yucm94S.png "File / Import")

- / Git / Projects from Git

![/ Git / Projects from Git ](https://i.imgur.com/NJd9b4x.png "/ Git / Projects from Git ")

- / Clone URI

![/ Clone URI](https://i.imgur.com/2LJBSe2.png "Clone URI")

- / Enter Github Repo

![/ Enter Github Repo](https://i.imgur.com/7CLLk1A.png "/ Enter Github Repo")

- / Select Master Branch

![/ Select Master Branch](https://i.imgur.com/ixSurJo.png "/ Select Master Branch")

- / Select Destination

![/ Select Destination](https://i.imgur.com/2Kp7NiC.png "/ Select Destination")

- / Import Existing Projects

![/ Import Existing Projects]( https://i.imgur.com/KC3LcJL.png "/ Import Existing Projects")

- Click on ```Finish```

![/ Finish](https://i.imgur.com/BRmXqYz.png "/ Finish")

## Start the wallet from the Eclipse's workspace

When you have successfully imported Qora to your Eclipse's Workspace you then can start the wallet by following the below steps:

- Select the ```>Qora [Qora master]``` from Package Explorer, click on Run on menu bar and then Run again.

![Run](https://i.imgur.com/j38tm5s.png "Run")

- Run as Java Application

![Run as Java Application](https://i.imgur.com/4Sb9CDZ.png "Run as Java Application")

- On the next step scroll down and click on the Start - (default package) and click OK

![Start](https://i.imgur.com/jUh89lu.png "Start")

<aside class="success">
You have launched the wallet directly from source
</aside>
## Compile Qora from source code

- Select the ```>Qora [Qora master]``` from Package Explorer

![Master](http://i.imgur.com/H8tK1rZ.jpg "Master")

- Go to ```/ File / Export / Java / Runnable JAR file```

![Export](https://i.imgur.com/sIadzQn.png "Export")

- Export

  - On Launch Configuration field select ```Start - Qora```vfrom the drop down menu.
    You will have to [run the wallet first](#start-the-wallet-from-the-eclipse's-workspace) in order to have the option ```Start  - Qora``` available
  - / Select Export destination
  - / Select Package required libraries into generated JAR

![Export](https://i.imgur.com/BXvovZj.png "Export")  

You have now compiled the Qora.jar file directly from source code.

## Submit a pull request


# Qora team

## Team

# Find Help

## FAQ

## Known Issues

## Report a bug
