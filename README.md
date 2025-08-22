# web3-message-app

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Simple Web3 App</title>
  <link rel="stylesheet" href="style.css">
  <!-- Ethers v6 UMD bundle -->
  <script src="https://cdn.jsdelivr.net/npm/ethers@6.13.2/dist/ethers.umd.min.js"></script>
</head>
<body>
  <div class="app">
    <h1>Simple Web3 App</h1>

    <div class="card">
      <button id="connectBtn">Connect Wallet</button>
      <div id="status" class="status">Not connected</div>
      <div class="network">Target network: Sepolia (chainId 11155111)</div>
      <div class="small">If asked, approve switching to Sepolia.</div>
    </div>

    <div class="card">
      <h2>Read</h2>
      <div>Current message:</div>
      <pre id="currentMessage">—</pre>
      <button id="refreshBtn">Refresh</button>
    </div>

    <div class="card">
      <h2>Write</h2>
      <input id="messageInput" placeholder="Type a new message" />
      <button id="updateBtn">Update Message</button>
      <div id="txStatus" class="small"></div>
    </div>

    <footer>
      <div class="small">
        Set your contract address in <code>app.js</code> (look for REPLACE_WITH_YOUR_CONTRACT_ADDRESS).
      </div>
    </footer>
  </div>

  <script src="app.js" type="module"></script>
</body>
</html>
