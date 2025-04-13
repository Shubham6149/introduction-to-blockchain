# introduction-to-blockchain
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





# Hyperledger Fabric Practical
1. Install Golang
 <br>

```

sudo apt install golang-go
```

<br>
Installs Golang, which is necessary for running Hyperledger Fabric binaries.
<br>

Screenshot
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/e38de3438849018b3853100088275a071ea9990d/Screenshot%202025-04-13%20143125.png)

2. Check Docker Version
```
docker --version
```
<br>
Verifies that Docker is installed and running correctly.
<br>

Screenshot
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/a51ddc26719a0b9bdd0b5ba355acdeb0cc93c2d8/Screenshot%202025-04-13%20143202.png)

3.Check Docker Compose Version
```
docker compose version
```
<br>
Verifies the installation of Docker Compose.
<br>

Screenshot
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/734e23a30bd221490c1f90a5a74c6a59b6d57fa8/Screenshot%202025-04-13%20143214.png)

4.List Files in Current Directory
```
ls
```
<br>
Shows the list of files and folders in the current directory.

5.Clone the Fabric Samples Repository and Move into the Cloned Folder
```
git clone https://github.com/Akshitakaushik123/fabric-samples.git; cd fabric-samples
```
<br>
Downloads the official Hyperledger Fabric sample code from GitHub. Enters the cloned folder where Fabric examples are available.
<br>
Screenshot

6.Download Fabric Binaries
```
curl -sSL https://bit.ly/2ysbOFE | bash -s
```
<br>
Downloads necessary Fabric binaries and Docker images like peer, orderer, and cryptogen.
<br>
Screenshot

7.Enter the Test Network Directory
```
cd test-network
```
<br>
Navigates to the directory that contains scripts for running a sample Fabric network.
<br>
Screenshot

8.View the Network Script
```
./network.sh
```
<br>
Shows the options available with the network.sh script.
<br>
Screenshot

9.Start the Fabric Network
```
./network.sh up
```
<br>
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.
<br>
Screenshot

10.Create a Channel
```
./network.sh createChannel
```
<br>
Creates a default channel (usually named mychannel) and joins the peers to it.
<br>
Screenshot


11.Shut Down the Network
```
./network.sh down
```
<br>
Stops all containers and deletes the crypto material and artifacts created during the setup.
<br>
Screenshot








