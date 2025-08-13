---
layout: default
title: Exercise 14
---
# Exercise 14: Create wallet Bob Legacy Script Type

This exercise will show you what happens if you restore a wallet via a saved seed phrase, but use a Script Type that’s different from what the wallet was created with.

It’s important to understand this situation, because many people have “lost” bitcoin, through recovering the wallet with the wrong script type. The funds aren’t truly lost, it’s just that the wallet needs to be set up correctly. Relying on another person to help you in this situation introduces risk—it’s best to understand how to fix it yourself.

The seed phrase you’ll be working with is the one for the Bob wallet.

1.     Open Sparrow, and close all open wallets. Click on **File > New Wallet**. For the wallet name, type “Bob Legacy Script Type”, and click **Create Wallet**.

2.     Next in the Settings window, for the first time we will change one of the defaults. Click on **Script Type**, and choose **Legacy (P2PKH)**.

3.     Below in the Keystores area of the Settings window, choose **New or imported software wallet**. Now look for the button on the top right that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.

4.     Enter the 12 words you wrote down in the exercise “Create a wallet in Sparrow—Bob”. Don’t create a passphrase. Click the **Create Keystore** button.

5.     Leave the derivation path at the default of m/44’/0’/0’. Note that it’s different from the derivation path you saw in other wallets. Click on **Import Keystore**.

6.     Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the Wallet Password screen.

With these steps you’ve created another wallet, based on the Bob seed phrase (private key). You’ve basically “recovered” a wallet, like you did in a previous exercise.

However, this wallet uses a different script type. Let’s do some checks here, to see how the script type affects the wallet.

1.     Open up the original Bob wallet.

2.     Click on the blue Transactions button in the original Bob wallet, and compare the transactions to those in the new Bob Legacy Script Type wallet. What do you see?

3.     Compare the addresses in Bob to the Bob Legacy Script Type wallet. Notice that they’re in a different format. In the original Bob wallet, they all start with bc1. Also, the rest of the address is different as well.

The Transactions screen in the new wallet should be empty, with a zero balance. Even though you used the same exact seed phrase, the addresses are different if the script type is different. Sparrow checks the blockchain only for those addresses that it knows about. And it uses the script type to generate the addresses, so it gets different addresses when the script type is different.

### Learn more: Script type problems

The most important thing to remember about script type is that whenever you’re recovering a wallet, or using a watch only wallet, you _must_ match the script type (and other settings, like the Derivation) with the original wallet.

Bitcoin script types define address formats and spending rules. The default now, in 2025, is Native Segwit, but earlier it was different.

This should happen by default, in most modern bitcoin wallet software, but it’s best to check.

This situation—having different script types when you’re trying to recover a wallet—has caused many people anxiety. Maybe you _know_ that you wrote down and entered the seed phrase correctly, but you just don’t see any transactions when you know there should be some.

But it may be that when you created your wallet, the software you used had one particular default script type. And then in the software you used to recover it, the default script type is different. That causes the addresses to be different, which causes the transactions to not be found. When the transactions can’t be found, your wallet shows a balance of zero.

You won’t have an exercise on this, but the derivation setting is similar to script type. If you restore your wallet with an incorrect derivation, you will get different addresses, and will not see your bitcoin.

It’s important to know that getting the Script Type or Derivation wrong is not bad in the same way as losing your seed phrase. If you have completely lost your seed phrase, there is no chance at all of recovering your bitcoin. But if there’s a script type mismatch, you just need to fix that one thing, and you’ll be fine.