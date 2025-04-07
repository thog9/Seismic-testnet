# Seismic Testnet Scripts

This repository contains Python scripts for interacting with Seismic, a high-performance blockchain network. Commands for receiving permissioned tokens from token contracts and NFTs, minting tokens/NFTs, sending transactions, and managing assets on Seismic via RPC. Uses the `web3.py` library, supports Vietnamese and English.

Faucet: [Seismic Faucet](https://faucet-2.seismicdev.net/)

## Features Overview

### General Features

- **Multi-Account Support**: Reads private keys from `pvkey.txt` to perform actions across multiple accounts.
- **Colorful CLI**: Uses `colorama` for visually appealing output with colored text and borders.
- **Asynchronous Execution**: Built with `asyncio` for efficient blockchain interactions.
- **Error Handling**: Comprehensive error catching for blockchain transactions and RPC issues.
- **Bilingual Support**: Supports both English and Vietnamese output based on user selection.

### Included Scripts

1. **sendtx.py**: Send random token transactions or to addresses from address.txt on Seismic.
2. **deploytoken.py**: Deploy an ERC20 token smart contract on Seismic.
3. **sendtoken.py**: Send ERC20 tokens to random addresses or from addressERC20.txt on Seismic.
4. **nftcollection.py**: Deploy and manage an NFT smart contract (Create, Mint, Burn) on Seismic.
5. **mintair.py**: Deploying Timer Contract on Seismic.

## Prerequisites

Before running the scripts, ensure you have the following installed:

- Python 3.8+
- `pip` (Python package manager)
- **Dependencies**: Install via `pip install -r requirements.txt` (ensure `web3.py`, `colorama`, `asyncio`, `eth-account`, and `inquirer` are included).
- **pvkey.txt**: Add private keys (one per line) for wallet automation.
- **address.txt / addressERC20.txt**: Optional files for specifying recipient addresses.

## Installation

1. **Clone this repository:**
- Open cmd or Shell, then run the command:
```sh
git clone https://github.com/thog9/Seismic-testnet.git
```
```sh
cd Seismic-testnet
```
2. **Install Dependencies:**
- Open cmd or Shell, then run the command:
```sh
pip install -r requirements.txt
```
3. **Prepare Input Files:**
- Open the `pvkey.txt`: Add your private keys (one per line) in the root directory.
```sh
nano pvkey.txt 
```
- Open the `address.txt`(optional): Add recipient addresses (one per line) for `sendtx.py`, `deploytoken.py`, `sendtoken.py`,`nftcollection.py`.
```sh
nano address.txt 
```
```sh
nano addressERC20.txt
```
```sh
nano contractERC20.txt
```
```sh
nano contractNFT.txt
```
4. **Run:**
- Open cmd or Shell, then run command:
```sh
python main.py
```
- Choose a language (Vietnamese/English).

## Contact

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099) 

## BUY ME COFFEE

- **BUYMECAFE**: https://buymecafe.vercel.app/
