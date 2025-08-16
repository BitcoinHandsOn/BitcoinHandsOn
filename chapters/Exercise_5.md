---
layout: default
title: Exercise 5
---
# Exercise 5: Recover your Alice wallet

Being able to recover your wallet is an important step in Bitcoin security. If something unexpected happens, you need to be able to gain access to your bitcoin again with just your seed phrase.

So, practicing recovery is a must, when learning to use bitcoin.

1.     In Sparrow, click on **File > New Wallet**. Name the wallet “Alice Recovery” and click on **Create Wallet**.  
Note that we’re creating a new wallet file in Sparrow here, but it will be derived from the original Alice wallet, and will have the same seed phrase (private key).

2.     You’re now in the Settings window. Leave the settings as they are (Single Signature, Native Segwit). At the bottom in the Keystores section, click **New or Imported Software Wallet.** In the next window, look for the button on the top right that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.

3.     Enter in the 12 words you wrote down in the exercise “Create a wallet in Sparrow—Alice”. Don’t create a passphrase. Click the **Create Keystore** button.

4.     Leave the derivation path at the default of m/84’/0’/0’, and click on **Import Keystore**.

5.     Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the “Wallet Password” screen.

6.     You have now recovered your Alice wallet. Click on to the blue Transactions button on the left, to switch to that window. You should be able to see the transaction you made earlier.

7.     Also check the addresses, between the original and the recovered wallet. To do this, open the original Alice wallet, and click on the blue Address button on the left. Do the same in the Alice Recovery wallet.

8.     Cross check the first few Receive addresses between the two wallets. Make sure they’re the same. If the addresses are the same, and you see the previous transaction, you’ve restored the wallet correctly. Congratulations!

### Learn more: wallet recovery

It’s good to practice recovering a wallet occasionally. If you lose your computer, or the Sparrow wallet file, or lose your hardware wallet, you can still recover your wallet—but only if you kept the seed phrase safe.

But if a disaster happened _and_ you didn’t have your original seed phrase or a backup, then unfortunately you’ve lost your funds. You no longer have access to your bitcoin, and you can’t recover from that.

### Common problems when recovering wallets

Some of the common problems that occur when recovering wallets are:

·       Missing a Passphrase

·       Differences in Script Type

We’ll go over both of these issues in more depth in upcoming exercises.