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


![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/43e0b5f15b4cf7d9c8815cc9510441ba0ecaac1c/Screenshot%202025-05-19%20141827.png)



# After Deploying we can see the green tick which show our contract is deployed on the blockchain

![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/b04651fcbf6ceddfd53cb80882331766df8057ef/Screenshot%202025-05-19%20140144.png)



![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/fd839b0690e0ff928deb968865d1e780db44224d/Screenshot%202025-05-19%20140933.png)



# Q2 Write a contract that manages a list of student records (name, roll number). Allow adding and retrieving student data.

# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

/**
 * @title StudentRecords
 * @custom:dev-run-script ./scripts/deploy_student_records.js
 */
contract StudentRecords {
    struct Student {
        string name;
        uint256 rollNumber;
    }

    mapping(uint256 => Student) private students;
    uint256[] private rollNumbers;

    event StudentAdded(string name, uint256 rollNumber);

    modifier uniqueRollNumber(uint256 rollNumber) {
        require(bytes(students[rollNumber].name).length == 0, "Student already exists.");
        _;
    }

    function addStudent(string memory _name, uint256 _rollNumber) public uniqueRollNumber(_rollNumber) {
        students[_rollNumber] = Student(_name, _rollNumber);
        rollNumbers.push(_rollNumber);
        emit StudentAdded(_name, _rollNumber);
    }

    function getStudent(uint256 _rollNumber) public view returns (string memory name, uint256 rollNumber) {
        require(bytes(students[_rollNumber].name).length > 0, "Student not found.");
        Student memory student = students[_rollNumber];
        return (student.name, student.rollNumber);
    }

    function getAllRollNumbers() public view returns (uint256[] memory) {
        return rollNumbers;
    }

    function getStudentCount() public view returns (uint256) {
        return rollNumbers.length;
    }
}
```


# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/5aeb85e7e212072ee703a9b67ad39cb77d5e3761/Screenshot%202025-05-19%20143304.png)


# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/2ec0f7db75d0a501075251376e8be83c04a84256/Screenshot%202025-05-19%20143404.png)



# After Deploying we can see the green tick which show our contract is deployed on the blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/18b91c8830423ff20e57b5a0c9f31c9499c91045/Screenshot%202025-05-19%20143416.png)



# 3 Develop a contract that only allows the deployer (owner) to call a specific function (use modifiers).

# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

/**
 * @title OwnerOnly
 * @dev This contract allows only the deployer (owner) to call specific functions.
 * @custom:dev-run-script ./scripts/deploy_owner_only.js
 */
contract OwnerOnly {
    address public owner;

    modifier onlyOwner() {
        require(msg.sender == owner, "Only the owner can call this function.");
        _;
    }

    constructor() {
        owner = msg.sender;
    }

    function ownerOnlyFunction() public onlyOwner {
        // Logic that only the owner can execute
    }

    function publicFunction() public {
        // Logic that anyone can execute
    }

    function transferOwnership(address newOwner) public onlyOwner {
        require(newOwner != address(0), "New owner cannot be the zero address.");
        owner = newOwner;
    }
}
```

# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8a7233439e731e627a8b44707c9067065f1a4adb/Screenshot%202025-05-19%20144026.png)


# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/194a30957ba70541e5a55a7174f2c1d51089d30e/Screenshot%202025-05-19%20144041.png)



# After Deploying we can see the green tick which show our contract is deployed on the blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/1cdb7e55d7ceea3e8adb4ffe496a50d849f3fe0e/Screenshot%202025-05-19%20144050.png)




# 4 Write a contract where people can donate Ether and the top 3 donors are tracked.

# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

/**
 * @title TopDonors
 * @dev This contract allows people to donate Ether and tracks the top 3 donors.
 * @custom:dev-run-script ./scripts/deploy_top_donors.js
 */
contract TopDonors {
    struct Donor {
        address addr;
        uint256 amount;
    }

    // Array to store the top 3 donors
    Donor[3] public topDonors;

    // Event emitted when a donation is made
    event DonationReceived(address indexed donor, uint256 amount);
    event TopDonorsUpdated(address[3] addresses, uint256[3] amounts);

    // Function to donate Ether
    function donate() external payable {
        require(msg.value > 0, "Donation must be greater than zero.");

        // Emit the donation event
        emit DonationReceived(msg.sender, msg.value);

        // Update the top 3 donors
        updateTopDonors(msg.sender, msg.value);
    }

    // Internal function to update the top 3 donors list
    function updateTopDonors(address _donor, uint256 _amount) internal {
        for (uint256 i = 0; i < 3; i++) {
            if (topDonors[i].addr == _donor) {
                topDonors[i].amount += _amount;
                sortTopDonors();
                emitTopDonors();
                return;
            }
        }

        if (_amount > topDonors[2].amount) {
            topDonors[2] = Donor(_donor, _amount);
            sortTopDonors();
            emitTopDonors();
        }
    }

    // Sort the top donors by the amount in descending order
    function sortTopDonors() internal {
        for (uint256 i = 0; i < 3; i++) {
            for (uint256 j = i + 1; j < 3; j++) {
                if (topDonors[j].amount > topDonors[i].amount) {
                    Donor memory temp = topDonors[i];
                    topDonors[i] = topDonors[j];
                    topDonors[j] = temp;
                }
            }
        }
    }

    // Emit the top donors
    function emitTopDonors() internal {
        address[3] memory addresses;
        uint256[3] memory amounts;
        for (uint256 i = 0; i < 3; i++) {
            addresses[i] = topDonors[i].addr;
            amounts[i] = topDonors[i].amount;
        }
        emit TopDonorsUpdated(addresses, amounts);
    }

    // Public function to view the top 3 donors
    function getTopDonors() public view returns (address[3] memory, uint256[3] memory) {
        address[3] memory addresses;
        uint256[3] memory amounts;
        for (uint256 i = 0; i < 3; i++) {
            addresses[i] = topDonors[i].addr;
            amounts[i] = topDonors[i].amount;
        }
        return (addresses, amounts);
    }
}
```

# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/1a54cd74a4e73da1c6127d65b8d013fa88bbdd92/Screenshot%202025-05-19%20145615.png)



# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/8f99e0ce8d47904c9b20a29541ca71c0a0b02798/Screenshot%202025-05-19%20145626.png)


# After Deploying we can see the green tick which show our contract is deployed on the blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/38aa25e5b8fb0f5af6b13d1da16bea6f64c3b1c0/Screenshot%202025-05-19%20145658.png)



# 5 Implement a simple auction system where users can place bids, and the highest bidder wins.


# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

/**
 * @title SimpleAuction
 * @dev A simple auction contract where users can place bids, and the highest bidder wins.
 * @custom:dev-run-script ./scripts/deploy_simple_auction.js
 */
contract SimpleAuction {
    address public owner;
    uint256 public auctionEndTime;
    address public highestBidder;
    uint256 public highestBid;

    mapping(address => uint256) public pendingReturns;
    bool public ended;

    event AuctionStarted(uint256 duration);
    event HighestBidIncreased(address bidder, uint256 amount);
    event AuctionEnded(address winner, uint256 amount);

    modifier onlyOwner() {
        require(msg.sender == owner, "Only the owner can call this function.");
        _;
    }

    modifier auctionActive() {
        require(block.timestamp < auctionEndTime, "Auction already ended.");
        _;
    }

    modifier auctionEnded() {
        require(block.timestamp >= auctionEndTime, "Auction not yet ended.");
        require(!ended, "Auction end has already been called.");
        _;
    }

    constructor(uint256 _biddingTime) {
        owner = msg.sender;
        auctionEndTime = block.timestamp + _biddingTime;
        emit AuctionStarted(_biddingTime);
    }

    /// @dev Bid function where users place their bids
    function bid() external payable auctionActive {
        require(msg.value > highestBid, "There already is a higher bid.");

        if (highestBid != 0) {
            pendingReturns[highestBidder] += highestBid;
        }

        highestBidder = msg.sender;
        highestBid = msg.value;
        emit HighestBidIncreased(msg.sender, msg.value);
    }

    /// @dev Withdraw function to retrieve overbid funds
    function withdraw() external returns (bool) {
        uint256 amount = pendingReturns[msg.sender];
        require(amount > 0, "No funds to withdraw.");

        pendingReturns[msg.sender] = 0;

        if (!payable(msg.sender).send(amount)) {
            pendingReturns[msg.sender] = amount;
            return false;
        }
        return true;
    }

    /// @dev Ends the auction and sends the highest bid to the owner
    function endAuction() external onlyOwner auctionEnded {
        ended = true;
        emit AuctionEnded(highestBidder, highestBid);

        (bool success, ) = payable(owner).call{value: highestBid}("");
        require(success, "Transfer failed.");
    }
}
```

# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/4c9ad9c27c024a81883e195914190dae1ee30463/Screenshot%202025-05-19%20150611.png)



# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/7bbee02cbc47003d276df4d6a6d1bc75e0d96c2e/Screenshot%202025-05-19%20150703.png)


# After Deploying we can see the green tick which show our contract is deployed on the blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/f1ca610b535351b3d635eb85918f67b5f3a1688f/Screenshot%202025-05-19%20150716.png)




# 6 Create a contract that splits incoming Ether between 3 fixed addresses.

# code
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

/**
 * @title EtherSplitter
 * @dev This contract splits incoming Ether equally between three fixed addresses.
 * @custom:dev-run-script ./scripts/deploy_ether_splitter.js
 */
contract EtherSplitter {
    address payable public recipient1;
    address payable public recipient2;
    address payable public recipient3;

    event EtherReceived(address indexed sender, uint256 amount);
    event EtherSplit(uint256 amount1, uint256 amount2, uint256 amount3);

    /**
     * @dev Initializes the contract with three fixed addresses.
     * @param _recipient1 The first recipient address.
     * @param _recipient2 The second recipient address.
     * @param _recipient3 The third recipient address.
     */
    constructor(address payable _recipient1, address payable _recipient2, address payable _recipient3) {
        require(_recipient1 != address(0) && _recipient2 != address(0) && _recipient3 != address(0), "Invalid address");
        recipient1 = _recipient1;
        recipient2 = _recipient2;
        recipient3 = _recipient3;
    }

    /**
     * @dev Receive function to automatically split Ether upon reception.
     */
    receive() external payable {
        require(msg.value > 0, "No Ether sent");
        emit EtherReceived(msg.sender, msg.value);

        uint256 splitAmount = msg.value / 3;

        // Transfer the split amounts
        (bool sent1, ) = recipient1.call{value: splitAmount}("");
        require(sent1, "Transfer to recipient1 failed");

        (bool sent2, ) = recipient2.call{value: splitAmount}("");
        require(sent2, "Transfer to recipient2 failed");

        (bool sent3, ) = recipient3.call{value: msg.value - (2 * splitAmount)}("");
        require(sent3, "Transfer to recipient3 failed");

        emit EtherSplit(splitAmount, splitAmount, msg.value - (2 * splitAmount));
    }
}
```

# compiling the code
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/bf43cebaa9ab317e628a800509eb9bf482b2d959/Screenshot%202025-05-19%20151426.png)



# deploying on blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/484d30cf224fd408c1fdc0e4d5f3cb96bf58f030/Screenshot%202025-05-19%20151444.png)


# After Deploying we can see the green tick which show our contract is deployed on the blockchain
![image alt](https://github.com/Shubham6149/introduction-to-blockchain/blob/6418d149fd7bd472f84a305994ea1f5a4e85a15b/Screenshot%202025-05-19%20151454.png)











