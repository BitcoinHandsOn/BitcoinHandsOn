---
layout: default
title: Exercise 16
---
# Exercise 16: Review some transactions

In this exercise we’ll be reviewing some of the transactions that have occurred, and learning more about how transactions work. You don’t need to know every single detail on this topic, this is just to get an overview.

Understanding how transactions work will give you a better grasp of how to begin optimizing for lower fees and privacy.

### Review your initial transaction into the Alice wallet

Let’s take a more detailed look at the very first transaction that you made, when you received your first bitcoin into the Alice wallet.

1.     In Sparrow, open the Alice wallet. Click on the blue **Transactions button** on the top left in Sparrow. Go to your earliest transaction.

2.     Hover your cursor over the date of that transaction, and a little magnifying glass will pop up on the right. Click on the **magnifying glass** to view details about the transaction.

3.     The fee is at the bottom. The fee is what’s left after the recipients have been paid, and the change has gone back to the change address. The fee goes to the bitcoin miners.

4.     If you purchased the bitcoin from an exchange, it can look somewhat complex. It’s likely that there will be one input (from your exchange), and many outputs, as the exchange splits the payments to many different people’s addresses.  
One of these outputs is the one you received, into your address. Your output has a downward pointing arrow icon, the others have what looks like a paper airplane.

### Explore an address in Mempool.space

Now you’re going to use the blockchain explorer [https://mempool.space](https://mempool.space/) to view transactions. What exactly is a blockchain explorer? It’s a website that allows users to view everything that’s available on the bitcoin blockchain, like transactions, addresses, etc. Mempool.space is the most well-known bitcoin blockchain explorer. Another blockchain explorer is Blockstream.info.

This exercise helps you gain a fresh perspective on blockchain data. By reviewing transactions through a tool other than Sparrow, you develop a clearer understanding of the blockchain. It reinforces the idea that the transactions you’re seeing are part of a global network powered by tens of thousands of bitcoin nodes, all working together to maintain the blockchain network’s stability.

1.     Go to Sparrow, where you have the transaction open for the very first bitcoin you received into Alice. Go to your receive address (the one with a downward pointing arrow icon). Right-click (or Control-click on a Mac), and then click on **Copy Address**

2.     Now in a browser, go to [https://mempool.space/](https://mempool.space/). In the top right, where it says Explore the full Bitcoin ecosystem, **paste in the Address** you just copied. Click the **magnifying glass** to the right, to run the search.

3.     You’ll see a screen full of information about your receive address. It has the current balance, which may not be the same as the original one. You may see more than one transaction, related to this bitcoin address.

4.     Under the Address section, there will be a Transactions section. It will probably say **2 of 2 Transactions**. Click on the **Transaction ID** that’s the same as the TXID you saw earlier in Sparrow. This should also be the _earliest_ transaction for that address.

5.     In Mempool.space **find the number of confirmations** for that transaction. This should be identical to what you see for the same transaction, in Sparrow. The Block (called Block Height in Sparrow, the number of the block that the transaction got into) should also be the same between Mempool.space and Sparrow.  
The timestamp may not be identical, because of time zone differences.

6.     Scroll down in Mempool.space to the Flow section. This is where you get a comprehensive layout of the entire transaction, with all inputs, all outputs, and fees. Your address will be among the outputs.

7.     Notice that you can see, in the Flow section, any additional transactions that your address (and other addresses that were in the transaction) were involved in.

### Learn more: Never reuse bitcoin addresses

As you saw in the exercise above, it’s simple to track bitcoin, if you know the bitcoin address. The fact that no history is lost in the bitcoin blockchain is another reason to be careful about your privacy. One of the ways to improve your privacy in bitcoin is to never use a bitcoin address more than once.

Never reuse bitcoin addresses

If someone happens to know one of your bitcoin addresses, and if you use that address again and again, they know exactly how much bitcoin you have in it. They also know when you received it, and how much you received in each transaction.

Fortunately, most modern bitcoin wallet software makes it difficult to reuse a bitcoin address. For instance, in Sparrow, when you click Receive, you are given a new receive address, and not one that you’ve used before.

### Learn more: Expanding on the Blockchain

In a previous exercise, you learned some of the essentials about the bitcoin blockchain. It’s basically a public ledger, stored and duplicated on an enormous, decentralized network of computers running bitcoin software, all around the world. It records every single bitcoin transaction that has ever taken place, in chronological order. In it you can see all the addresses in the transactions, and the amount of bitcoin associated with each address. And also, it’s completely open to the public—if you had a spare computer, you could run a bitcoin node in your home.

About every 10 minutes on the blockchain, a new block is added on top of the last block. This has been happening with almost 100% reliability ever since bitcoin was first started up in January 2009. When a new block is created and attached to the bitcoin blockchain, it’s like a new link on a metal chain—the new block is attached to the previous block via a mathematical fingerprint.

There’s a popular saying among bitcoiners, “Tick tock, next block”

Tick tock, next block

This saying captures the mindset of bitcoiners. The price might be up or down, but Bitcoin will keep on going. And it will gradually but steadily replace other types of money. No government or corporation in the world can stop bitcoin from being transacted, and new blocks from being added to the blockchain.