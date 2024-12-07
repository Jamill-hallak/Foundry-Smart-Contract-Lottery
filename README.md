
# **Foundry Smart Contract Lottery**

This project was developed as part of the **Cyfrin Foundry Solidity Course**, where I built a decentralized lottery system powered by **Chainlink VRF** and **Chainlink Automation**. The project demonstrates expertise in Solidity, Foundry, and blockchain development.

---

## **Project Overview**

This lottery system uses **Chainlink VRF** for provably fair randomness and **Chainlink Automation** to automate winner selection. It includes comprehensive testing, deployment on **Sepolia**, and automation using upkeeps.

### **Core Features**
- **Fair Winner Selection**: Uses **Chainlink VRF** to select winners randomly and verifiably.  
- **Automated Lottery Draws**: Utilizes **Chainlink Automation** to automatically trigger the winner selection.  
- **Full Stack Testing**: Includes **unit, integration, and forked tests** to ensure contract reliability.  
- **Sepolia Testnet Deployment**: Deployed to **Sepolia** with environment variables for security and flexibility.

---

## **Why Chainlink?**
**Chainlink** ensures the lottery process is secure, transparent, and automated.  
- **VRF (Verifiable Random Function)**: Ensures fair randomness for winner selection.  
- **Automation (Upkeep)**: Triggers the lottery draw automatically, reducing manual intervention.  

These features provide **decentralization, security, and transparency** in the lottery process. 

---

## **Getting Started**

### **Requirements**
- **Git**: [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  
  Verify with: `git --version`
- **Foundry**: [Install Foundry](https://getfoundry.sh/)
  
  Verify with: `forge --version`

---

### **Quickstart**

\`\`\`bash

git clone https://github.com/Jamill-hallak/Foundry-Smart-Contract-Lottery.git

cd foundry-smart-contract-lottery-cu

forge build

\`\`\`

---

## **Usage**

### **Run Local Blockchain**
Start a local blockchain using **Anvil**:  
\`\`\`bash

make anvil

\`\`\`

### **Test the Contract**
Run all tests locally:  
\`\`\`bash

forge test

\`\`\`

Run forked tests against **Sepolia**:  
\`\`\`bash

forge test --fork-url $SEPOLIA_RPC_URL

\`\`\`

---

## **Deployment**

1. **Set Environment Variables**  
   Create a `.env` file with:  
   \`\`\`bash
   
   SEPOLIA_RPC_URL=<Your Sepolia RPC URL>
   PRIVATE_KEY=<Your Metamask Private Key>
   
   \`\`\`

3. **Get Testnet ETH**  
   Visit [faucets.chain.link](https://faucets.chain.link/) to receive **Sepolia ETH**.

4. **Deploy Contract**  
   Deploy to **Sepolia**:  
   \`\`\`bash
   make deploy ARGS="--network sepolia"
   \`\`\`

5. **Register Chainlink Automation**  
   Register a new upkeep at [Chainlink Automation](https://automation.chain.link/new) to automate the lottery draw.

---

## **Chainlink Services**

### **Chainlink VRF**  
- Generates a verifiable, tamper-proof random number for winner selection.  
- Enhances trust and fairness in the lottery process.  

### **Chainlink Automation**  
- Automates the process of drawing the winner.  
- Uses an upkeep to monitor lottery conditions and trigger winner selection.  

---

## **Commands**

| **Command**           | **Description**                      |
|---------------------  |------------------------------------- |
| \`make anvil\`          | Start a local blockchain (Anvil)      |
| \`forge build\`         | Compile contracts                    |
| \`forge test\`          | Run all tests                        |
| \`make deploy\`         | Deploy to Sepolia testnet            |
| \`make createSubscription\` | Create a Chainlink VRF subscription |

---

## **Conclusion**

This project showcases my ability to integrate **Chainlink VRF** and **Automation** into a decentralized lottery system. It highlights my skills in Solidity, smart contract development, and blockchain deployment using **Foundry**. If you'd like any adjustments or additional details, feel free to reach out!
