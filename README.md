# Blockchain Documentation

## Structure

<div align="center" style="float: left">
  <img alt="Blockchain Strucutre" width="250" src="https://github.com/marcosrachid/blockchain-definition/blob/master/public/Blockchain_Structure.png" />
</div>

* Block 0: Genesis block, configurable by genesis.json file
* Block 1: Contain transactions and part of hash key signature from block 0
* Block 2: Contain transactions and part of hash key signature from block 1
* Block 3: Contain transactions and part of hash key signature from block 2
* Block n: Contain transactions and part of hash key signature from block n - 1

The ways to create new blocks depends on the **Proof of** concept blockchain is using. The most famous concept that is being used by bitcoin and ethereum is **Proof of Work**, that the miner must solve a **mathematical riddle** to find a valid block. Ex:

<div align="center" style="float: left">
  <img alt="Mathematical Riddle" src="https://github.com/marcosrachid/blockchain-definition/blob/master/public/equation.svg" />
</div>

The above equation is a polynomial equation, that mean x can be n different numbers (if assume that there is no repeated number), the riddle is to find a one of these numbers to create a block within the network consensus.
