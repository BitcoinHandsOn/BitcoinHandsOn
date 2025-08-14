---
layout: default
title: Exercise 26
---
# Exercise 26: Send all bitcoin from the Bob Recovery wallet in Blue Wallet to Alice in Sparrow

Once you’ve created your recovery wallet, what’s the next step?

Your next step would be to test it, to make sure you can actually spend from it. After all, that’s the moment of truth—if everything was done correctly, you can send bitcoin from your recovery wallet.

So in this exercise, you will send bitcoin from the Bob Recovery wallet (in Blue Wallet) to the Alice wallet, in Sparrow.

You’ll send _all_ the bitcoin in this step, because we’re nearing the end of the book, and you don’t necessarily want to have bitcoin scattered across different wallets.

1.     Open Sparrow. Open the Alice wallet, and click the blue **Receive** button on the left, to bring up a receive address. You’ll be using the QR code, to transfer the receive address to Blue Wallet.

2.     In Blue Wallet, open the Bob Recovery wallet. At the bottom of the screen, click **Send**. On the Send screen, click **Scan** to the right of the address, to bring up the camera.

3.     Use Blue Wallet on your phone to scan the receive address in Sparrow. It should populate the address field, to the left of the Scan button.

4.     In Blue Wallet on your phone, instead of entering the amount of sats to send, click on the three dots at the top right corner. Then click on the option **Use Full Balance**. Blue Wallet will ask you to confirm.

5.     The default fee in Blue Wallet is set to get your transaction into the next block. You can click on it, to adjust the fee. I lowered mine to 2 sats/vB, because fees were low in general, and I thought it would still go through quickly enough.

6.     Enter in the Note to Self field: “**send to Alice in Sparrow**”, and click **Next.** On the next screen, click **Send now**.

After you hit Send now, you’ll see that in Blue Wallet, in the main screen, you have a pending transaction. It shows with the amount you sent, plus the fee, and starts out as Pending, because it hasn’t yet been confirmed.

Whenever the transaction gets confirmed, you’ll see the “Pending” disappear in Blue Wallet. Also, it will now show up with a confirmation in the Alice wallet in Sparrow.

### Learn more: recovery after a potential seed phrase theft

What would you need to do in a real emergency recovery? For instance, in a situation where your laptop has been stolen, and you had Sparrow set up on that laptop, with a “hot” software wallet on it?

If the thief understood bitcoin, and knew you had Sparrow installed with a software wallet, you might be out of luck. The thief would probably have instantly sent all the bitcoin from your wallet to a different wallet, one that he controls.

In case the thief didn’t know these details, you may have more time. However, you still need to move your bitcoin. You need to send the entire amount from your old wallet, with the old seed phrase, to a new wallet with a new seed phrase. Moving all the funds from one bitcoin wallet to another is called “sweeping”.

Note that if you do this, you will lose all the labels for your transactions and addresses, because they’re saved in the Sparrow wallet file, not on the blockchain. This can be a serious issue, because knowing where your sats came from (through the labels) can be important for privacy. If you’d like to learn more, read up on the topic of “coin control in bitcoin”.