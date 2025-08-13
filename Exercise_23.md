---
layout: default
title: Exercise 23
---
# Exercise 23: Import the Alice wallet to Blue Wallet via the descriptor

Now you’ll take the public key from Sparrow via the descriptor field, and use it to create a new watch only wallet.

The descriptor in Sparrow is like an expanded version of the public key, which gives complete details about the setup of the wallet.  Not only does it include the public key (xpub/zpub), it also includes the derivation path, the script type, etc. It makes interoperability between different wallet applications much easier.

When creating a watch only wallet, use the descriptor when possible. This means you don’t need to worry about compatibility, and matching all the settings exactly.

1.     Open Blue Wallet, on your phone. Click on the **plus symbol** in the top right corner, to add a wallet.

2.     Ignore everything but the **Import wallet** button at the very bottom. Click on it.

3.     In the Import screen, at the bottom, click the **Scan or import a file** button.

4.     On your computer, go back to the QR code you brought up in Sparrow, and scan it with your phone.  
If you have a problem scanning it, try changing the density of the QR code (with the Decrease Density/Increase Density button at the bottom).

5.     Blue Wallet immediately creates a new watch only wallet for you, with the descriptor you imported by scanning. If the transactions don’t appear within a few minutes, close and reopen the app and you should see them.

6.     The name of the wallet will be Imported Watch-only, and it’s okay to leave it like that.

Do you see transactions in this watch only wallet? You should have the exact same transactions that you see in the Alice wallet in Sparrow, just like with the previous exercise.