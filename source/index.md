---
title: Qora Manual


toc_footers:
  - <a href='http://github.com/tripit/slate'>Documentation Powered by Slate</a>


search: true
---

# Introduction


# About Qora


## Features

## Source Code


## External Resources


# Getting Started

- [Download the client](#downloads)
- Create a Wallet
- Learn the application
- Get some Qora

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

## Retrieve wallet's seed

# Accounts

## Create account

## Delete account

## Import account from seed

## Retrieve account's seed

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

# View Asset details

# Add to Favorites

# Open Pair

## Buy asset

## Sell asset

## Place a buy order

## Cancel a buy order

## Place a sell order

## Cancel a sell order

## Issue asset

## Transfer asset

## Send multi payment

# Arbitrary Transactions

The data of the arbitrary transaction must be base58 encoded and must be between 1-4000 bytes.

<aside class="notice">
Currently arbitrary transactions can only be made through the API.
</aside>

To create an arbitrary transaction, open the console and then send your Command.

Below you will see an example command.

> POST arbitrarytransacions {"creator": "QNbA69dbnmwqJHLQeS9v63hSLZXXGkmtC6","data":"4GFHMAo9fmbUq7usopgntwUfAiLtpL98K6QCosAJsqQmY95tfd5KoUaKu34v6Qwp7RtYEhobCx7LVi7aYbbtpzfA","service": 555,"fee": "1.00001"}


Returns the transaction in JSON when successful.

If you have encountered an error while making the arbitrary transaction, console will display the error code.
Below is the errors list.

### ERRORS

| Error |	Description |
|------ | ----------- |
| 1 |	Json error. |
| 2 |	Not enough balance. |
| 3 |	Not yet released. |
| 102 |	Invalid address. |
| 105 |	Invalid fee. |
| 115 |	Invalid data. |
| 116 |	Invalid data length. |
| 201 |	Wallet does not exist. |
| 202 |	Address does not exist in wallet. |
| 203 |	Wallet is locked. |

# Automated Transactions

## Deploy AT

To deploy an AT (smart contract) go to the AT tab and click Deploy AT.

Enter the values accordingly on each field and click deploy.

# Atomic Cross-Chain Transfers

## Initiate ACCT

## Response ACCT

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

  - On Launch Configuration field select ```Start - Qora```from the drop down menu.
    You will have to [run the wallet first](#start-the-wallet-from-the-eclipse's-workspace) in order to have the option ```Start  - Qora``` available
  - / Select Export destination
  - / Select Package required libraries into generated JAR

![Export](https://i.imgur.com/BXvovZj.png "Export")  

You have now compiled the Qora.jar file directly from source code.

## Submit a pull request

You can submit a pull request to the source code by following the below steps.

# Help

## How To

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


## FAQ

Here are some frequently asked questions that might help you

## Known Issues

Below are listed the latest know bugs


## Report a bug

Found a bug? You can report it to the official Github of Qora!
