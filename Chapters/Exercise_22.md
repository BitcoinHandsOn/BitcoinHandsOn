---
layout: default
title: Exercise 22
---
# Exercise 22: Import the Alice wallet to Blue Wallet via the public key

In this exercise we’ll take the public key from Sparrow, and use it to create a new watch only wallet in Blue Wallet. You’ll learn how this works in general, and some of the pitfalls to avoid in the process.

1.     In Sparrow, close any other wallets and open the Alice wallet. Click on the **Settings** button.

2.     In the Keystores section at the bottom, look to the right of the xpub/zpub field for the QR code symbol. Click on the **QR code symbol**, to pop it up for this xpub.

3.     Now open Blue Wallet, on your phone. Click on the **plus symbol** in the top right corner, to add a wallet.

4.     Skip the Name field, and do not click the Create button. Instead, at the very bottom, click **Import**.

5.     In the Import screen, at the bottom, click the **Scan or import a file** button. On your computer, go back to the QR code you brought up in Sparrow, and scan it.

6.     Blue Wallet immediately creates a new watch only wallet for you, with the xpub you imported by scanning. If the transactions don’t appear within a few minutes, close and reopen the app and you should see them.  
The name of the wallet will be Imported Watch-only, it’s okay to leave it like that.

7.     Do you see transactions in this watch only wallet? You should have the same transactions that you see in the Alice wallet in Sparrow.

### Learn More: Different derivation paths = different address

In an older version of Blue Wallet, the steps you just went through would not have worked. You wouldn’t have seen any transactions. This was because if you imported an xpub in Blue Wallet, the wallet would have been set up with a different script type and derivation path. This means the transactions would never have shown up, because different addresses would have been generated.

This caused lots of problems and stress for people who set up a watch only wallet to get receive addresses. They did this to easily receive bitcoin, while not having their seed phrase in Blue Wallet.

But if they used a receive address that they copied from Blue Wallet, the transaction would never have shown up in Sparrow because of the difference in derivation path.

Happily, this problem has now been resolved by Blue Wallet. But always remember to do some checking when setting up a watch only wallet.

·       If there are existing transactions in the wallet, you should be able to see them. If you can’t, there’s a problem.

·       Check that the first few addresses are the same. You know where to find the addresses in Sparrow. In Blue Wallet, click on the three dots at the top right, and then click on Show Addresses.

Before the next exercise, the wallet that you just created needs to be deleted. To do that, follow these steps:

·       Click on the wallet to open it (the name will be Imported Watch-only).

·       Click on the three dots in the top right corner, to get to the settings screen. Click on the three dots in the top right corner again, and you’ll find a red Delete option. Click it.

·       Blue Wallet will ask you to confirm. Click “YES, DELETE” to confirm.