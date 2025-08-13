---
layout: default
title: Exercise 9
---
# Exercise 9: Explore the Settings window of the Alice wallet 

In this exercise, we’re going to get familiar with a few of the items in the Settings window of the Alice wallet. We won’t go into all of these settings in depth—this is just to get an overview of the settings you’re most likely to use.

1.     In Sparrow, make sure you have the Alice wallet open. The first option is **Policy Type**. With Policy Type you can choose between Single Signature and Multi Signature. Single Signature is the most common and simplest, and that’s what we’ll be using in this book.  
Multi Signature is much more complex, and requires multiple different private keys. It’s for people with significant assets in bitcoin, who need more security.  
(Warning: If you’re experimenting and switch to Multi Sig, it’ll look as though you lost your seed. Just close and reopen the wallet, and it'll be fine)

2.     Next is **Script Type**. Native Segwit is what we’ll be using now, and that’s the default in Sparrow and most bitcoin wallet software. But it’s useful to know that using different or incorrect script types can cause problems. This happens occasionally when trying to restore a wallet.

3.     The **Descriptor** is a way of encoding information about your wallet, in a way that it can be easily transferred between two different bitcoin wallet applications. We’ll be using it in upcoming exercises.

4.     Inside the Keystore area on the Settings window, you can click on the **View Seed** button and easily see the seed phrase you wrote down earlier.  
This isn’t secure, of course, but since this is a low-risk wallet (both temporary and containing only a small amount of bitcoin), you don’t need to worry about it now. Later on, you’ll want more security, and we’ll review other options.

5.     The **Label** is mostly a way of distinguishing between different wallets. By default with this type of wallet, it’s set to BIP39, but you can change it. It’s used mostly with Multi Signature wallets.  
The **Master Fingerprint** is similar to the Label, in that it uniquely identifies the wallet. But Master Fingerprint is system generated, as opposed to being something you can edit.

6.     The **Derivation** field is basically the method that Sparrow uses, in order to figure out how to create addresses from the seed phrase. We’ll mostly be using the default. But if you’re recovering a wallet and the derivation for a wallet isn’t correct, then the addresses won’t be correct either. And then no transactions will be found.

7.     At the bottom, there’s a field labeled **xpub/zpub**. This is usually called the **public key**. We’ll be using it in the next exercise.

  

**Congratulations!**

 You've completed the beginner exercises, and have mastered some basics.

Are you enjoying this book so far?  I'd love for you to share your thoughts with a review on Amazon!

If you have feedback on the exercises, please let me know. Contact me at [feedback@BitcoinHandsOn.com](file:///C:/Sylvia/_PracticalBitcoinBook/feedback@BitcoinHandsOn.com).

Exercise 10: Create watch only wallet based on Alice

In this exercise you’ll create a special kind of wallet, a watch only wallet. It’ll be based on the Alice wallet you created earlier.

Why create a watch only wallet? The main reason is to keep your seed phrase—that extremely important set of words—secure, private, and not exposed very often.

In a watch only wallet you can do many of the tasks that you need to do in a wallet, like receive bitcoin, and monitor transactions. The only thing you can’t do is spend bitcoin.

It’s common to create a watch only wallet for your main wallet. A watch only wallet is not a “hot wallet”. This means that it does _not_ hold your private key. And there’s no “View Seed” button in the wallet, like we saw in exercise 9.

However, you can still see the transactions and addresses, though you can’t spend. So, it’s more secure to have a watch only wallet set up on your computer than it is to have an actual “hot” wallet, which is what your Alice wallet is.

To create the wallet, follow these steps:

1.     Open Sparrow. Close all wallets except the Alice wallet.

2.     Click on File > New Wallet. Name it “Alice Watch Only”.

3.     In the new wallet, you’ll end up on the Settings window. In the Keystore section, click on **xPub / Watch Only Wallet**.

4.     Now, open your Alice wallet, if it’s not already open. Click on the blue **Settings** button to go to the Settings window in your Alice wallet.

5.     In the Keystores section of the Alice wallet, at the bottom, is the xpub/zpub, which is the public key. **Copy the public key**, and then switch to the Alice Watch Only wallet. **Paste it** in the xpub/zpub text box.

6.     Click **Apply,** to create the Alice Watch Only wallet.

7.     On the Wallet Password screen, click **No Password**.

You’ve now successfully created a new watch only wallet in Sparrow. You should be able to see, in the Transaction window of the Alice Watch Only wallet, the same transactions that you see in the Alice wallet.

### Learn more: Public keys, watch only wallets, and privacy

A watch only wallet is created, as you saw above, with the public key. Sometimes in more technical discussions, it’s called extended public key, or master public key, but I’ll use the term public key in this book.

In Bitcoin, your public key is similar to an account number. From it, you (or anyone) can generate addresses, and use those addresses to send you bitcoin. And because they see your addresses, they can track your transactions on those addresses.

Your public key is generated _from_ your private key with some complex math, but can't be reversed to reveal your private key. And without your private key, your bitcoin cannot be spent. Still, you don’t want to expose your public key, because anyone who knows it can track all your bitcoin addresses, and all your transactions.

So, for the sake of privacy, make sure that you keep your public key a secret.

One common use of watch only wallets is to generate receive addresses. We’ll talk about this more in an upcoming exercise.