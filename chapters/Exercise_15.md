---
layout: default
title: Exercise 15
---
# Exercise 15: Create wallet Alice With Passphrase

In this exercise, we’ll be exploring what happens when you add a passphrase on top of your seed phrase.

Remember, the passphrase is different from the password. A passphrase actually _changes_ your private key. It’s as though you had a completely different seed phrase. But the password, in Sparrow, just unlocks the wallet file so it can be opened.

Awareness of the potential complexity of a passphrase in bitcoin goes a long way in avoiding problems.

1.     Open Sparrow. Close all other wallets, and go to **File > New Wallet**. For the wallet name, type “Alice With Passphrase”, and click **Create Wallet**. Leave everything at the defaults in the Settings window.

**2.**     Below in the Keystores area of the Settings window, choose **New or imported software wallet.**

**3.**     In the top right of the next window, look for the button that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.

4.     Enter the 12 words you wrote down in the step “Create a wallet in Sparrow—Alice”.

5.     Here’s the critical step—this time, go ahead and **click the “Use passphrase?” checkbox**, at the bottom of the words you wrote down. A window titled “Add a passphrase?” will pop up, with some warning text. Sparrow will ask you to confirm that you want to create a passphrase. Click **Yes** to confirm.

6.     Now enter your passphrase. The passphrase is not limited to the BIP39 word list, you can type anything you want in there, including numbers and symbols. It’s also case-sensitive. For now, keep it simple by putting in “**MyPassphrase1234**”. Write down the passphrase on a sheet of paper, and label it “Passphrase for wallet Alice With Passphrase”.

7.     Click the **Create Keystore** button, then the **Import Keystore** button. You’ll be asked to re-enter the passphrase. Re-enter and click **OK**.

8.     Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the “Wallet Password” screen. (Remember, this is the _password_ on the wallet file, it’s not the _passphrase_.)

9.     Now click on the Transactions button. Do you see any transactions? There should be none.

### Learn more: passphrase and password

The reason you don’t see transactions in the step above is that with the passphrase on the original seed phrase, you’ve created a completely different private key, with different addresses. When Sparrow looks up those addresses on the blockchain, there’s no transactions associated with them.

The _password_ (as opposed to passphrase), in Sparrow, is just an extra piece of security that you can put on your wallet file. If you lose the password, but still have the seed phrase, you can easily restore the wallet.

In contrast, the passphrase is a special concept in bitcoin. When you create a wallet with a certain seed phrase, and no passphrase, you generate a specific private key. But when you create a wallet with the exact same seed phrase, and add a passphrase, you get a completely different private key.

Beginners and experts alike often have problems with passphrases. It can seem like a good idea to get some extra security on the seed phrase.

But apparently this particular issue—setting up a passphrase and then forgetting it—is _the most common problem_ that causes people to lose their bitcoin in self custody. People think they’ll always remember the passphrase, then their memory fails them.

The bottom line? **Don’t use a passphrase unless you’re an expert**, and completely understand the risks.