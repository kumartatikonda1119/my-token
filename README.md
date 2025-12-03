# 🪙 MyToken (MTK)

## 🚀 Overview

**MyToken** is a simple **ERC-20 compliant cryptocurrency token** built on the Ethereum blockchain as part of my blockchain learning journey.  
This project helped me understand how real-world tokens like **USDT, LINK, and SHIB** work internally using smart contracts and mappings.

The token supports transfers, approvals, delegated transfers, and emits standard ERC-20 events — making it compatible with Ethereum tools and wallets.

---

## 🪙 Token Details

| Property        | Value               |
|----------------|---------------------|
| **Name**       | MyToken             |
| **Symbol**     | MTK                 |
| **Decimals**   | 18                  |
| **Total Supply** | 1,000,000 MTK      |

> Internally stored as: `1000000000000000000000000` (1M × 10^18)

---

## 🧠 What is an ERC-20 Token?

ERC-20 is the Ethereum token standard that defines how a token must behave.  
If a smart contract follows this standard, then:

- Wallets like MetaMask can detect & show balances  
- Exchanges can list the token  
- Smart contracts can use it without modifications  

It’s the reason Web3 has thousands of interoperable tokens.

---

## 📁 Project Structure
my-token/
├── contracts/
│   └── MyToken.sol
├── screenshots/
│   ├── allowance.png
│   ├── approve.png
│   ├── balance-of-A-after-transaction.png
│   ├── balance-of-B-after-transaction.png
│   ├── compilation.png
│   ├── deployment.png
│   ├── token-info.png
│   └── transfer-from.png
└── README.md



---

## 🛠 Smart Contract Features

| Feature | Description |
|--------|-------------|
| **Mint at Deployment** | Entire supply minted to deployer's wallet |
| **Transfer** | Send tokens to any valid address |
| **Approve** | Give permission to another address to spend tokens |
| **transferFrom** | Spender uses approved tokens on behalf of owner |
| **balanceOf** | Check token balance of any address |
| **allowance** | See remaining approved tokens |
| **Events** | Emits `Transfer` and `Approval` logs |

---

## 🚀 Deployment Instructions (Remix IDE)

1. Open Remix: https://remix.ethereum.org  
2. Create file: `contracts/MyToken.sol`  
3. Paste the smart contract code  
4. Compile using **Solidity 0.8.x**  
5. Deploy using **Remix VM**  
6. Enter this initial supply:1000000000000000000000000

7. Click **Deploy** ✔️

---

## 🧪 Usage Examples

### Check Balance
balanceOf(0xYourAddress)
transfer(0xRecipient, 1000000000000000000) // 1 MTK
approve(0xSpender, 3000000000000000000) // 3 MTK
transferFrom(0xOwner, 0xRecipient, 1000000000000000000)
allowance(0xOwner, 0xSpender)


---

## 🧾 Tests Performed

✔️ Contract compiled successfully  
✔️ Deployed on Remix VM  
✔️ `balanceOf` returned correct values  
✔️ `transfer()` updated balances correctly  
✔️ `approve()` set spender allowance  
✔️ `transferFrom()` reduced allowance and transferred tokens  
✔️ `Transfer` and `Approval` events emitted properly  

Screenshots included in `/screenshots`.

---

## 🎯 What I Learned

- What ERC-20 tokens are and why the standard is important  
- How Ethereum stores token balances using `mapping(address ⇒ uint256)`  
- Why `transferFrom` needs an approval mechanism  
- The purpose of `decimals` and `18` precision  
- How event logs help track token actions on the blockchain  
- Basics of smart contract deployment and testing

This project was my entry point into **Blockchain & Web3 development** and gave me confidence to explore advanced concepts like NFTs, DeFi, and smart contract design.

---

## 👨‍💻 Author

**Kumar Swamy Tatikonda**  
B.Tech CSE (AI & ML) Student  
Passionate about DSA, AI, and full-stack development 🚀

---

## 🏁 Conclusion

**MyToken (MTK)** is a complete, working ERC-20 token that follows Ethereum standards, supports all required functions, and demonstrates core blockchain concepts clearly.  
This project serves as a strong foundation for creating production-ready tokens, decentralized apps, and future Web3 innovations.

---

