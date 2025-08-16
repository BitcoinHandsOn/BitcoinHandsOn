---
layout: default
title: Exercise 25
---
# Exercise 25: Recover the Bob wallet in Blue Wallet

In this exercise you’ll practice an emergency recovery, recreating the Bob wallet (created in Sparrow) onto the Blue Wallet app on your phone. In any bitcoin wallet software you use, you should always practice an emergency recovery. That way, if the emergency does occur, you’ll be prepared.

Note that this does _not_ create a watch only wallet. Instead, because you’re using your seed phrase, it’s recreating the private key. That means that this wallet will have full signing and spending ability.

1.     Open up Blue Wallet. In the top right is a plus sign, to add a new wallet. **Click on the plus sign**.

2.     On the Add Wallet screen, under Type, make sure to stick with the default of Bitcoin (not Multisig Vault).

3.     Do _not_ click on Create, which is the default. (That creates a brand new wallet.) Instead, click on **Import**. This will give you the opportunity to enter the seed phrase.

4.     Enter the 12 seed phrase for the Bob wallet in the free form field. Make sure to enter them in the right order, with the correct spelling, and a space between each word. Click **Import**.

5.     The transactions will show up soon, if everything was entered correctly.  
You may need to close and reopen Blue Wallet, to make the transactions appear.

6.     The default name for an imported wallet starts with “Imported”. Click on the three dots at the top right, and rename the wallet **Bob Recovery**.

Did you get a message “No wallets were found”? This usually means that you typed in the seed phrase incorrectly. Check the words very carefully, make sure the spelling is exact, and that there’s a space between each word.

**Checking the recovered wallet**: To double-check that the recovered wallet was set up correctly, do two things:

1.     **Review transactions**: You should be able to see the same transactions in the Bob Recovery wallet in Blue Wallet as you do in the original Bob wallet in Sparrow.

2.     **Review Addresses**: Assuming you see the transactions, everything should be good. But in general (and especially if the original wallet has no transactions) you want to review addresses between the original and a recovered wallet.  
In the Bob wallet in Sparrow, click on the blue Addresses button to see the addresses. In the Bob Recovery wallet in Blue Wallet, click on the three dots at the top right. At the very bottom of the dropdown, there’s a **Show Addresses** option. Compare a few of them with the Sparrow addresses. They should be the same. (Blue Wallet makes it difficult to review the addresses that are already used, so just look at the unused ones.)

### Learn more: the private key is portable between wallet applications.

As you know by now, you see identical transactions in Blue Wallet and Sparrow because you used either the public key (for a watch only wallet) or the seed phrase (to recover a wallet).

For the recovered wallet, you entered the seed phrase that was generated for the first Bob wallet. That seed phrase translates to the same private key, and that private key is linked to the same addresses (assuming the script type, etc., is set up correctly).

When Blue Wallet looks up the addresses in the blockchain, it finds the same transactions as Sparrow did, looking up those same addresses in the blockchain.

One of the beautiful things about bitcoin is that you don’t need any _specific_ software. As long as you hold your own private key (which is the whole point of self custody), nobody can prevent you from switching to a different bitcoin software wallet. For instance, if you didn’t like Sparrow, you might decide to work with Blue Wallet.

Compare this to traditional banking. Switching banks requires a lengthy process—transferring funds, closing your old account, submitting ID documents to open a new one, and waiting for approvals. You need permission from financial institutions and government agencies at every step.

Or, consider people living in countries where it’s difficult or impossible to get a bank account. They are often forced to use actual paper currency, which is always losing value, sometimes rapidly. So, they’re completely unable to save money for their future.

Bitcoin can be a lifeline in these situations, if you know how to use it. Nobody can prevent you from saving, sending, or receiving bitcoin.