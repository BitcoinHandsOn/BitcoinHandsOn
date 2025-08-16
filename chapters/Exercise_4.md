---
layout: default
title: Exercise 4
---
# Exercise 4: Receive bitcoin into your Alice wallet

In this exercise, you’ll actually receive bitcoin into your wallet. The procedure will be a little different on each exchange. Some exchanges may even require you to get approval for the receive address.

But basically, it will involve steps similar to this:

·       Open up the website or app for your exchange (where you bought the bitcoin), and navigate to where you can send bitcoin out of the exchange.

·       Enter a bitcoin address. (This will be a receive address that you get from the Alice wallet).

·       Decide how much you want to send. It’s easier to think of bitcoin amounts in terms of sats, because 1 bitcoin is now very expensive. (Sats is short for Satoshis. One whole bitcoin equals 100 million sats.)

·       Enter the amount of sats you want to send to the Alice receive address.

·       Decide on the amount of fees you’re willing to pay. Some exchanges may offer free transaction fees.

·       Hit the send button, and wait for the bitcoin to arrive in your wallet.

### Example: Using Strike to receive bitcoin

These are what the steps look like when sending bitcoin from Strike, the KYC exchange that I mentioned above. Remember, the process in the exchange that you use will be different. Using Strike (which is a mobile app on your phone), it’s easiest to use QR codes to get the bitcoin receive address, instead of copying and pasting the address.

1.     In Sparrow, open up the Alice wallet file. Click on the blue **Receive** button on the left. Your wallet has many, many receive addresses, and Sparrow will show you the first available address.

2.     Label the receive address. I wrote “Receive from Strike” in the label. When using the defaults in Sparrow, all bitcoin addresses start with bc1. The QR code for the address, which I’ll use in the next step, is to the right of the address.  
Don’t skip the label! Some of the following exercises depend on having labels.

3.     In the Strike app, I click the Bitcoin icon at the bottom left. I scroll to the Send screen, and click Bitcoin wallet.  
Then I go back to Sparrow on my computer, where the Receive window is still open. I use Strike on my phone to scan the Sparrow QR code for the receive address.

4.     In Strike, I enter the amount of sats that I want to send (about half of what I purchased).

5.     Next is the fee. I could either pay a larger fee, to have the transaction go through in the next 10 minutes, a medium fee to send it in the next hour, or zero, to have it go through in the next 24 hours.  
I chose to pay the higher fee, and have it go through within about 10 minutes. Other exchanges will have different options for fees.

6.     On the next screen I review the details (amount, receive address), before clicking to confirm the transaction.

If the exchange you’re using is a desktop application, and not a mobile app, you’ll need to copy and paste the bitcoin address, instead of using a QR code.

### Monitoring the receive into Alice

You will now receive the bitcoin into your Alice wallet, in Sparrow. No matter where the bitcoin originally came from, here’s what you should see as the transaction goes through.

If you’ve chosen to pay a higher fee for a quicker transaction, it’ll all happen within about 10 minutes. Otherwise it will take longer.

1.     The first step is that you get a pop-up notice in the top right corner, in Sparrow. It’ll have a message entitled “New mempool transaction”, and the amount of the transaction. These Sparrow notifications disappear after a few seconds.  
That means your transaction is in the mempool. (See the below section “Learn more: Mempool and Blockchain” for more info.)

2.     Once you’ve gotten the pop-up notice in your Alice wallet, click on the blue **Transactions** button on the left. You should have one transaction in there, from the transaction you just made. The transaction will show up in light gray at first.

3.     You’ll receive another pop-up notification in Sparrow when the first confirmation occurs, which is usually in about 10 minutes. Six confirmations is usually considered final, and then the transaction in Sparrow will switch from light gray to black.

4.     Notice that in the Transactions window, there’s a US dollar amount in there. For the dollar amount, the current bitcoin price is used. (To set up a different default currency, go to File > Settings > Currency.)

Congratulations! You now truly own some bitcoin, it’s on your own personal wallet, and you have the private key.

### Troubleshooting your connection in Sparrow

This was also mentioned in Exercise 1, but here’s a reminder, because it happens often.  You may notice that a transaction doesn't show up when it should. If this happens, check the slider at the very bottom right corner in Sparrow. If it's gray, you have lost your connection. This can happen sometimes, especially after restarting.

To fix this, click on the slider to reconnect.

### Learn more: Mempool and blockchain

The mempool is a holding area for bitcoin transactions that have been submitted, but not yet added to a block. It’s like bitcoin’s waiting room—an area where transactions sit before being included in a block. When you send bitcoin, your transaction joins others in the mempool, waiting for bitcoin miners to pick them up.

After a miner picks them up and confirms them in a new block, the block gets added to the bitcoin blockchain. This means that the transaction has one confirmation. When another block gets added to the blockchain, your transaction will have two confirmations. Once it has six confirmations, most people consider that “final settlement”—in other words, it’s almost impossible to reverse.

What is the blockchain? It’s like a giant public notebook, or ledger, of all the transactions that have ever occurred. By looking at the blockchain, you can see exactly what the transactions were, the amounts of the transactions, and the sending and receiving address.

You pay a fee, called the transaction fee, for having your transaction included in the next block, and added to the blockchain. This can be higher or lower, depending on how much competition there is for transaction space in the bitcoin blockchain. Transactions that include higher fees usually get chosen first by the miners, and go into the very next block. Lower-fee transactions wait longer. We’ll discuss fees in more detail later.

### Learn more: bitcoin mining

Just now, in the section on Mempool and blockchain, the term bitcoin miners came up. What is, actually, the process of bitcoin mining?

Basically, bitcoin mining happens with a decentralized network of special computers (“miners”), all around the world. These miners are competing to solve a mathematical problem, every 10 minutes. Whichever computer finds the solution first gets to “mine” the next block of transactions, which means linking the new block to the previous one in the blockchain.

Bitcoin mining takes special, expensive computers, and lots of electricity. The reason that the miners do this work is that they earn bitcoin in two different ways, each time they mine a block.

·       First, there’s a reward in bitcoin, for the computer that mines that block. This reward is substantial. In 2025, each mined block earns 3.125 bitcoin.

·       Also, the successful miner gets to keep the transaction fees associated with the block.

The reward in bitcoin for the successful miner is straightforward, it’s just a set amount.

The transaction fees are more complex. Every single transaction needs to pay a fee, to pay for the work of putting it in the block. And transaction fees depend on how busy the network is. If many people are trying to make transactions, fees go up because there’s more competition for a scarce resource—space on the bitcoin blockchain.

It’s similar to when a city is hosting the Olympics. Hotel rooms will get much more expensive because there’s only a set amount of them. Similarly, you will have to pay more in transaction fees when the bitcoin network is congested.

Luckily, it’s now (in 2025) a period of relatively low fees, so the transactions you’ll be making in these exercises will be relatively inexpensive.