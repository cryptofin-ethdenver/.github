# DIING.xyz
### Meet Diing!
https://www.diing.xyz

## One-Sentence

Diing is a personal finance dApp that supports ZK-based magic links for token transfers and also offers on-chain credit score checking and lending services.

---

## Git Repositories
*CHECK HOW WE USED TRUFFLE & INFURA HERE*<br>
AWESOME SmartContracts: https://github.com/cryptofin-ethdenver/diing-contract<br/>
Price Crawler BE: https://github.com/cryptofin-ethdenver/diing-be

---

## Summary

Diing provides a magic link for token transfers, eliminating the need for users to ask for each other's wallet addresses. For example, if Alice, a community manager at Discord, wants to airdrop tokens to Bob, a holder of a crypto community, Alice can simply create a magic link in Diing and send it to Bob, who can then claim the token by clicking the link. The link is encrypted using ZK technology, ensuring privacy and security. Diing is also useful for onboarding people who don't have a crypto wallet yet.

In addition to token transfers, Diing offers two other services with on-chain credit. Users can check their credit score by connecting their wallet, and based on their score, they can use Diing's internal pool-based lending service.

---

## Problem

Communicating with people on Discord, Telegram, or Snapchat and asking for wallet addresses to transfer tokens is time-consuming and inconvenient, especially for anonymous communities.

---

## Target Users

1. Community managers of Discord and Telegram groups who want to transfer tokens without asking for wallet addresses.<br/>
2. **Users who don't have a crypto wallet yet** and want to claim tokens using Diing's magic links.

## User Stories

### **Sender**
<img src="./deposit.jpeg">
1. Connect the wallet and select the desired cryptocurrency.<br/>
2. Set the amount and message, then create a magic link.<br/>
3. Share the link with the receiver.



### **Receiver**
<img src="./withdraw.jpeg">
1. Click the link sent by the sender on Discord or Telegram.<br/>
2. Be redirected to Diing's interface and claim the tokens.

### Currencies

- ETH
- USDC
- USDT
- MATIC

---

## Solution

Diing eliminates the need to know the receiver's wallet address. Users can choose the token and amount in their wallet and create a magic link in Diing. The magic link is encrypted using ZK technology, ensuring privacy and security.

---

## Feature Development

1. **ZK-based magic links for token transfers**
    
    Create a link without knowing the receiver's wallet address.
    
2. **On-chain credit score checking**
    
    Check your credit score for crypto credit management.
    
3. **Lending service**
    
    Users with a credit score of over 700 can choose to use Diing's internal pool-based lending service or Huma Protocol's lending service.
    

---

## Future Development

1. **Meta Transaction Support**
    
    Add actual user support in gas fee payment
    
2. **Account Abstraction support**
    
    Implement account abstraction support
    
3. **Cooperation with wallets wants mass adoption**
    
    Cooperate with wallet providers to onboard more users to Diing.

## Smart Contract Addresses
All networks are testnets. We supports 

### ETH

- DiingTransfer: Currently N/A
- DiiingLoan: Currently N/A
- USDC: 0xae8130a68e2a58D9Fc819B3D17f882fC6D1d4e8e
- USDT: 0x38AB0a1773410c158B43c070Cb4a8E2657f2E5d8
- MATIC: 0x3AdBFE246c472c4b7bF137E2E1957CD0A0b6bA1c

### MATIC

- DiingTransfer:
- DiiingLoan:
- USDC: 0xae8130a68e2a58D9Fc819B3D17f882fC6D1d4e8e
- USDT: 0x38AB0a1773410c158B43c070Cb4a8E2657f2E5d8
- ETH: 0x67960C2276b8A8949376E10d227207D041F0eA64

### AURORA

- DiingTransfer: 0x1D805ad4EC233960f97Ab3C870266447d49bd09eLOAN
- DiiingLoan: 0x0bC539932E09E27A0434A13512Db21c377e0832f
- USDC: 0x88801948C288c5Aea29fCb283564d3584D1643fa
- USDT: 0xB30D9c09a8fdF7a8d937Cc68F2148B5257031797
- MATIC: 0x8BC49BDb972f668380ac6c73480eb4534a6E8805

### BASE

- DiingTransfer: 0x02B4a411a2775ECC8fd814718CAf0ca90e5fFC76
- DiiingLoan: 0xc627dd27c08347fAe786A3EF6A1F7AA62c23241b
- USDC: 0xB30D9c09a8fdF7a8d937Cc68F2148B5257031797
- USDT: 0xae8130a68e2a58D9Fc819B3D17f882fC6D1d4e8e
- MATIC: 0x38AB0a1773410c158B43c070Cb4a8E2657f2E5d8

### Scroll

- DiingTransfer: 0x7209bf1f5d472D936aCA18F59B37CA41a575E995
- DiiingLoan: 0xEe72088c20cEECD5a12aa99a86b91181Ee1915D1
- USDC: 0x88801948C288c5Aea29fCb283564d3584D1643fa
- USDT: 0xB30D9c09a8fdF7a8d937Cc68F2148B5257031797
- MATIC: 0xae8130a68e2a58D9Fc819B3D17f882fC6D1d4e8e

## Bounty & Challenges we ran into
### 1. Truffle + Infura
As we support several networks(Ethereum, Polygon Aurora, Base, Scroll), Truffle and Infura were great choice to manage multiple networks and RPCs
### 2. Polygon
MATIC amount supported by faucet is too limited. PolygonScan is a bit slow but useful. Other things were really satisfying.
### 3. Base
It's good that Faucet is Coinbase wallet, Mainnet ETH balance is necessary to claim. This point was inconvenient. But it was not a big problem cause we purchased our own ETH.
### 4.Scroll
Considering contract It was same as EVM. But our front end framework was Wagmi, Scroll didn???t support directly. So it took much more time for customizin
### 5. Near Aurora
We don't know the reason but network was too slow. We spent most of the time to make contract creation call.
### 6. Cypher
We tried a mobile connecting at the first time, Cypher doesn't support mile modal, So we connect Cypher's modal in web. The close button was disappeared at the token listing page, we've questioned cypher's discord and solved it.
### 7. Spectral Finance
Spectral supported partner API for credit score. We wereWe lack of the rate limit on the development process. Spectral Finance team supported more rate limit with 5000 requests.
### 8. Huma Finance
We support Huma Finance lending service for users who want to use in-service lending.
### 9. Wallet connect
Web3modal was great tool, but wallet addition was tricky. WAGMI was the easiest example so we changed stack once.
