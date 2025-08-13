---
layout: default
title: Exercise 11
---
# Exercise 11: Explore the Alice Watch Only wallet

In this exercise, we’ll explore the Alice Watch Only wallet, and compare it with the original Alice wallet.

1.     In Sparrow, open the newly created Alice Watch Only wallet, and also the original Alice wallet.

2.     In the Alice Watch Only wallet, click on the blue **Transactions** button on the left. You should see two transactions there. The first is when you received bitcoin from your original source. The second is from sending bitcoin from Alice to Bob.

3.     Look for labels in the Transactions. Do you see any?

4.     Now switch to the original Alice, and click the blue **Transactions** button. You’ll see the two transactions there, with identical amounts. What do the labels look like?

5.     If the transactions are visible, then the Alice Watch Only wallet should be set up correctly. But let’s check the addresses anyway. So, switch to the original Alice wallet, and click on the blue **Addresses** button on the left. Do the same in the Alice Watch Only wallet.

6.     **Review** that the first few Receive addresses are identical, between the two wallets. If the addresses are identical, and you see the previous transactions, then the watch only wallet is set up correctly. (The labels will be missing on the watch only wallet, though, just like they’re missing for the transactions.)

### Learn more: Why are the labels missing?

Why do the labels only show up in the Alice wallet? It’s because the label isn’t part of the bitcoin blockchain. The label is stored inside the Sparrow wallet file, and not on the blockchain.

When you’re recovering a wallet from a seed phrase, or creating a watch only wallet, all the information you see comes from the bitcoin blockchain, because that’s where it’s fetched from. Recovering a wallet from the seed phrase, or creating a watch only wallet—both of these will generate a list of addresses. When those addresses are checked in the bitcoin blockchain, it gives you any transactions (along with the amounts and dates) associated with the addresses.

What you’re explicitly _not_ getting is information that’s stored in the Sparrow wallet file, such as labels from transactions or addresses.

Here’s another thing to note about the label—the transaction gets the label from the original address. For instance, when you set up your initial receive transaction, from the exchange to your Alice wallet, you entered a label for the receive address. This label shows up as the label for the transaction as well.

### Learn more: checking receive addresses

The last step in this exercise was to compare addresses. What’s the point of comparing the receive addresses between the Alice wallet, and the Alice Watch Only wallet? You did the same thing in Exercise 5: Recover your Alice wallet.

Here’s the reason you compare the addresses. If any of the settings of the wallet are different (such as the script type, or derivation path), then the addresses will be different. In order to make sure that it’s set up correctly, you check to make sure that the first few addresses are the same between the two wallets.

In this case, it’s not strictly necessary because you already see the transactions in the watch only wallet. This means that Sparrow used the correct addresses, and found the correct transactions. But it’s definitely a good idea to remember to check addresses, whenever creating a watch only wallet.