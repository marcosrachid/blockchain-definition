# Blockchain Documentation

* [1. Structure](#structure)
* [2. Keys](#keys)
* [3. Where is blockchain ?](#where-is-blockchain-)
* [4. "Proof of" concepts](#proof-of-concepts)

## 1. Structure

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

The above equation is a polynomial equation, that mean x can be n different numbers (if assume that the equation has no repeated number), the riddle is to find a one of these numbers to create a block within the network consensus. It's a hard riddle to solve, but an easy riddle to validate.

The new block will be created and signed to the solver's **Private Key**

## 2. Keys

There are two types of keys in the Blockchain environment:

* **Private Key**: Is a cryptographic hash used to sign transactions on blockchain. As the name says it's private to only the owner knowledge, if the owner loses the private key, he will lose access to tokens and smart contracts.

* **Public key**: Derived from the private key and is used to verify transactions, a public key cannot return a private key.

* **Adresses**: Dereived from public key, represents your wallet address containing your tokens.

## 3. Where is blockchain ?

Blockchain is a massive distributed database, saved in every computer, so from now on, you are responsible for holding your account (private key) and your own token.

The blockchain are accessible from clients like **GoEthereum**, **Paraity**, **Ethereum++** and others, starting a client, it begins to download the whole blockchain to your computer. In resume, there is no server side storage.

## 4. "Proof of" concepts

There are three existing concepts till now:

* **Proof of Work**(PoW): Need to put a lot of effort to mine new blocks (eletricity, power and money), the currently problem is that sacrificies a lot of network making a slow environment. (3-10 transactions/s)

* **Proof of Stake**(PoS): You need to put ether where you stake to mine/forge blocks.

* **Delegated Proof of Stake**(DPoS): The stake is voted on fair and democratic way, then the staker is allowed to mine/forge new blocks.
