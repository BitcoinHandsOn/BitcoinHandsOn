---
layout: default
title: Exercise 19
---
# Exercise 19: Install Blue Wallet and create the Carol wallet

Your next exercise is to install the Blue Wallet app on your phone, and create a new wallet with it. Blue Wallet is a widely used bitcoin wallet that has a long track record.

Why bother working with another wallet? Wouldn’t it be easier to just stick with Sparrow, since you’ve learned so much about it? Yes, it would be easier. But you wouldn’t learn as much. And you wouldn’t have practiced your ability to restore a seed phrase and test a wallet in an entirely different system. And that’s a _very_ important skill to have, and practice regularly.

Also, learning how a different type of wallet software operates will solidify your understanding of some of the basic concepts of bitcoin—private keys, addresses, and transactions. Comparing two different products helps illustrate these concepts.

Blue Wallet is mostly a mobile wallet, but also has a desktop version for MacOS. We’ll use it on the phone to generate a new wallet, Carol. Just like Alice and Bob, Carol represents a new user of bitcoin. Then we’ll send bitcoin to Carol, and do some other exercises.

Go to the website ([https://bluewallet.io/](https://bluewallet.io/)). Towards the bottom there are links to install it via Google Play or the Apple App Store. Also, you can install it directly on an Android phone, via the APK.

Choose whichever mobile option you prefer, and complete the install. The version that I installed was 7.1.6.

Now, set up the Carol wallet using the following steps:

1.     On a fresh install of Blue Wallet, you’ll see an **Add now** button, to start a new wallet. Click it.

2.     In the Name field at the top, type **Carol**.

3.     There’s an option to choose between a regular Bitcoin wallet, and a Multisig Vault—basically between a single sig wallet, and a multisig wallet. Keep the default of Bitcoin, and click **Create**.

4.     In the next screen “Your wallet has been created”, you’re presented with the seed phrase (Blue Wallet refers to it as a mnemonic phrase). **Write them down** on a sheet of paper, labeled Carol Seed Phrase. Keep this paper safe.  
**Warning**: Blue Wallet does _not_ ask you to check your seed phrase, unlike Sparrow. Be sure to double check that you wrote it down correctly, because it’s easy to be careless. I just made this mistake myself. One of my words was “two”, and for some reason I wrote down “too” instead of “two”. I would have been without a good backup. Luckily, I had a feeling that I was going too quickly, so I double-checked and figured it out in time.

5.     To make it easier to read amounts, switch from the default, of using BTC as the unit, to sats. To do this, click on the Carol wallet to bring it up. Click on the label that says BTC to the right of the amount field. This will switch between BTC, sats, and USD (or whatever currency you have set up in the Settings).

### Learn more: Blue Wallet

Notice that Blue Wallet has many fewer options than Sparrow. There’s only one option for the number of words in your seed phrase (12). And the script type (which Blue Wallet calls Type) is not customizable. You can view the Type, Addresses, and other settings by clicking the three dots in the top right corner, when the wallet is open.

But Blue Wallet is very straightforward to use, and probably has all the functionality you need for a mobile phone wallet. Like Sparrow, Blue Wallet is also open source, which means that the code is publicly available for review ([https://github.com/BlueWallet/BlueWallet](https://github.com/BlueWallet/BlueWallet)).

Here’s a security tip to keep in mind: Whenever you install any bitcoin related software, be very sure that the site you’re installing it from is the real one. For Sparrow, you went to the right site—[https://SparrowWallet.com](https://sparrowwallet.com/).

If you’re downloading an app, make sure it’s the real thing as well. Often scammer apps will get onto the Google Play Store, or Apple App Store. These apps are designed to look just like the real app. Always double-check with reputable people or established websites to be sure you’re installing the real thing.

### Learn more: what is logged in the bitcoin blockchain?

In this exercise you created a new wallet in Blue Wallet. Consider for a moment—is there anything in the bitcoin blockchain, right now, that registers that this wallet has been created?

No, there’s not. This step just creates the wallet in Blue Wallet. You’ve basically just had Blue Wallet create a very large random number for you—your private key, encoded by your seed phrase. You could do this even without an internet connection.

But no actual transactions have taken place. And it’s only the transactions that are broadcast, and logged in the blockchain. The creation of a wallet is not logged in the blockchain.