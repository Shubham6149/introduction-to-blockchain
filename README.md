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

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8b945277507cdb260b5077bb727f56ebbf6f74b6/Screenshot%202025-04-16%20220330.png)

2. Check Docker Version
```
docker --version
```
<br>
Verifies that Docker is installed and running correctly.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/60995a7ce104d527d0fef2112a50ab0ea0baaa4b/Screenshot%202025-04-16%20220342.png)

3.Check Docker Compose Version
```
docker compose version
```
<br>
Verifies the installation of Docker Compose.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/a1e87e4b0f7abf24eb6de9a8a150b1cce67de2e5/Screenshot%202025-04-16%20220352.png)

4.List Files in Current Directory
```
ls
```
<br>
Shows the list of files and folders in the current directory.


5.Clone the Fabric Samples Repository and Move into the Cloned Folder
```
git clone -b main https://github.com/hyperledger/fabric-samples.git
```
<br>
Downloads the official Hyperledger Fabric sample code from GitHub. Enters the cloned folder where Fabric examples are available.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/da5fcfde196a72065455d0d042c854ff7fe6c401/Screenshot%202025-04-16%20220408.png)

6.Download Fabric Binaries
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
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/06274ff129fbb8833dfb4d70e7af24e23f9ed336/Screenshot%202025-04-13%20143339.png)

7.Enter the Test Network Directory
```
cd test-network
```
<br>
Navigates to the directory that contains scripts for running a sample Fabric network.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/6135b4d97defaf4ffc4fe124fa8fb0d40d71587c/Screenshot%202025-04-13%20143416.png)

8.View the Network Script
```
./network.sh
```
<br>
Shows the options available with the network.sh script.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8c17d5c5768067011c18c198eee4f174c3a153e8/Screenshot%202025-04-13%20143444.png)

9.Start the Fabric Network
```
./network.sh up
```
<br>
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/955425f88caa472c8df9ed3118ee7a485b7a3978/Screenshot%202025-04-13%20143454.png)

10.Create a Channel
```
./network.sh createChannel
```
<br>
Creates a default channel (usually named mychannel) and joins the peers to it.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/ed6c7d843c0dcd00ba27314a54ab6030aaa81e80/Screenshot%202025-04-13%20143507.png)

11.Shut Down the Network
```
./network.sh down
```
<br>
Stops all containers and deletes the crypto material and artifacts created during the setup.
<br>

# Screenshot
<br>

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/11188af1f5246f4e96a6298efee19276b75010b7/Screenshot%202025-04-13%20143529.png)







