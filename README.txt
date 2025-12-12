
PLEDGE (Demo)
===========================

Files:
- index.html : Single-file frontend that connects to MetaMask and PLEDGE contract.
- This folder is safe to unzip on your machine.

How to use:
1) Edit index.html:
   - Open index.html in a code editor, Visual Studio Code is recommended.

2) Serve the file over HTTP:
   - Using Python 3:
       python -m http.server 8000
     Then open http://localhost:8000/index.html
   - Or use VS Code Live Server extension.

3) In the page:
   - Click "Connect Wallet" and allow MetaMask.
   - The UI shows NGOs, donation inputs, donation history.
   - Owner account can use "Add NGO".
   - Donor account can "Donate" (enter ETH like 0.001)
   - NGO account can "Withdraw".

Notes:
- Make sure MetaMask is on the Ethereum Sepolia test network because the contract has been deployed on Sepolia.
- Amounts are processed using ethers.js; small decimals should be entered like "0.001".

