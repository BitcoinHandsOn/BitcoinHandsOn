---
layout: default
title: Exercise 7
---
# Exercise 7: Your first send—transfer bitcoin from Alice to Bob

In this exercise, you’ll practice sending bitcoin from the Alice wallet to the Bob wallet. In other words, you’re simulating Alice sending some bitcoin to Bob.

The main thing that would be different if there were really two separate people involved, is transferring the receive address. Instead of being a simple copy/paste of a receive address between two wallets on your computer, it would involve transferring the receive address between 2 different people. You could do this with an email, but more private options like a QR code would be better.

1.     Make sure the Alice and Bob wallets are open in Sparrow. You can close the Alice Recovery wallet.

2.     In the Bob wallet, click on the blue **Receive** button on the left. In the Label field, type in “receive from Alice”. Then go to the Address field, and copy the address to the clipboard.

3.     In Alice, click on the blue **Send** button on the left. In the “Pay to:” text box, paste the receive address from Bob. Enter “send to Bob” in the Label field.  
Remember, don’t skip the label! In following exercises you’ll need them.

4.     Still in the Alice wallet, in the Amount field, enter about half of the sats that you have in Alice.  
If you don’t remember how many sats are in Alice, an easy way to do that is to click the Max button to the right of the amount. Then, divide that in half. It’s best for privacy to not send a rounded amount—for instance, instead of 25,000 sats, send 24,359. Sparrow recommends this for privacy.

5.     For now, we’ll leave the Fee set to the default.  
(You’ll learn more later, but for now, just know that the fee is what the miners receive, for running their specialized computers to process bitcoin transactions. By default, Sparrow will suggest the fee amount that gets the transaction processed into the next block. A lower fee will often still get processed, but won’t necessarily get into the next block.)

6.     In the bottom right corner, click **Create Transaction**. Sparrow will pop up a Transaction window, with details of the transaction. We don’t need to go through all the details right now.

7.     Click **Finalize Transaction for Signing**, then **Sign**. When you sign a transaction, you’re using your private key to authorize it with a digital signature. Sparrow has access to the private key because you’re using a software wallet, and the private key (derived from the seed phrase) is stored with it.

8.     Now click the **Broadcast Transaction** button. This is the last step, and sends the fully signed transaction out to the Bitcoin mempool.  
(Is the Broadcast Transaction button missing? Check the troubleshooting section below.)

After you click the Broadcast Transaction button, you should quickly see 2 notifications pop up on the top right corner of your screen. One will show a debit for the Alice wallet, because we sent bitcoin out of it. The other will show a credit for the Bob wallet, because it received the bitcoin. This first pop-up is just to show that the transaction has been received into the mempool. It doesn’t mean it’s been confirmed, that’ll come in about 10 minutes.

### Troubleshooting: Broadcast Transaction button isn’t visible

After you sign the transaction, the next thing you should see is a Broadcast Transaction button. If you don’t see that, your connection may have been lost.

Check the slider at the very bottom right corner in Sparrow. If it's gray, you have lost your connection. This can happen sometimes, especially after restarting.

To fix this, click on the slider to reconnect.

### Learn more: addresses

Bitcoin receive addresses are unique identifiers (strings of letters and numbers) that bitcoin can be sent to, by anyone. One private key has many different addresses. Addresses should never be reused, because that makes your transactions much less private.

In Sparrow, in the Bob wallet, click on the blue Addresses button on the left. Notice that you don’t have just one section for addresses.

Instead, you have two sections for addresses, the Receive and the Change addresses, and they both have multiple addresses. And that’s not all—there’s essentially an unlimited number of addresses that can be generated, via some complex math, by the extended private key, which is represented by your seed phrase.

The **receive address** in Bitcoin is an address that’s designed for incoming transactions.

The **change address**, on the other hand, is specifically set up for when you send bitcoin, and then receive change back from the transaction. Because of some of the internals of bitcoin, you almost always send a larger amount than what you want to spend. It comes back as “change”, to one of the change addresses in your wallet.

It’s like paying for a $1 pack of gum with a $100 bill, and receiving $99 dollars back in change.

Almost all of your addresses in Bob are unused right now, except for

·       the one used for the first receive into the Alice wallet

·       one or more change addresses, that happen as a result of your first send in this exercise

Exercise 8: Review the Alice to Bob transaction

Let’s review the transaction you just made.

1.     In the Bob wallet, click on the blue **Transactions** button on the left. There is a Balance at the top of the Transactions. You can see the total either in Bitcoin or sats. (A sat is a fraction of a bitcoin, each 1 bitcoin has 100 million sats.)

2.     Your transaction may not have any confirmations yet. As it gets confirmations, the circle next to the Value begins to fill in. When it gets 6 confirmations (in about one hour) it will be considered “final settlement”, and the text for the transaction will switch from gray to black.

3.     To the right of the Balance label, **click** **on the actual number amount**. Notice that the numbers switch, from sats to BTC and back. My preference is to see the balance in sats, because it’s easier to read small amounts. The transaction you just made will be at the top.

4.     You also see the transaction amount in USD (or whatever you have set up as the currency in the Settings menu).

5.     Open the Alice wallet and click on the blue Transactions button. Again, the transaction you just made will be at the top. But it will not show the exact amount that you sent in sats. Instead it will show more. You spent more from Alice than what Bob received. The difference is the fee you paid, to get the transaction processed.  
How much was the fee for this transaction?

6.     Still in the Alice wallet, hover your cursor on the transaction date/time of the transaction you just made. There will be a little magnifying glass to the right. **Click on the magnifying glass**, to pop up transaction details.

·       This screen is similar to what you saw in the previous exercise, when you were creating the transaction. But now you’ll see a Blockchain section at the bottom. (This is visible once the transaction has at least one confirmation).

·       The Blockchain section shows you the status of the transaction, how many confirmations there are, and also some information about the block containing your transaction—the block height, and timestamp.  
Also, below the Blockchain section you see a section with a lot of colored numbers and letters, which is how the transaction appears in the blockchain. You can ignore it.

### Learn more: permissionless transactions

You control both the Alice and Bob wallet, so sending a transaction between them is just sending to yourself. But you could just as easily have sent bitcoin to a wallet owned by someone else. It would have been the exact same process.

There are only four things you need to make bitcoin transactions to any corner of the globe.

·       Bitcoin that you truly own, and have the private key for

·       Bitcoin wallet software

·       An internet connection

·       The bitcoin address you want to send to

If you have these things, you can send bitcoin to anyone, anywhere, anytime. The Bitcoin network is running 24/7.

One of the most important benefits of bitcoin is that no permission is needed, in order to make transactions. Bitcoin is what’s called a “bearer asset”. Whoever actually owns the bitcoin (in other words, has the seed phrase/private key) can spend them, with no intermediaries like government, banks or any other financial institution. In this way it’s similar to cash or gold bars.

Government currencies like the US dollar—often called fiat currencies—are tightly regulated. With government currencies, there are many ways that you could be blocked from accessing your own money. For example, during protests like the Canadian Truckers Protest, some protesters, or those people who wanted to donate to protesters, found their bank accounts frozen or restricted.

Also, transactions between different countries are frequently controlled. These types of regulations are called capital controls. If there’s a way for access to your money to be blocked, it’ll probably happen at some point. Capital controls and events like the Canadian Truckers Protest of 2022 have demonstrated that the only assets that _truly_ belong to you, are the ones that you control.

Luckily, there’s Bitcoin. And with Bitcoin, it’s impossible for someone to prevent you from accessing and spending your bitcoin—assuming you control your private keys.