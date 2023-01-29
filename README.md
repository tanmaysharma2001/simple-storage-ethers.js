## Development guide

1. Solc.js for compiling solidity code:
    ```
    yarn solcjs --bin --abi --include-path node_modules/ --base-path . -o . SimpleStorage.sol
    ```
    we add the above command in scrips compile in package.json
2. Ganache: fake blockchain virtual machine
3. RPC: remote procedure call stands for a connection to a blockchain node that somebody is running
4. We use ethers.js to make api calls behind the scenes without actually having to use the axios library.
5. We connect our wallet as we are gonna need to it sign the transactions
6. to deploy the contract we need the abi and binary file
7. we need fs-extra package to read from the two files.
8. we also need contract factory to deploy contract
9. nonce: to send transactions
10. for ganache the network id is the chain id