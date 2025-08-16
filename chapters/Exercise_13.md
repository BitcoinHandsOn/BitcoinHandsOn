---
layout: default
title: Exercise 13
---
# Exercise 13: Use the Alice Watch Only wallet to send a transaction

In this exercise, you’ll explore what happens when you try to actually send a transaction, using the Alice Watch Only wallet. This will deepen your understanding of the situations in which you might choose to use watch only wallets.

1.     Make sure the Alice wallet is closed.  (If you don’t close it, this exercise won’t show the expected results.)

2.     Make sure the Alice Watch Only and Bob wallets are open.

3.     In the Bob wallet, click on the blue **Receive** button on the left, and copy the Address that’s shown.

4.     Switch to the Alice Watch Only wallet, and click on **Send** on the left. In the Pay to field, paste the receive address you got from the Bob wallet. Also add an amount—make it about half of what’s currently in Alice. For Label, type in “Send via Alice Watch Only”.

5.     Click **Create Transaction** at the bottom right, then **Finalize Transaction for Signing**.

6.     Now click **Sign**. What happens?

If you’ve done all the previous steps, Sparrow will pop up this message “Connect Hardware Wallet”.

Here’s why this is happening. Sparrow is not able to provide signing authority for the Alice Watch Only wallet, because it doesn’t have the private key for it, since it’s a watch only wallet. Often, to provide a private key to send from a watch only wallet, you would connect a hardware wallet.

For a watch only wallet, Sparrow only has the public key, from which it can look up the addresses associated with that key. But it cannot sign any transactions to send from those addresses.

### Try again

Now, try the exact same process, using the same steps above, with one change—make sure the Alice wallet is _open_, instead of closed.

Notice that when you’re on the screen that has the “Finalize Transaction for Signing” button, there’s a “Signing Wallet” dropdown, just above the button. Sparrow has determined that the Alice wallet has signing authority, and makes it the default signing wallet, even if you created the transaction from the watch only wallet.

Now, after you click Sign, Sparrow _does_ allow you to sign. If you choose to, you can continue and actually click **Broadcast Transaction** to complete the transaction. Even though the transaction was started from Alice Watch Only—as long as the Alice wallet is open in Sparrow, it will be used to do the signing.