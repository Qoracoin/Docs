---
title: Qora Documentation


toc_footers:
  - <a href='http://github.com/tripit/slate'>Documentation Powered by Slate</a>


search: true
---

# About Qora

Qora is a community-based cryptocurrency network. The emphasis is on community services like blogs, websites, etc. based on blockchain technology.

## Source Code

Qora source code is hosted by [github](https://github.com/Qoracoin/Qora)

## External Resources

Take a look at the [Qora website](http://qora.org)

# Getting Started

- [Download and install the application](#installation)
- [Create a Wallet](#create-a-wallet)
- [Learn the application](#how-to)
- Get some Qora

# Installation

- [Windows Wallet](#windows-wallet)
- [Universal Wallet](#universal-wallet)

## Windows Wallet

1. Download the latest Windows installer from github: [![release](https://img.shields.io/github/release/Qoracoin/Qora.svg)](https://github.com/Qoracoin/Qora/releases)

2. Run the installer and follow the instructions.

3. If installation is successful then you should have a Qora desktop icon and entries in your Windows menu.

## Universal Wallet

1. Make sure you have at least Java v8 installed. [Check your Java version](https://www.java.com/en/download/installed.jsp) or [download Java](https://www.java.com/en/download/manual.jsp)

2. Download the latest Qora Zipfile from github: [![release](https://img.shields.io/github/release/Qoracoin/Qora.svg)](https://github.com/Qoracoin/Qora/releases)

3. Once the file is downloaded, unzip it and it will make a Qora folder. You can move the Qora folder to wherever you like i.e. desktop, home directory etc.

4. Inside the Qora folder there will be a **run.sh** file you can double-click. Make sure you have the right permissions set to execute the file, right click on **run.sh**, choose "Properties" from the menu, go to the "Permissions" tab, in the "Execute" field make sure it reads "Only owner and group" and apply changes if needed.

5. Alternatively you can open a command prompt or shell window, change directory to the Qora folder and type:

`./run.sh`

# Settings

## Basic

* GUI Enabled

Most users will leave this enabled so they can access their wallets. Only people running a headless, high-availability node might consider disabling the GUI.

* RPC Enabled
* RPC port

Enabling RPC allows your Qora client to process API calls via the specified port using HTTP. Some of the built-in web pages use API calls, e.g. block explorer, name storage, anything wallet-related. For these to work you need to have RPC enabled. To restrict API callers, take a look at [Access Permissions](#access-permission). 

* WEB Enabled
* WEB port

Enabling WEB allows you to access the Qora network/blockchain/features using your web browser, which might be easier and more feature-rich than the Qora client's GUI. To restrict access, take a look at [Access Permissions](#access-permission).

## Known Peers

This is a list of peer IP addresses known to your Qora client, along with a tick-box to show if you're connected to them. You can add new peer IP addresses using the input box below then clicking "Add". To remove an address, right-click on the address and select "Delete address".

## Access Permission

These are two lists of IP addresses that can connect to the RPC and WEB ports of your Qora client (if enabled). You can add IP addresses using the input box below then clicking "Add". To remove an address, right-click on the address and select "Delete address".

## settings.json

When you click "Apply" your settings.json file will be rewritten to reflect the new settings. 

# Wallet

## Start the application

## Create a Wallet

## Recover wallet from seed  

## Lock your wallet  

## Unlock your wallet  

# Accounts

## Create account

## Delete account

## Import account from seed

# Seed  

## Retrieve wallet's seed  

To retrieve the seed of your wallet you first need to have your [wallet unlocked](#unlock-your-wallet) in order to be able to get the seed.  
Open the console and type the below command :

> GET wallet/seed  

The above command will return the 32-byte long base58-encoded wallet seed.  

You can also made the above API request by simply visiting the below URL while RCP is enabled.  

### HTTP Request  

[http://127.0.0.1:9085/wallet/seed](http://127.0.0.1:9085/wallet/seed)  

If you have encountered an error while making the above request, the exact error code will be displayed.Below is the errors list.  

### ERRORS

| Error |	Description |
|-------|-------------|
| 201 |	Wallet does not exist. |
| 203 |	Wallet is locked. |

<aside class="warning">
The wallet seed is the ticket to access to your wallet, make sure it's kept safe and securely!
</aside>

## Retrieve account's seed

You can retrieve the seed of a specific address that exists in your wallet.  
To retrieve the seed of your addres you first need to have your [wallet unlocked](#unlock-your-wallet) in order to be able to get the seed.  
Open the console and type the below command :

> GET addresses/seed/{address}

The above command will return the 32-byte long base58-encoded seed of the given address.  

You can also made the above API request by simply visiting the below URL while RCP is enabled.  

### HTTP Request  

[http://127.0.0.1:9085/addresses/seed/{address}](http://127.0.0.1:9085/addresses/seed/{address})

If you have encountered an error while making the above request, the exact error code will be displayed.Below is the errors list.  

### ERRORS

| Error |	Description |
|-------|-------------|
| 102 |	Invalid address. |
| 201 |	Wallet does not exist. |
| 202 |	Address does not exist in wallet. |
| 203 |	Wallet is locked. |

<aside class="warning">
The addres seed is the ticket to access to your address, make sure it's kept safe and securely!
</aside>

## Generate a seed

You can generate a random base58 encoded seed with a simple API request.  
Open the console and type the below command :

> GET seed  

The above command will return a base58 encoded random seed of 32 bytes.These seeds can be used to [create a wallet](#create-a-wallet) or to [import an account](#import-account-from-seed).  
Use the optional parameter length to request a seed of {length} bytes.

> GET seed/{length}  

You can also made the above API request by simply visiting the below URL while RCP is enabled.  

### HTTP Request  

[http://127.0.0.1:9085/seed](http://127.0.0.1:9085/seed)  


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

1. Using your Qora client, first click on the "Naming Service" tab.
2. Next click on "Register" button. This should open a new window.
3. Select the Qora account that should own, and pay for, your new name from the drop-down list.
4. Type in your chosen name in the "Name" box. As you type the "Name Details" box below will inform you if your name has already been taken or not.
5. For first time use, you can ignore the "Key" and "Value" fields - or delete the "defaultkey" that is made for you using the "Remove" button.
6. Click the "Register" button and your name registration request transaction will be submitted to the Qora network for confirmation.

You will know when your new name is ready to use when the "Confirmed" tick-box is ticked.

## Update name

1. Using your Qora client, first click on the "Naming Service" tab.
2. Right-click on a name and select "Update" from the pop-up menu. This should open a new window.
3. In this new window you can change the owner (make sure you get the address correct) or add/remove key-value pairs associated with the name using the "Add" and "Remove" buttons.
  - To add a key-value pair, enter the key and value in the respective input boxes then click "Add"
  - To remove a key-value pair, single-click the pair in the list to highlight it then click "Remove"
  
Note that altering the data storage associated with a name is done via [the web-based name storage editor](http://127.0.0.1:9090/index/namestorage.html)

## Transfer name

## Exchange

## Buy a name

## Sell Name

## Cancel sell name

# Polls

## Navigate

## Vote

## Create a poll

# Assets

## Navigate

## View Asset details

## Add to Favorites

## Open Pair

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

Arbitrary transactions is a Qora feature that allows storage on the blockchain.  
The data of the arbitrary transaction must be base58 encoded and must be between 1-4000 bytes.

<aside class="notice">
Currently arbitrary transactions can only be made through the API.
</aside>

## Send arbitrary transaction

To create an arbitrary transaction, open the console and then send your Command.

Below you will see an example command.

> POST arbitrarytransacions {"creator": "QNbA69dbnmwqJHLQeS9v63hSLZXXGkmtC6",
"data":"4GFHMAo9fmbUq7usopgntwUfAiLtpL98K6QCosAJsqQmY95tfd5KoUaKu34v6Qwp7RtYEhobCx7LVi7aYbbtpzfA","service": 555,"fee": "1.00001"}


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

## Load arbitrary transaction

To load an arbitrary transaction, open the console and then send your Command.

Below you will see an example command.

> POST transactions/scan {"type":10,"creator":"QNbA69dbnmwqJHLQeS9v63hSLZXXGkmtC6"}  

Returns all the arbitrary transactions made by the given creator.  

# Automated Transactions

## Deploy AT

To deploy an AT (smart contract) go to the AT tab and click Deploy AT.

Enter the values accordingly on each field and click deploy.

# Atomic Cross-Chain Transfers

## Initiate ACCT

## Response ACCT  

# Qora Web

## Web Server

The built-in web server can be accessed by either:

- right-clicking on the Qora icon in your system tray and selecting "Qora Web/Social Network"
- from the "File" menu in your Qora client GUI select "Decentralized web server" (also via Alt-W)

## Browse the web

You can view blockchain-stored websites by going to the [web directory](http://127.0.0.1:9090/index/webdirectory.html).

## Deploy a website

First of all, you'll need a registered name. If you don't have one already, please see [Registering a name](#register-a-name).
To create/edit your name's website use the [web-based name storage editor](http://127.0.0.1:9090/index/namestorage.html)

1. First pick which name's website you want to create/edit from the drop-down list.
2. Make sure the "key" field is left blank (or explicitly use the key "website").
3. Create/edit your website either using the "data" field and its built-in *Visual Editor* OR upload the data from a file on your computer using the "BROWSE" button. (This will overwrite the contents of the "data" field).
4. Click "Submit" to submit your website to the Qora network for confirmation!

Note that the fee charged depends on how much data you store (i.e. the size of your website). Make sure you have enough balance!

# Tools

Here you can find a list of tools

## Block Explorer

[node.qora.tech](http://node.qora.tech:9090/index/blockexplorer.html) is an online Qora block chain browser which displays the contents of individual blocks, transactions, transaction histories, balances of addresses, unconfirmed transactions, assets, polls and many statistics.It's written and operated by agran and it's the official Qora block explorer.

## Blogging Service

Official blogging service of Qora has been created by _agran_.
You can view the [timeline of blog entries](http://node.qora.tech:9090/index/blog.html) or find individual blogs using the [blog directory](http://node.qora.tech:9090/index/blogdirectory.html).  
This service uses the arbitrary transactions feature of Qora to serve a socialized blogging suite.  
To create a new blog post click the new blog entry icon at the top of the [blog timeline page](http://node.qora.tech:9090/index/blog.html).  

## Faucet

## VanitygenQora

**VanitygenQora** is a command-line vanity Qora address generator created by agran.  
You can find the latest version here : [https://github.com/agran/VanitygenQora/releases](https://github.com/agran/VanitygenQora/releases)

## HTML Editor

## Multiple Pages Generator  

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


## Known Issues  

Please visit [Qora github issues page](https://github.com/Qoracoin/Qora/issues).

## Find help

## Report a bug  

Found a bug? You can report it at the [Qora github issues page](https://github.com/Qoracoin/Qora/issues).

# FAQ  

Here are some frequently asked questions that might help you.

# Developers  

## Import source code to Eclipse  

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

- Click on **Finish**

![/ Finish](https://i.imgur.com/BRmXqYz.png "/ Finish")

## Start the wallet from the Eclipse's workspace  

When you have successfully imported Qora to your Eclipse's Workspace you then can start the wallet by following the below steps:

- Select the **>Qora [Qora master]** from Package Explorer, click on Run on menu bar and then Run again.

![Run](https://i.imgur.com/j38tm5s.png "Run")

- Run as Java Application

![Run as Java Application](https://i.imgur.com/4Sb9CDZ.png "Run as Java Application")

- On the next step scroll down and click on the Start - (default package) and click OK

![Start](https://i.imgur.com/jUh89lu.png "Start")

<aside class="success">
You have launched the wallet directly from source
</aside>
## Compile Qora from source code  

- Select the **>Qora [Qora master]** from Package Explorer

![Master](http://i.imgur.com/H8tK1rZ.jpg "Master")

- Go to **/ File / Export / Java / Runnable JAR file**

![Export](https://i.imgur.com/sIadzQn.png "Export")

- Export

  - On Launch Configuration field select **Start - Qora** from the drop down menu.
    You will have to [run the wallet first](#start-the-wallet-from-the-eclipse's-workspace) in order to have the option **Start  - Qora** available
  - / Select Export destination
  - / Select Package required libraries into generated JAR

![Export](https://i.imgur.com/BXvovZj.png "Export")  

<aside class="success">
You have now compiled the Qora.jar file directly from source code.
</aside>  

## API  

Qora uses a REST API to communicate with the wallet.
You can find the entire API documentation here : [http://api.qora.org](http://api.qora.org)

## Submit a pull request  

You can submit a pull request to the source code by following the below steps.
