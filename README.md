# Create an NFT Collection

## Simple Overview of Use/Purpose
This project focuses on building a straightforward NFT (Non-Fungible Token) collection using JavaScript. The program includes functionalities to mint new NFTs, display all created NFTs, and determine the total number of NFTs. This exercise is designed to teach the basics of creating and managing NFTs programmatically.
## Description
In this project, you will write JavaScript functions to create and manage an NFT collection. You will define a variable to hold the NFTs, implement a function to mint new NFTs with specific metadata, create a function to list all NFTs, and develop a function to get the total count of minted NFTs. This project offers a basic understanding of handling NFT collections and their metadata.

## Getting Started

### Installing

No installation is needed for this project since it is based on JavaScript. You can run the code in any JavaScript runtime environment, such as Node.js or a web browser console.
### Executing Program

1. Create a new JavaScript file and name it `nftCollection.js`.
2. Copy and paste the following code into the file:

    ```javascript
    // Create a variable to hold your NFTs
const NFTS = [];

// Function to mint a new NFT
function mintNFT(username, transactionCount, paytmBalance, membershipStatus, rewardPoints, linkedServices) {
    const NFT = {
        username: username,
        transactionCount: transactionCount,
        paytmBalance: paytmBalance,
        membershipStatus: membershipStatus,
        rewardPoints: rewardPoints,
        linkedServices: linkedServices,
    }
    console.log("Minted: " + username);
    NFTS.push(NFT);
}

// Function to list all NFTs
function listNFTS() {
    for(let i = 0; i < NFTS.length; i++){
        console.table(NFTS[i]);
    }
}

// Function to get the total supply of NFTs
function getTotalSupply() {
    console.log("Total NFT's: " + NFTS.length);
}

// Minting some NFTs
mintNFT("user_ashish", 500, 15000, "Gold", 1200, ["Paytm Wallet", "Paytm Postpaid"]);
mintNFT("user_neha", 300, 8000, "Silver", 800, ["Paytm Wallet", "Paytm Insurance"]);
mintNFT("user_rahul", 700, 20000, "Platinum", 2000, ["Paytm Wallet", "Paytm Bank", "Paytm Postpaid"]);
mintNFT("user_ria", 200, 5000, "Silver", 600, ["Paytm Wallet", "Paytm Insurance"]);
mintNFT("user_ankit", 1000, 30000, "Platinum", 3000, ["Paytm Wallet", "Paytm Bank", "Paytm Postpaid", "Paytm Insurance"]);
mintNFT("user_kiran", 400, 10000, "Gold", 1500, ["Paytm Wallet", "Paytm Postpaid"]);

listNFTS();
getTotalSupply();
    ```

3. Run the program using a JavaScript runtime environment, such as Node.js, or by copying the code into a web browser console.

    ```bash
    node nftCollection.js
    ```

## Help

For common problems or issues:

1. Ensure your JavaScript runtime environment is properly set up.
2. Double-check the syntax for any typos or errors.
3. Make sure the functions are called correctly with the appropriate parameters.

For further assistance, you can refer to JavaScript documentation or seek help from online programming communities.

## Authors

Contributors:

- Sonu Choubey  
  - GitHub: [@sonuchoubey](https://github.com/sonuchoubey)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
