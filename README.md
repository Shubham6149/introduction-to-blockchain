# Introduction-to-blockchain
# Blockchain-practical-metamask-wallet
This repo contains my blockchain practical screenshots and transaction hash.

# Create Metamask Wallet (Sepolia Testnet)
   # Introduction
This is a practical task demonstrate how to create a Metamask wallet and perform a transaction using the Sepolia Testnet.

# Transaction details
Network : Sepolia Testent Amount Sent : 0.02 ETH Transaction hash:
<br>
0x30592f0abe394df3be9d0c9932c5498b09929410f980727a079f99e8d41acc93view
<br>
(https://sepolia.etherscan.io/tx/0x30592f0abe394df3be9d0c9932c5498b09929410f980727a079f99e8d41acc93) Status : Successful

# Getting Sepolia ETH from Faucet
1.Visited the google cloud Sepolia Faucet.
<br>
2.Logged in with my google account.
<br>
3.Entered my Metamask wallet address.
<br>
4.Clicked on "Request 0.05 ETH".
<br>
5.ETH was sent to my wallet within a few seconds.
<br>
6.Verified the transaction on sepolia Etherscan.
# Screenshot
<br>
Below is the screenshot of getting ETH from sepolia faucet using google cloud: Screenshot 2025-04-08 120659

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/c419c994e1b294e696eece66e8664d2b5c1f24eb/Screenshot%202025-04-08%20170241.png)

# Steps followed
1.Connected Metamask to Sepolia Testnet.
<br>
2.Claimed Sepolia ETH from faucet.
<br>
3.Sent ETH to another Address.
<br>
4.Verified transaction was confirmed.
# Screenshot
Below is the screenshot of the transaction: Screenshot 2025-04-07 213239
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/eb92c420254fab1656962e38fe0fc3dd4407d60a/Screenshot%202025-04-08%20170404.png)
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/2b1b0bd2fd57b38edcb9ac65eedc251facc34a1a/Screenshot%202025-04-11%20081631.png)


# IPFS Practical - Uploading a file to IPFS
# IPFS Installation
I downloaded and install IPFS desktop for windows from the official website : (https://docs.ipfs.tech/install/ipfs-desktop/)

# IPFS Setup
1.After installing, I launched the IPFS desktop.
<br>
2.IPFS node automatically connected and status showed as Online.
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/180752cf40c31e3c7a3a8f53c9ac5aed9c81785d/Screenshot%20(2).png)


# File Upload
1.I clicked on the file section in IPFS Desktop.
<br>
2.Then i selected the option "Import" and uploaded a sample file, picture of flower and music also.
<br>
3.Once the file was uploaded, IPFS generate a unique CID(Content Identifier) for the file.
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/6df133f50023617a56eb99b49d9172e02148f40b/Screenshot%20(5).png)
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/a1b48d3f6eb73d8270b04ccf6c3f69306faf3336/Screenshot%20(4).png)


# Assignment 5: IPFS Privacy and Encryption
This assignment demonstrates how to use the InterPlanetary File System (IPFS) along with OpenSSL to perform file encryption and ensure privacy via the command line.

# Steps
# 1. Create a file to be added to IPFS
```

echo "Hello, IPFS!" > myfile.txt
```
<br>

# 2.Add the original file to IPFS
```

ipfs add myfile.txt
```
# 3.Encrypt the file using OpenSSL (AES-256-CBC)
```

openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword
```
# 4.Add the encrypted file to IPFS
```

ipfs add myfile_encrypted.txt
```
# 5.View the encrypted file (optional)
```

cat myfile_encrypted.txt
```
# 6.Decrypt the file
```

openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword
```
# 7.Verify the decrypted file content
```

cat decrypted_file.txt
```
# 8.Add the decrypted file to IPFS
```

ipfs add decrypted_file.txt
```

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/2913b4807c0a523feccfc47339d8db17027128f2/Screenshot%202025-04-20%20160622.png)

# Notes
● Replace `yourpassword` with a strong, secure password of your choice.
<br>
● Ensure that IPFS is properly installed and initialized before running these commands.



# Hyperledger Fabric Practical
<br>

# 1. Install Golang
 <br>

```

sudo apt install golang-go
```

<br>
Installs Golang, which is necessary for running Hyperledger Fabric binaries.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8b945277507cdb260b5077bb727f56ebbf6f74b6/Screenshot%202025-04-16%20220330.png)

# 2. Check Docker Version
```
docker --version
```
<br>
Verifies that Docker is installed and running correctly.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/60995a7ce104d527d0fef2112a50ab0ea0baaa4b/Screenshot%202025-04-16%20220342.png)

# 3.Check Docker Compose Version
```
docker compose version
```
<br>
Verifies the installation of Docker Compose.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/a1e87e4b0f7abf24eb6de9a8a150b1cce67de2e5/Screenshot%202025-04-16%20220352.png)

# 4.List Files in Current Directory
```
ls
```
<br>
Shows the list of files and folders in the current directory.


# 5.Clone the Fabric Samples Repository and Move into the Cloned Folder
```
git clone -b main https://github.com/hyperledger/fabric-samples.git
```
<br>
Downloads the official Hyperledger Fabric sample code from GitHub. Enters the cloned folder where Fabric examples are available.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/da5fcfde196a72065455d0d042c854ff7fe6c401/Screenshot%202025-04-16%20220408.png)

# 6.Download Fabric Binaries
```
curl -sSL https://bit.ly/2ysbOFE | bash -s
```
<br>
Downloads necessary Fabric binaries and Docker images like peer, orderer, and cryptogen.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/0ddebda48d2428b03eb88c0347bf3f66b0d4b8e5/Screenshot%202025-04-16%20220524.png)
<br>
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/66c340382f6ee3bf920b01e6f08ece2fc313e373/Screenshot%202025-04-16%20220556.png)

# 7.Enter the Test Network Directory
```
cd test-network
```
<br>
Navigates to the directory that contains scripts for running a sample Fabric network.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/945b4ad4f46e56dc57d14c3cb519d582fa798677/Screenshot%202025-04-16%20220614.png)

# 8.View the Network Script
```
./network.sh
```
<br>
Shows the options available with the network.sh script.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/b82ab3b32647da9bcfcccdb280064efbde465c2a/Screenshot%202025-04-16%20220638.png)

# 9.Start the Fabric Network
```
./network.sh up
```
<br>
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/a211b218b2403536e1669b499ae3199597212898/Screenshot%202025-04-16%20221553.png)

# 10.Create a Channel
```
./network.sh createChannel
```
<br>
Creates a default channel (usually named mychannel) and joins the peers to it.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/9f61906eb0cc443b6ee8532eb70a9d704f61fd32/Screenshot%202025-04-16%20221613.png)
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/0b54ae74a55ca48f94d789423995b2e095c6b61f/Screenshot%202025-04-16%20221628.png)

# 11.Shut Down the Network
```
./network.sh down
```
<br>
Stops all containers and deletes the crypto material and artifacts created during the setup.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/9b5aa30f291f7f1ea68c4a86ac196971465f59e7/Screenshot%202025-04-16%20221651.png)





# Solidity

Step 1: Set Up the Development Environment
<br>

Website: https://remix.ethereum.org
<br>

It’s an online editor where you can write, test, and deploy Solidity code directly in your browser. No installation needed.

<br>
Step 2: Write Your First Smart Contract (in Solidity)



```
pragma solidity ^0.8.0;

contract HelloWorld {
    string public message = "Hello Blockchain!";

    function setMessage(string memory newMessage) public {
        message = newMessage;
    }
}
```




Step 3: Compile the Contract In Remix:
<br>

Click on the Solidity compiler tab (compiler icon).
<br>

Click Compile to check for errors.

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/92560e5cd5ca1bb7e9dc396a167071b2736e2d80/Screenshot%202025-05-18%20165643.png)


![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/147aeb72ed44701e8e23b96c314974b5d0242da6/Screenshot%202025-05-18%20165656.png)



Step 4: Deploy the Smart Contract Go to the Deploy & Run Transactions tab in Remix.
<br>

Choose Environment as "JavaScript VM" (for testing in browser).
<br>

Click Deploy.
<br>

After deployment, contract will appear in the Deployed Contracts section.
<br>

Step 5: Interact with the Contract Now you can:
<br>

Click message() to read the current message.
<br>

Use setMessage() to change the message.
<br>

This simulates how smart contracts work on blockchain.



# Q1 Create a voting system with multiple candidates. Each address can vote only once.

# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Voting {
    address public owner;
    mapping(address => bool) public hasVoted;
    mapping(string => uint256) public votes;
    string[] public candidates;
    bool public votingOpen;

    event Voted(address indexed voter, string candidate);
    event VotingStatusChanged(bool isOpen);

    modifier onlyOwner() {
        require(msg.sender == owner, "Only owner can call this function.");
        _;
    }

    modifier onlyWhileOpen() {
        require(votingOpen, "Voting is not open.");
        _;
    }

    constructor(string[] memory _candidates) {
        owner = msg.sender;
        candidates = _candidates;
        votingOpen = true;
    }

    function vote(string memory candidate) public onlyWhileOpen {
        require(!hasVoted[msg.sender], "You have already voted.");
        require(isValidCandidate(candidate), "Invalid candidate.");

        hasVoted[msg.sender] = true;
        votes[candidate] += 1;
        emit Voted(msg.sender, candidate);
    }

    function isValidCandidate(string memory candidate) internal view returns (bool) {
        for (uint256 i = 0; i < candidates.length; i++) {
            if (keccak256(abi.encodePacked(candidates[i])) == keccak256(abi.encodePacked(candidate))) {
                return true;
            }
        }
        return false;
    }

    function getCandidates() public view returns (string[] memory) {
        return candidates;
    }

    function getVotes(string memory candidate) public view returns (uint256) {
        require(isValidCandidate(candidate), "Invalid candidate.");
        return votes[candidate];
    }

    function changeVotingStatus(bool _status) public onlyOwner {
        votingOpen = _status;
        emit VotingStatusChanged(_status);
    }
}
```

# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8704ffac73fc388592e59c160b7124420bf39b80/Screenshot%202025-05-19%20140000.png)



# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/90cdb849160a4499d54f10d0995dcf5b208ad3da/Screenshot%202025-05-19%20140019.png)

# After Deploying we can see the green tick which show our contract is deployed on the blockchain

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/b04651fcbf6ceddfd53cb80882331766df8057ef/Screenshot%202025-05-19%20140144.png)



![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/fd839b0690e0ff928deb968865d1e780db44224d/Screenshot%202025-05-19%20140933.png)









