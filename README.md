# ProofofExistence
Proof of Existence Smart Contracts

First run 'truffle compile' to compile the contracts within the proofofExistence directory. 
Second, create your own .secret file with your 12 seed Mnemonic phrase from your Metamask account on the Rinkeby network. 
Third, signup for Infura. 
Fourth, create a project "Proof Of Existence" on Infura. 
Fifth, grab the project id and insert it into the truffle-config.js file. 
Sixth, run 'npm install truffle-hdwallet-provider'
Seventh, declare a variable called infuraURL, set it equal to the Rinkeby network address in your Infura project. 
  'const infuraURL= "https://rinkeby.infura.io/v3/
Eighth: check the rinkeby network options: 
`rinkeby: {
      provider: () => new HDWalletProvider(mnemonic, infuraURL),
      network_id: 4,       // Rinkeby's network id
      gas: 5500000
    }`

Nineth, run 'truffle migrate --network rinkeby' to deploy the contracts to the Rinkeby network. 

If you have any trouble with an already deployed contract, try running 'truffle migrate --reset --network rinkeby'. 
This will redeploy the contracts to the Rinkeby network. 

If you have any questions or comments, let me know! 

Feel free to test the contracts and deployment on Ganache first. 

Tools used: Truffle, Truffle-HDWallet-Provider, Infura, (optional:Ganache)
