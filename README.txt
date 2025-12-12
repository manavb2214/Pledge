
PLEDGE (Demo)
===========================

Files:
- index.html : Single-file frontend that connects to MetaMask and PLEDGE contract.
- This folder is safe to unzip on your machine.

How to use:
1) Edit index.html:
   - Open index.html in a text editor.
   - Replace the placeholder string REPLACE_WITH_YOUR_CONTRACT_ADDRESS with your contract address.
   - Replace the placeholder CONTRACT_ABI = /* PASTE_YOUR_CONTRACT_ABI_ARRAY_HERE */ [] with the ABI JSON array you copied from Remix.
     Make sure the ABI is pasted as a JavaScript array (starts with [ and ends with ]). Do not wrap it in quotes.

2) Serve the file over HTTP (recommended):
   - Using Python 3:
       python -m http.server 8000
     Then open http://localhost:8000/index.html
   - Or use VS Code Live Server extension.

3) In the page:
   - Click "Connect Wallet" and allow MetaMask.
   - The UI shows NGOs, donation inputs, donation history.
   - Owner account can use "Add NGO".
   - Donor account can "Donate" (enter ETH like 0.01).
   - NGO account can "Withdraw".

Notes:
- Make sure MetaMask is on the same test network you deployed the contract to (e.g., Sepolia or Polygon Mumbai).
- Amounts are processed using ethers.js; small decimals should be entered like "0.01".
- If you see errors, open browser console (F12) - the page logs helpful messages.
