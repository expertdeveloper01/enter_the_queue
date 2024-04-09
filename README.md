# Enter The Queue

Where Real World Art Comes To Life In The Digital World.
Marketplace website for NFT (Non-Fungible Token) on ethereum blockchain.


![Logo](https://enterthequeue.com/_next/image/?url=%2Fimg%2Flogo.png&w=256&q=75)


## Developers

- [@paradisetechsoftsolutions](https://github.com/paradisetechsoftsolutions)
- [@paradisetester](https://github.com/paradisetester)


## Tech Stack

**Framework:** [Nextjs](https://nextjs.org/)

**Client:** [Material UI](https://mui.com/), [Tailwind Css](https://tailwindcss.com/)

**Server:** [Node](https://nodejs.org), [pm2](https://pm2.keymetrics.io/), [NVM (Node Version Manager)](https://github.com/nvm-sh/nvm)

**Database:** [Mongodb](https://www.mongodb.com/)

**Miscellaneous:** [Infura](https://infura.io/), [Hardhat](https://hardhat.org), [Web3modal](https://web3modal.com/)

## Requirements for the project

- [Mongodb](https://www.mongodb.com/try/download/community) `required`
- [Node](https://nodejs.org/en/download/) (v18.12.1) `required`
- [NVM for ubuntu](https://github.com/nvm-sh/nvm#installing-and-updating) 
- [NVM for window](https://github.com/coreybutler/nvm-windows/releases)


## Run Locally

Clone the project

```bash
  git clone https://gitlab.com/paradisetechsoft/jennifer-build-marketplace.git enterthequeue
```

Go to the project directory

```bash
  cd enterthequeue
```

Use Node (v18.12.1) for the project

```bash
  nvm use
```

Install dependencies

```bash
  npm install
```

Generate contract ABI files of the smart contracts

```bash
  npx hardhat compile
```

Befor run the below command please check **Environment Variables** section

Start the dev server

```bash
  npm run dev
```


## Deployment

Deploy Marketplace Smart Contract through [Remix Online IDE](https://remix.ethereum.org/)

Create build of the project

```bash
  npm run build
```

Check build code on local
```bash
  npm run start
```

On live server (restart the pm2 server)

```bash
  pm2 restart {command_name}
```


## Environment Variables

To run this project, you will need to copy the content from .env.example file to your .env file

### .env file

```env
# Private key of the wallet
PRIVATE_KEY=

# SECRET key
SECRET='enter-the-queue-token'

# Chain ids of the network
CONTRACT_CHAIN_NETWORK="goerli"

# Base Url
APP_BASE_URL="http://localhost:3000/"


# NFT addresses
NFT_MARKET_PLACE_ADDRESS="0xc7Fa7CC756F6b418b58B57469D25CE80518Fb0C7"
NFT_ADDRESS="0x195d3011b05D4ab85117171F1a939580283A2c28"

# MongoDb Details
MONGODB_URI="mongodb://127.0.0.1:27017/"
MONGODB_NAME="enter-the-queue"

# Infura Details
INFURA_PROJECT_ID=
INFURA_PROJECT_SECRET=
INFURA_API_ENDPOINT="https://ipfs.infura.io:5001"
INFURA_IPFS_BASE_URL=
INFURA_RPC_ENDPOINT="https://${CONTRACT_CHAIN_NETWORK}.infura.io/v3/${INFURA_KEY}"

```

### variables.json file

```env
{
    "PRIVATE_KEY": "",

    "SECRET": "enter-the-queue-token",

    "CONTRACT_CHAIN_NETWORK": "goerli",

    "APP_BASE_URL": "http://localhost:3000/",

    "NFT_MARKET_PLACE_ADDRESS": "0xc7Fa7CC756F6b418b58B57469D25CE80518Fb0C7",
    "NFT_ADDRESS": "0x195d3011b05D4ab85117171F1a939580283A2c28",
    
    "MONGODB_URI": "mongodb://127.0.0.1:27017/",
    "MONGODB_NAME": "enter-the-queue",
    
    "INFURA_PROJECT_ID": "",
    "INFURA_PROJECT_SECRET": "",
    "INFURA_API_ENDPOINT": "https://ipfs.infura.io:5001",
    "INFURA_IPFS_BASE_URL": "",
    "INFURA_RPC_ENDPOINT": "https://goerli.infura.io/v3/f9a50f205dd4475bbf1da2a0d21f7c36"
    
}


```

