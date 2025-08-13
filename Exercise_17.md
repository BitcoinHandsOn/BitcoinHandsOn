---
layout: default
title: Exercise 17
---
# Exercise 17: Send bitcoin from Alice to Bob—review fees

In this exercise you’ll again send some bitcoin from Alice to Bob. Along the way and in the next exercise, we’ll look at fees in more detail. You want to minimize fees in your transactions, and the next exercises will teach you some fundamentals of bitcoin fees.

1.     Open both the Bob wallet and the Alice wallet.

2.     In the Bob wallet, click on the blue **Receive** button on the left. In the Label field, type in “receive from Alice”. Then go to the Address field, and copy it.

3.     In Alice, click on the **Send** button on the left. In the “Pay to” text box, paste the receive address that you just copied. In the Label, type “Send to Bob”. In the Amount field, enter about half the bitcoin you have in Alice.

4.     Now, let’s do some experimentation with fees and amounts to get a sense of how they work.

·       Go to the website [https://mempool.space/](https://mempool.space/) and look at what the estimated transaction fees are, on the bottom left. They range from No Priority to High Priority.

·       Back in Sparrow, take a look at the Fee field. What is the fee? By default, it appears that Sparrow tries to set the fee amount to get your transaction in the “High” or “Medium” priority range. Sparrow is receiving information about the current bitcoin market rate fees from mempool.space, in order to make these recommendations.

·       Change the transaction amount, make it as low as possible. Does Sparrow allow you to spend more on the fee, than you do on the transaction?

·       There’s a slider going from 1 to 50+, to the right of the label **Blocks**. Sparrow often starts out with a setting of 4 blocks—in other words, it sets a transaction fee that’s as low as possible, while still getting the transaction in the blockchain sometime within the next 4 blocks (approximately 40 minutes).

5.     Experiment with this slider. Unless fees are already very low, try moving it to the right, so that it takes longer, but the fees are lower. Only do this for transactions that are not urgent.

6.     After these experiments, you’re ready to actually create the transaction. But first, switch the Amount back to the original amount (about half of what you have in Alice).  
In the bottom right corner, click **Create Transaction**. Then click **Finalize Transaction for Signing**, and then **Sign** button. By clicking Sign, you’re authorizing the transaction, with your private key.

7.     Now click the **Broadcast Transaction** button. You’ve just sent the transaction to the bitcoin mempool. You’ll get the same pop-up messages that you’ve received before in Sparrow, when sending a transaction.

8.     Check the latest transactions in the Transactions window, in both the Alice wallet and the Bob wallet. You should see the transaction you just made, in both wallets. They will be in light gray instead of black, until they’re confirmed.

**Learn more: Amounts too small to usefully spend—“dust”**

In Step 4, you experimented with lowering the transaction amount—did you notice Sparrow lets you spend more on fees than the actual transaction amount? While possible, you should generally avoid this.

Amounts too small to spend economically are called “dust”. Dust happens when leftover Bitcoin (UTXOs) becomes worthless to move, because the fees exceed the value. It’s like packaging up and mailing a penny, but spending $1 on postage. Whether or not a chunk of bitcoin is “dust” depends on how high transaction fees are at the time.

If you're interested, consider exploring this topic online (search for UTXO and dust).