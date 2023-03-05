# DIING.xyz

## One-Sentence

Diing is a personal finance dApp that supports ZK-based magic links for token transfers and also offers on-chain credit score checking and lending services.

---

## Summary

Diing provides a magic link for token transfers, eliminating the need for users to ask for each other's wallet addresses. For example, if Alice, a community manager at Discord, wants to airdrop tokens to Bob, a holder of a crypto community, Alice can simply create a magic link in Diing and send it to Bob, who can then claim the token by clicking the link. The link is encrypted using ZK technology, ensuring privacy and security. Diing is also useful for onboarding people who don't have a crypto wallet yet.

In addition to token transfers, Diing offers two other services with on-chain credit. Users can check their credit score by connecting their wallet, and based on their score, they can use Diing's internal pool-based lending service.

---

## Problem

Communicating with people on Discord, Telegram, or Snapchat and asking for wallet addresses to transfer tokens is time-consuming and inconvenient, especially for anonymous communities.

---

## Target Users

1. Community managers of Discord and Telegram groups who want to transfer tokens without asking for wallet addresses.
2. **Users who don't have a crypto wallet yet** and want to claim tokens using Diing's magic links.

## User Stories

### **Sender**

1. Connect the wallet and select the desired cryptocurrency.
2. Set the amount and message, then create a magic link.
3. Share the link with the receiver.

### **Receiver**

1. Click the link sent by the sender on Discord or Telegram.
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