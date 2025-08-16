---
layout: default
title: Exercise 12
---
# Exercise 12: Receive bitcoin via a watch only wallet

Getting receive addresses is one of the most important uses of a watch only wallet. This exercise demonstrates how to receive bitcoin to a wallet, without even having it open (and potentially exposed).

In order to do this, we use a watch only wallet.

1.     In Sparrow, open the Bob wallet, and the Alice Watch Only wallet. Close all other wallets, especially the Alice wallet.

2.     Go to the Alice Watch Only wallet. Click on the blue **Receive** button on the left. For the Label field, type in “Send from Bob to Alice Watch Only”. And now, copy the contents of the Address field.

3.     Now switch to the Bob wallet, and click the blue **Send** button on the left. Into the Pay to field, paste the address you just copied from Alice Watch Only. Type the same text in the Label, “Send from Bob to Alice Watch Only”.

4.     In Amount, enter the number of sats that you’ll be sending to Alice Watch Only—about half of your balance.

5.     Click **Create Transaction** on the bottom right. On the next screen, click **Finalize Transaction for Signing.**

6.     Now click **Sign**, in the bottom right corner. Then click **Broadcast Transaction**. Remember, if the Broadcast Transaction button is not visible, you may need to reconnect with the slider at the very bottom right.

This sends the transaction that you just created to the bitcoin mempool. Because you have the two wallets that are involved in this transaction open, you’ll get two pop-up notices from Sparrow. One will have a negative amount for the Bob wallet, the other will have a positive amount for the Alice Watch Only wallet.

From there, the transaction will soon get added to a block, and be incorporated into the blockchain. You’ll receive two more notices (one for each open wallet) when the first confirmation happens, usually in around 10 minutes.

### Learn more: Receive addresses from watch only wallets

Getting receive addresses via a watch only wallet is very common. For instance, say that somebody wants to pay you in bitcoin. If you have your watch only wallet set up, you can give them a receive address, using _only_ the watch only wallet. You may want to do this because as you acquire more bitcoin, you’ll set up your wallet much more securely than your current wallets. You may have it hidden away somewhere, or in a safe.

In general, you want to keep your bitcoin wallets secure, and that means not opening them frequently. A watch only wallet, set up with the public key of your main wallet, can prevent you from needing to open your wallet just for a receive address.

Of course, before relying on a watch only wallet like this, make sure that the watch only wallet is set up correctly. It’s important to check that the receive addresses are identical to the original wallet.