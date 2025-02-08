# fake-product-Detection--using-Blockchain
1. Doiwnload node js V 17.0.1 <a href="https://nodejs.org/en/blog/release/v17.0.1">Node Js Link</a> or version between 16 to below 18 and ganache <a href="https://archive.trufflesuite.com/ganache/">Ganachelink</a>.
2. Go to the project folder, open terminal there and run following command to install required node_modules:-
```
npm install
```
3. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-
```
truffle compile
```
4. Open Ganache, (to setup local blockchain)
    - crerate new workspace
    - add truffle-config.js  in truffle project 
    - change port to 7545 in server settings (same as port in truffle-config.js)
5. In chrome, open metamask link : <a href="https://metamask.io/download/">Metamask</a>
   - add new test network using  
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:7545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import account using private key of any account from local blockchain available in Ganache.
6. In terminal, run following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```
- To start a server and it will open a homepage (index.html) file in the default browser.
```
npm run dev 
``` 
7. Login to metamask ,and connect the added account to local blockchain by clicking the 'Connect Wallet' button on the homescreen.
8. Interact with website
