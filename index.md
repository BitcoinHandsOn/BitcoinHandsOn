Bitcoin

Hands-On!

_28 “learn-by-doing” exercises to master the basics of managing your own Bitcoin, including wallets, transactions, and  
self custody_

Sylvia Vasilik

Copyright © 2025 by Sylvia Vasilik

All rights reserved. No part of this book may be used or reproduced in any manner whatsoever without written permission, except in the case of brief quotations in critical articles or reviews.

ISBN 978-1-7341663-2-3 (ebook)

ISBN 978-1-7341663-3-0 (paperback)

Published by Fluid Progress Press

Version 200  
July 2025

**Disclaimer**

This book is intended for educational and informational purposes only. The content is the author’s understanding of Bitcoin. It should not be considered financial, investment, legal, or tax advice. Always do your own research, consult qualified professionals, and follow local laws and regulations. Protect your private keys and other data—lost or stolen keys mean lost funds.

By reading this book, you accept full responsibility for your actions and acknowledge these risks.

**Contents**

[Introduction 1](#_Toc202777437)

[Exercise 1: Install Sparrow Bitcoin Wallet 5](#_Toc202777438)

[Exercise 2: Create Alice wallet in Sparrow 9](#_Toc202777439)

[Exercise 3: Buy Bitcoin 13](#_Toc202777440)

[Exercise 4: Receive bitcoin into your Alice wallet 17](#_Toc202777441)

[Exercise 5: Recover your Alice wallet 22](#_Toc202777442)

[Exercise 6: Create wallet Bob 24](#_Toc202777443)

[Exercise 7: Your first send—transfer bitcoin from Alice to Bob 26](#_Toc202777444)

[Exercise 8: Review the Alice to Bob transaction 29](#_Toc202777445)

[Exercise 9: Explore the Settings window of the Alice wallet 32](#_Toc202777446)

[Exercise 10: Create watch only wallet based on Alice 35](#_Toc202777447)

[Exercise 11: Explore the Alice Watch Only wallet 37](#_Toc202777448)

[Exercise 12: Receive bitcoin via a watch only wallet 39](#_Toc202777449)

[Exercise 13: Use the Alice Watch Only wallet to send a transaction 41](#_Toc202777450)

[Exercise 14: Create wallet Bob Legacy Script Type 43](#_Toc202777451)

[Exercise 15: Create wallet Alice With Passphrase 46](#_Toc202777452)

[Exercise 16: Review some transactions 49](#_Toc202777453)

[Exercise 17: Send bitcoin from Alice to Bob—review fees 53](#_Toc202777454)

[Exercise 18: Bitcoin fees—what you pay, and why 56](#_Toc202777455)

[Exercise 19: Install Blue Wallet and create the Carol wallet 60](#_Toc202777456)

[Exercise 20: Send bitcoin from Bob in Sparrow to Carol in Blue Wallet 63](#_Toc202777457)

[Exercise 21: Send bitcoin from your exchange to Blue Wallet Carol 65](#_Toc202777458)

[Exercise 22: Import the Alice wallet to Blue Wallet via the public key 67](#_Toc202777459)

[Exercise 23: Import the Alice wallet to Blue Wallet via the descriptor 69](#_Toc202777460)

[Exercise 24: Set up password protection on Blue Wallet 71](#_Toc202777461)

[Exercise 25: Recover the Bob wallet in Blue Wallet 73](#_Toc202777462)

[Exercise 26: Send all bitcoin from the Bob Recovery wallet in Blue Wallet to Alice in Sparrow 76](#_Toc202777463)

[Exercise 27: Bonus—use Blockstream wallet 78](#_Toc202777464)

[Exercise 28: Clearing practice wallets and creating a long-term wallet 80](#_Toc202777465)

[Final notes and next steps 82](#_Toc202777466)

[Resources 91](#_Toc202777467)

Introduction

First of all, thank you for purchasing this book! Any feedback would be appreciated. For any questions or issues, please send email to [feedback@BitcoinHandsOn.com](feedback@BitcoinHandsOn.com).

I’ll start out by telling you what this book is not. It’s not about the “why” of Bitcoin. I’m going to assume that since you’re reading this book, you’re convinced that Bitcoin has a lot of promise, and you believe that learning how to use Bitcoin directly, without intermediaries, is important.

It’s also not about the history of money, why government currencies (also known as “fiat currencies”) seem to inevitably fail, how inflation is actually theft, or similar topics. There are writers much smarter than I am who have gone over these topics, in depth. I list some of the best books in the [Resources](#Resources) section.

Instead, this book is all about actually using Bitcoin. It’s about using software to create wallets that you control directly—in other words, self custody. It’s about understanding, at a very practical level, what a private key is and why it’s important. It’s about learning to manage your wallets, and sending and receiving sats (short for satoshis, 1 bitcoin equals 100 million sats) without needing to go through gatekeepers like banks or investment firms. Learning how to use Bitcoin may be the most important technical skill you ever develop.

Why is self custody important?

Holding your own bitcoin—self custody—is key to getting the benefit of Bitcoin, over the long run.

If you already own bitcoin, is it in self custody? Well, if you don’t have the private key—the private key that you could use to send and receive the bitcoin directly—then it’s not in self custody.

Let’s look at some cases where people think they own bitcoin, but they don’t actually control it:

*   If you’re holding bitcoin on an ETF (exchange traded fund), then you don’t have bitcoin in self custody, it’s all managed by the fund. It’s not possible to withdraw actual bitcoin from the exchange. Instead, you need to sell the bitcoin and withdraw USD.
*   If you’re holding bitcoin on an exchange, such as Coinbase or Kraken, then you still don’t have bitcoin in self custody.

An exchange is an improvement over an ETF, because usually you can withdraw the bitcoin into a self custody wallet.

But still, many exchanges have failed—through hacks or fraud—since Bitcoin’s creation. Early bitcoiners learned through bitter experience that they shouldn’t trust exchanges.

The history of Bitcoin exchanges is full of these scams and thefts, ranging from one of the earliest and most famous (Mt. Gox in 2014) to more recent scams (FTX and Celsius in 2022).

There’s one thing these disasters had in common. It’s that the supposed “owners” of the bitcoin did _not_ actually hold their own keys. Instead, they left their bitcoin in the custody of others, in what are called “custodial wallets”. People thought it was safer to have their bitcoin in the custody of large firms, instead of managing it themselves. They were wrong.

Not your keys, not your coins

If you didn’t understand “_Not your keys, not your coins_”, you wouldn’t have necessarily known that you were doing something dangerous, by relying on other people to manage your bitcoin.

For instance, take one of the more recent exchange failures, FTX. Mainstream media news coverage of FTX was glowing. It stayed positive until just before the whole thing unraveled, and was revealed as a huge scam. Most users didn’t realize they were taking a serious risk by leaving their bitcoin on the platform.

It’s not as hard as it seems

For many people, self custody—using bitcoin directly and holding the private key themselves—is intimidating. Without an intermediary like a bitcoin exchange or ETF, people worry about making mistakes and losing their hard-earned money. Many people avoid self custody because they don’t understand seed phrases and private keys.

Bitcoin can seem mystifying and complex. It may seem that using Bitcoin requires an understanding of the underlying technology, and in-depth knowledge of cryptography.

But that’s absolutely not true. I’m here to tell you that you do _not_ need this in-depth knowledge. Do you need to understand how a car engine works, in order to drive? No, you don’t. You also don’t need to understand every technical detail about how Bitcoin works, in order to safely use it.

Taking small steps in a safe environment

The learn-by-doing exercises in this book will walk you through the process of learning Bitcoin, one simple step at a time.

When you’re learning to drive a car, do you immediately start driving on the highway? No, you don’t. You head to a large parking lot, and practice driving there. You make a lot of left turns and right turns, starts and stops. That’s what you’ll be doing in Bitcoin, Hands-On—lots of practice, in a low-risk environment.

Working your way through this book will help you overcome the anxiety that can come with managing your own bitcoin. The exercises use a few temporary, small test wallets, that you create and control. This is the Bitcoin equivalent of taking your first drive in a parking lot, to learn about the steering wheel, gas pedal, and brake.

With these small wallets, you’ll make steady progress through the exercises with small amounts, gaining confidence and learning to avoid the problems that can occur. You master the skills you need to safely send, receive, and store bitcoin.

How to get the most out of this book

Here’s a few tips on going through the exercises, and how to really learn the practical aspects of Bitcoin—in a way that sticks.

*   Name the wallets exactly as shown in the instructions. This makes it easier to follow along, because the same wallets are used throughout the whole book.
*   Complete all the exercises, even if you think you know what’s going to happen. Actually doing the steps is key to learning. Just reading isn’t enough.
*   Consider doing each exercise twice. First, follow along step by step with the book. Then, try it again without the instructions—just from memory and the name of the exercise. That’s where the real learning happens.
*   Transaction fees now (early 2025) are quite low. But if you’re concerned about fees, the lowest fees are usually on weekend mornings, US east coast time (EST). So, consider doing the exercises that involve transactions during that time. You’ll learn more in exercises 17 and 18 about fees.

Author’s note on Bitcoin capitalization:

Standards are still evolving on when Bitcoin should be capitalized, but the consensus seems to be—upper case when speaking of Bitcoin as a system, and lower case when speaking of the currency units, or as an adjective. That’s what I do in this book.

# Exercise 1: Install Sparrow Bitcoin Wallet

In this step we’ll install Sparrow Bitcoin Wallet. Sparrow is the most widely used and respected desktop Bitcoin wallet. It’s free—and more importantly, it’s open source. Open source software means that the code is publicly available for review. You can see the actual Sparrow Wallet source code right here: [https://github.com/sparrowwallet/sparrow](https://github.com/sparrowwallet/sparrow). This allows people to verify there’s nothing harmful hidden in the software.

Sparrow Wallet is suitable for beginners, but has all the functionality expert users need as well. So, it’s a great tool to use on your Bitcoin learning path. The Sparrow version that I used is 2.2.2. However, it’s frequently updated, and your version might be different. If any changes significantly impact these exercises, I will update them.

To install Sparrow, go to [https://sparrowwallet.com/download/](https://sparrowwallet.com/download/). You’ll see options for downloading versions for MacOS, Windows, and Linux. Download and install whichever version matches your operating system. The instructions for the install will be different for each operating system.

If you’re using Windows, there’s an Installer version and a Standalone version. Download the Installer version unless you have a specific reason to use the Standalone version. During the install, leave all the settings at the default.

The instructions in the exercises will be with the Windows version of Sparrow, but it should be very similar in the MacOS and Linux versions.

I get a warning “Windows protected your PC” when I try to install

If you’re running Windows, there are filters turned on to protect you against unsafe software. But this filter can also be triggered by software that’s less common, like Sparrow. As long as you’ve downloaded Sparrow from the above link, you’re fine. In the warning window, click “More info” and then “Run anyway” to continue with the installation.

In the Edge Browser, the Sparrow download has an orange warning triangle

When using the Windows Edge Browser, a message comes up saying that the file isn’t commonly downloaded, and make sure you trust it before opening it. Click on the 3 dots to the right of this message, click Show more, and then Keep Anyway.

Is it hard to see the full screen in Sparrow, or is the text too small?

Sparrow is written in Java, to make it easier to run on different operating systems. However, one disadvantage is that it can cause screen resolution problems.

For me, with my resolution, I just live with it because it’s not too bad. But you can also change the resolution by clicking on the Windows Start button, typing “Resolution”, and then choosing the option “Change the resolution of the display”.

Then under Scale and Layout, click the dropdown under “Change the size of text, apps, and other items”, I experimented with reducing my resolution. On your computer you may need to reduce or increase the resolution.

Here’s some information from the developers of Sparrow on the problem:

[https://sparrowwallet.com/docs/faq.html#im-running-on-a-high-resolution-screen-and-sparrow-icons-and-text-are-tiny](https://sparrowwallet.com/docs/faq.html#im-running-on-a-high-resolution-screen-and-sparrow-icons-and-text-are-tiny)

[https://sparrowwallet.com/docs/faq.html#sparrow-is-too-big-for-my-screen](https://sparrowwallet.com/docs/faq.html#sparrow-is-too-big-for-my-screen)

What server to connect to?

When you install Sparrow, you’ll get some options about choosing a server. This server is what Sparrow uses to point to the Bitcoin network. For now, we’ll stick to the default of using a public server, mempool.space.

Troubleshooting your connection in Sparrow

Occasionally, you may notice that you can’t click the “Broadcast Transaction” button to send a transaction, or that you’re not seeing the latest transaction in a wallet. If the slider at the very bottom right corner in Sparrow is gray, you have lost your connection. This can happen sometimes, especially after restarting or switching wifi networks.

To fix this, click on the slider to reconnect, or click **File > Preferences > Server**, to edit and test your connection.

Some warnings

There are websites and applications out there that pretend to be the real thing, but are not. For instance, the real site for Sparrow is [https://sparrowwallet.com](https://sparrowwallet.com).

Unfortunately, a scam website (sparrowwallet.net) sometimes comes up when you search for Sparrow Bitcoin Wallet. But the software on that website is designed to steal your bitcoin.

So, always be careful of any bitcoin related software that you install. Check multiple sources to make sure you’re downloading from the right website.

Extra Credit: verify the software

When using open source software—especially bitcoin software—the extra step of verifying the software is recommended. Verification is a step that confirms that the software is actually what it’s supposed to be. It validates that there’s no extra code snuck in, that could somehow compromise your bitcoin.

Verifying, and knowing for yourself, is one of the core principles of Bitcoin. It’s embodied in the saying popular with bitcoiners: “Don’t trust, verify”. And it’s also easier, with Bitcoin. All the core software is open source, and you can review it.

Don’t trust, verify

To verify the Sparrow code, go to this page: [https://sparrowwallet.com/download/.](https://sparrowwallet.com/download/.) Scroll down to the “Verifying the Release” section, and follow the steps there. This will ensure that the download wasn’t corrupted with malware.

# Exercise 2: Create Alice wallet in Sparrow

In this exercise, you’ll create your first wallet. Wallets are the foundation of working with bitcoin, and most of the exercises in this book involve wallets. The name Alice will be used for this wallet. You can think of the wallet as belonging to Alice. Later on, you’ll create more wallets, belonging to different characters.

1.  Open Sparrow, and click on **File > New Wallet**. For the wallet name, type “Alice”, and click **Create Wallet**. (Ignore the “Has existing transactions” checkbox, you’ll never use it.)
2.  Next, in the Settings window, leave everything at the defaults (policy type Single Signature, Script Type of Native Segwit). Below in the Keystores area of the Settings window, choose **New or imported software wallet.**
3.  In the window that comes up, look for the button on the top right that says Use 24 words and **click the arrow to the right**. Choose **Use 12 words instead**.
4.  A screen will pop up with 12 blank spaces for your words. At the bottom, click **Generate New** to have Sparrow auto-generate them. (Ignore the “Use passphrase?” checkbox.)

*   Sparrow will now generate a list of random words for your seed phrase.
*   They’re based on a special list of 2048 unique words, called the BIP39 list. The words were chosen because they’re common, easy to spell, and the first 4 letters are unique for each word.

1.  **Write down the words** on a sheet of paper. Make sure to number them correctly, because the order is very important. Label the words “Alice Seed phrase”.
2.  Once you’ve written down the words, click on **Confirm Backup**. On the next screen, confirm that you’ve written them down. Then click on **Re-enter Words**.
3.  Now re-enter the 12 words, then click **Create Keystore,** then **Import Keystore** in the top right.
4.  You’re back at the main screen, the Settings window. You need to apply all the changes you’ve made. Click **Apply**, on the bottom right. In the Wallet Password screen that comes up next, click **No Password**.

Congratulations! You’ve created your first wallet.

Learn more: seed phrases and private keys

In this exercise, we asked Sparrow to generate the Mnemonic Words. These words are also commonly called the recovery phrase, backup phrase, or seed words. But the most common way to refer to these words is “seed phrase”. That’s what I’ll use in this book.

This seed phrase represents a very large number, that’s more random and impossible to guess than we can comprehend. The seed phrase is just an easy way for humans to remember and write down that number, using a specific set of common words. This list is called the BIP39 word list.

For instance, here’s a sample 12 word seed phrase:

| 1. labor | 5. check | 9. gauge |
| --- | --- | --- |
| 2. stable | 6. amused | 10. fat |
| 3. narrow | 7. young | 11. surface |
| 4. high | 8. rotate | 12. cradle |

It translates into this very large hexadecimal number:

775638ce67a669ae9fcb7e5618782bdaafe93c233ebc09469144f475b2c74bf55f4752b51e1abb17460877c4cf9b2ae283f2e48831dc244f8d1ff5f184c1b33f

You can see why the seed phrase is easier to write down! This number is usually called the private key. Sometimes, in more technical discussions, it’s called the Master Private Key or Extended Private Key. But in this book, I’ll use the term private key. We’ll talk more later about how important it is to keep the seed phrase (and thus the private key) private and secure.

There are also methods for generating your own random words for a seed phrase with dice or coin tosses, without having Sparrow do it for you. I won’t go into them in this book.

Learn more: wallets

Is the word “wallet” the best word to use, for what you’re creating here? It’s been used a long time, and it’s the best word we have. But it can be misleading. It suggests that there is bitcoin actually stored in the wallet, but that’s not true.

Instead of thinking of the wallet as containing bitcoin, it’s better to think of the wallet as containing a key. The key that it contains is the private key, encoded from the seed phrase. The private key can unlock certain, specific chunks of bitcoin on the blockchain—any bitcoin that’s associated with addresses that belong to that private key. One private key can contain many addresses.

As you work through the rest of the book, you will create these separate wallets, each with its own unique seed phrase (private key). These wallets will be named:

*   **Alice**: The wallet you just created in Sparrow (Exercise 2)
*   **Bob**: A second wallet that you’ll create in Sparrow (in Exercise 6)
*   **Carol**: A wallet that you’ll set up in Blue Wallet, a popular bitcoin wallet application (in Exercise 19)
*   **Dan**: A wallet you create as a bonus final exercise, in Blockstream, which is another multi-platform bitcoin wallet (in Exercise 27)

Although you will create a few other wallets, they will all be derived from one of these four.

Though we’re naming wallets after people (like Alice and Bob), this is just to make it easier to understand. But one person _can_ have multiple wallets, for different purposes. For instance, Alice may have a Cold Storage wallet, and a Spending wallet, just like you might have a savings account and a checking account at a bank.

Using these different wallets, in multiple bitcoin wallet applications, you’ll gain hands on experience with many user interfaces. This approach is an excellent way to master the fundamentals of Bitcoin, and to learn the skills needed to safely hold, send, and receive bitcoin.

# Exercise 3: Buy Bitcoin

In this step, you’ll actually purchase bitcoin, using whichever source you prefer from the options given below. In the exercise after this one, you’ll move some of that bitcoin to the wallet you created in Exercise 2.

How much will you buy? Choose an amount that you’re comfortable with, probably less than 50 to 100 USD, or the equivalent in other currencies.

This should be an amount small enough that you’re not worried about losing it, but large enough to be able to do all the exercises. You’ll pay transaction fees to move the bitcoin around to different wallets, but otherwise the bitcoin is yours to keep. And you’ll learn more about transaction fees as you go through the exercises.

A reminder**—**when you’re buying bitcoin in this step, you’re _not_ buying it on an exchange traded fund (ETF), because then you wouldn’t be holding and managing your own bitcoin. Instead, you’re buying bitcoin that you can receive into your own wallet, in self custody.

Since there’s so many different sources to buy bitcoin from, I can’t walk you through the process of setting up an account and buying bitcoin, because it will be different everywhere. But I’ll give you some general thoughts about the best ways and sources to buy from.

Also, a note about keeping your bitcoin safe—at this point, you just need to take very basic security precautions. This is because:

*   The amounts that you’re dealing with are small.
*   The wallets you’re working with are temporary. Once you’ve finished the exercises, you’ll send the bitcoin to another wallet.

Where should you buy bitcoin? KYC or P2P

There are two main ways of buying bitcoin, KYC (“Know Your Customer”) and P2P (Peer To Peer).

**KYC** is what most people use, in countries where exchanges are available. It means using a centralized exchange, which follows government “Know Your Customer” laws. On a KYC exchange, you need to open an account, linked to your government ID, to purchase bitcoin. You will need to go through an identity verification process. This usually includes submitting photos of government-issued ID, as well as facial scans.

**P2P** means you’re not going through a regular exchange. Instead, you’re buying from a peer—someone who owns bitcoin and wants to sell it.

If you’re lucky enough to have a friend or family member who’s willing to sell you a small amount of bitcoin, then the transaction can be very simple. You hand the friend or family member some cash, and give them a bitcoin address from your wallet. Then they send you the bitcoin (minus the transaction fee).

But often, P2P trades will be done online, via one of the secure, private services mentioned below.

One of the main benefits of buying P2P is increased privacy. If you’re buying peer to peer, the only other person that knows about the purchase is the seller. However, if you’re buying from a KYC exchange, your personal information is available to both the exchange, and the government. And considering how often companies have been hacked and their customer database stolen—it’s not just the government who could get your data. Criminal gangs could get it as well.

The problem for people just starting to buy bitcoin is that for these P2P services, you need to already own at least a small amount of bitcoin. This is because usually a bitcoin bond or escrow needs to be set up.

KYC Exchanges

If you’ve decided that for now, you’ll use a KYC exchange, you have many options.

It’s important to purchase from a bitcoin-only exchange. An exchange that is bitcoin-only will have fewer points of failure. And more importantly, they won’t try to sell you other, inferior cryptocurrencies, that they make more commission on. Companies that sell anything other than bitcoin (exchanges such as Coinbase, Kraken, Robinhood, Binance) are _not_ recommended.

There’s a saying among bitcoiners that expresses a core belief—that Bitcoin stands alone, and is fundamentally superior to other cryptocurrencies.

Bitcoin, not crypto.

Here’s some KYC exchanges that are Bitcoin-only. This is not an exhaustive list, and this information can change quickly, so do your own research. Also, the exchange should make it very clear that they will actually allow you to withdraw your bitcoin, to your own wallet.

| Strike (Many countries) | https://strike.me/ |
| --- | --- |
| Swan (US) | https://www.swanbitcoin.com/ |
| Unchained Capital (US) | https://unchained.com/ |
| River (US) | https://river.com/ |
| Cashapp (US, UK) | https://cash.app |
| Relai (Europe, Swiss-based) | https://relai.app/ |
| Bull Bitcoin (Canada, Europe) | https://www.bullbitcoin.com/ |

P2P exchanges

In general, using a P2P exchange can be a little more challenging. Also, even more so than with KYC exchanges, you’ll need to stay informed because the P2P markets can change quickly. But on the plus side, you get the best possible privacy, and that’s worth a lot.

Below are some of the more common P2P exchanges. For more options, take a look at this site: [https://kycnot.me/](https://kycnot.me/).

| Robosats | https://learn.robosats.com/ |
| --- | --- |
| Bisq | https://bisq.network/ |
| Peach | https://peachbitcoin.com/ |
| Hodl Hodl | https://hodlhodl.com/ |
| Vexl | https://vexl.it/ |

Robosats requires a Bitcoin Lightning wallet in order to use it (see the [Resources](#Resources) section at the end of this book for more information on Lightning), but it’s one of the most popular and easiest P2P exchanges.

In the next exercise, you will need to have already completed the purchase of bitcoin. It needs to be ready to send, from the exchange to your own receive address.

# Exercise 4: Receive bitcoin into your Alice wallet

In this exercise, you’ll actually receive bitcoin into your wallet. The procedure will be a little different on each exchange. Some exchanges may even require you to get approval for the receive address.

But basically, it will involve steps similar to this:

*   Open up the website or app for your exchange (where you bought the bitcoin), and navigate to where you can send bitcoin out of the exchange.
*   Enter a bitcoin address. (This will be a receive address that you get from the Alice wallet).
*   Decide how much you want to send. It’s easier to think of bitcoin amounts in terms of sats, because 1 bitcoin is now very expensive. (Sats is short for Satoshis. One whole bitcoin equals 100 million sats.)
*   Enter the amount of sats you want to send to the Alice receive address.
*   Decide on the amount of fees you’re willing to pay. Some exchanges may offer free transaction fees.
*   Hit the send button, and wait for the bitcoin to arrive in your wallet.

Example: Using Strike to receive bitcoin

These are what the steps look like when sending bitcoin from Strike, the KYC exchange that I mentioned above. Remember, the process in the exchange that you use will be different. Using Strike (which is a mobile app on your phone), it’s easiest to use QR codes to get the bitcoin receive address, instead of copying and pasting the address.

1.  In Sparrow, open up the Alice wallet file. Click on the blue **Receive** button on the left. Your wallet has many, many receive addresses, and Sparrow will show you the first available address.
2.  Label the receive address. I wrote “Receive from Strike” in the label. When using the defaults in Sparrow, all bitcoin addresses start with bc1. The QR code for the address, which I’ll use in the next step, is to the right of the address.  
    Don’t skip the label! Some of the following exercises depend on having labels.
3.  In the Strike app, I click the Bitcoin icon at the bottom left. I scroll to the Send screen, and click Bitcoin wallet.  
    Then I go back to Sparrow on my computer, where the Receive window is still open. I use Strike on my phone to scan the Sparrow QR code for the receive address.
4.  In Strike, I enter the amount of sats that I want to send (about half of what I purchased).
5.  Next is the fee. I could either pay a larger fee, to have the transaction go through in the next 10 minutes, a medium fee to send it in the next hour, or zero, to have it go through in the next 24 hours.  
    I chose to pay the higher fee, and have it go through within about 10 minutes. Other exchanges will have different options for fees.
6.  On the next screen I review the details (amount, receive address), before clicking to confirm the transaction.

If the exchange you’re using is a desktop application, and not a mobile app, you’ll need to copy and paste the bitcoin address, instead of using a QR code.

Monitoring the receive into Alice

You will now receive the bitcoin into your Alice wallet, in Sparrow. No matter where the bitcoin originally came from, here’s what you should see as the transaction goes through.

If you’ve chosen to pay a higher fee for a quicker transaction, it’ll all happen within about 10 minutes. Otherwise it will take longer.

1.  The first step is that you get a pop-up notice in the top right corner, in Sparrow. It’ll have a message entitled “New mempool transaction”, and the amount of the transaction. These Sparrow notifications disappear after a few seconds.  
    That means your transaction is in the mempool. (See the below section “Learn more: Mempool and Blockchain” for more info.)
2.  Once you’ve gotten the pop-up notice in your Alice wallet, click on the blue **Transactions** button on the left. You should have one transaction in there, from the transaction you just made. The transaction will show up in light gray at first.
3.  You’ll receive another pop-up notification in Sparrow when the first confirmation occurs, which is usually in about 10 minutes. Six confirmations is usually considered final, and then the transaction in Sparrow will switch from light gray to black.
4.  Notice that in the Transactions window, there’s a US dollar amount in there. For the dollar amount, the current bitcoin price is used. (To set up a different default currency, go to File > Settings > Currency.)

Congratulations! You now truly own some bitcoin, it’s on your own personal wallet, and you have the private key.

Troubleshooting your connection in Sparrow

This was also mentioned in Exercise 1, but here’s a reminder, because it happens often. You may notice that a transaction doesn't show up when it should. If this happens, check the slider at the very bottom right corner in Sparrow. If it's gray, you have lost your connection. This can happen sometimes, especially after restarting.

To fix this, click on the slider to reconnect.

Learn more: Mempool and blockchain

The mempool is a holding area for bitcoin transactions that have been submitted, but not yet added to a block. It’s like bitcoin’s waiting room—an area where transactions sit before being included in a block. When you send bitcoin, your transaction joins others in the mempool, waiting for bitcoin miners to pick them up.

After a miner picks them up and confirms them in a new block, the block gets added to the bitcoin blockchain. This means that the transaction has one confirmation. When another block gets added to the blockchain, your transaction will have two confirmations. Once it has six confirmations, most people consider that “final settlement”—in other words, it’s almost impossible to reverse.

What is the blockchain? It’s like a giant public notebook, or ledger, of all the transactions that have ever occurred. By looking at the blockchain, you can see exactly what the transactions were, the amounts of the transactions, and the sending and receiving address.

You pay a fee, called the transaction fee, for having your transaction included in the next block, and added to the blockchain. This can be higher or lower, depending on how much competition there is for transaction space in the bitcoin blockchain. Transactions that include higher fees usually get chosen first by the miners, and go into the very next block. Lower-fee transactions wait longer. We’ll discuss fees in more detail later.

Learn more: bitcoin mining

Just now, in the section on Mempool and blockchain, the term bitcoin miners came up. What is, actually, the process of bitcoin mining?

Basically, bitcoin mining happens with a decentralized network of special computers (“miners”), all around the world. These miners are competing to solve a mathematical problem, every 10 minutes. Whichever computer finds the solution first gets to “mine” the next block of transactions, which means linking the new block to the previous one in the blockchain.

Bitcoin mining takes special, expensive computers, and lots of electricity. The reason that the miners do this work is that they earn bitcoin in two different ways, each time they mine a block.

*   First, there’s a reward in bitcoin, for the computer that mines that block. This reward is substantial. In 2025, each mined block earns 3.125 bitcoin.
*   Also, the successful miner gets to keep the transaction fees associated with the block.

The reward in bitcoin for the successful miner is straightforward, it’s just a set amount.

The transaction fees are more complex. Every single transaction needs to pay a fee, to pay for the work of putting it in the block. And transaction fees depend on how busy the network is. If many people are trying to make transactions, fees go up because there’s more competition for a scarce resource—space on the bitcoin blockchain.

It’s similar to when a city is hosting the Olympics. Hotel rooms will get much more expensive because there’s only a set amount of them. Similarly, you will have to pay more in transaction fees when the bitcoin network is congested.

Luckily, it’s now (in 2025) a period of relatively low fees, so the transactions you’ll be making in these exercises will be relatively inexpensive.

# Exercise 5: Recover your Alice wallet

Being able to recover your wallet is an important step in Bitcoin security. If something unexpected happens, you need to be able to gain access to your bitcoin again with just your seed phrase.

So, practicing recovery is a must, when learning to use bitcoin.

1.  In Sparrow, click on **File > New Wallet**. Name the wallet “Alice Recovery” and click on **Create Wallet**.  
    Note that we’re creating a new wallet file in Sparrow here, but it will be derived from the original Alice wallet, and will have the same seed phrase (private key).
2.  You’re now in the Settings window. Leave the settings as they are (Single Signature, Native Segwit). At the bottom in the Keystores section, click **New or Imported Software Wallet.** In the next window, look for the button on the top right that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.
3.  Enter in the 12 words you wrote down in the exercise “Create a wallet in Sparrow—Alice”. Don’t create a passphrase. Click the **Create Keystore** button.
4.  Leave the derivation path at the default of m/84’/0’/0’, and click on **Import Keystore**.
5.  Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the “Wallet Password” screen.
6.  You have now recovered your Alice wallet. Click on to the blue Transactions button on the left, to switch to that window. You should be able to see the transaction you made earlier.
7.  Also check the addresses, between the original and the recovered wallet. To do this, open the original Alice wallet, and click on the blue Address button on the left. Do the same in the Alice Recovery wallet.
8.  Cross check the first few Receive addresses between the two wallets. Make sure they’re the same. If the addresses are the same, and you see the previous transaction, you’ve restored the wallet correctly. Congratulations!

Learn more: wallet recovery

It’s good to practice recovering a wallet occasionally. If you lose your computer, or the Sparrow wallet file, or lose your hardware wallet, you can still recover your wallet—but only if you kept the seed phrase safe.

But if a disaster happened _and_ you didn’t have your original seed phrase or a backup, then unfortunately you’ve lost your funds. You no longer have access to your bitcoin, and you can’t recover from that.

Common problems when recovering wallets

Some of the common problems that occur when recovering wallets are:

*   Missing a Passphrase
*   Differences in Script Type

We’ll go over both of these issues in more depth in upcoming exercises.

# Exercise 6: Create wallet Bob

In this step, you'll create the Bob wallet—a completely new wallet, with its own seed phrase. You’re doing this so that you can simulate having another, separate bitcoin user. In future exercises, you'll practice sending bitcoin from Alice to Bob.

1.  Click on **File > New Wallet**. For the wallet name, type “Bob”, and click **Create Wallet**. In the Settings window, leave everything at the defaults.
2.  Below in the Keystores area of the Settings window, choose **New or imported software wallet.**
3.  In the next window, look for the button that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.
4.  A screen will pop up with 12 blank spaces for your words. Click **Generate New** to have Sparrow auto-generate them, and ignore the “Use passphrase?” option. Now Sparrow has generated a list of random words for your seed phrase.
5.  Write down the words on a sheet of paper, numbering them correctly. Label the words on the paper “Bob Seed phrase”.
6.  Once you’ve written down the words, click on **Confirm Backup**. Confirm on the next screen that you’ve written them down, and click **Re-enter Words**.
7.  In this next screen, re-enter the 12 words. Then click on **Create Keystore**, then **Import Keystore** in the top right.
8.  Now back at the Settings screen, you need to apply all the changes you’ve made. Click **Apply**, on the bottom right. In the Wallet Password screen that comes up next, click **No Password**.

With these steps you’ve created a second bitcoin wallet on Sparrow, one that we’ll use for sending and receiving along with your first wallet, Alice.

Learn more: Privacy and security

So far, you’ve created two wallets with separate seed phrases, the Alice and Bob wallets. (The Alice Recovery wallet was based on the Alice wallet seed phrase).

Seed phrases in bitcoin are very important to keep private and secure. You also need to back the seed phrase up properly. There’s lots of information to absorb on this topic, and bitcoiners often discuss it at great length.

Later on in this book, we’ll go into this topic in more depth. For now, though, don’t worry too much about privacy and security. The wallets that you’re creating now are both small and temporary, so security isn’t that much of a concern. You only need to be as careful as you would be for the same amount of cash.

But when you have long-term wallets that will contain larger amounts of bitcoin, you need to be more aware of security. There’s an upcoming section later on, with more information on keeping your seed phrase safe.

# Exercise 7: Your first send—transfer bitcoin from Alice to Bob

In this exercise, you’ll practice sending bitcoin from the Alice wallet to the Bob wallet. In other words, you’re simulating Alice sending some bitcoin to Bob.

The main thing that would be different if there were really two separate people involved, is transferring the receive address. Instead of being a simple copy/paste of a receive address between two wallets on your computer, it would involve transferring the receive address between 2 different people. You could do this with an email, but more private options like a QR code would be better.

1.  Make sure the Alice and Bob wallets are open in Sparrow. You can close the Alice Recovery wallet.
2.  In the Bob wallet, click on the blue **Receive** button on the left. In the Label field, type in “receive from Alice”. Then go to the Address field, and copy the address to the clipboard.
3.  In Alice, click on the blue **Send** button on the left. In the “Pay to:” text box, paste the receive address from Bob. Enter “send to Bob” in the Label field.  
    Remember, don’t skip the label! In following exercises you’ll need them.
4.  Still in the Alice wallet, in the Amount field, enter about half of the sats that you have in Alice.  
    If you don’t remember how many sats are in Alice, an easy way to do that is to click the Max button to the right of the amount. Then, divide that in half. It’s best for privacy to not send a rounded amount—for instance, instead of 25,000 sats, send 24,359. Sparrow recommends this for privacy.
5.  For now, we’ll leave the Fee set to the default.  
    (You’ll learn more later, but for now, just know that the fee is what the miners receive, for running their specialized computers to process bitcoin transactions. By default, Sparrow will suggest the fee amount that gets the transaction processed into the next block. A lower fee will often still get processed, but won’t necessarily get into the next block.)
6.  In the bottom right corner, click **Create Transaction**. Sparrow will pop up a Transaction window, with details of the transaction. We don’t need to go through all the details right now.
7.  Click **Finalize Transaction for Signing**, then **Sign**. When you sign a transaction, you’re using your private key to authorize it with a digital signature. Sparrow has access to the private key because you’re using a software wallet, and the private key (derived from the seed phrase) is stored with it.
8.  Now click the **Broadcast Transaction** button. This is the last step, and sends the fully signed transaction out to the Bitcoin mempool.  
    (Is the Broadcast Transaction button missing? Check the troubleshooting section below.)

After you click the Broadcast Transaction button, you should quickly see 2 notifications pop up on the top right corner of your screen. One will show a debit for the Alice wallet, because we sent bitcoin out of it. The other will show a credit for the Bob wallet, because it received the bitcoin. This first pop-up is just to show that the transaction has been received into the mempool. It doesn’t mean it’s been confirmed, that’ll come in about 10 minutes.

Troubleshooting: Broadcast Transaction button isn’t visible

After you sign the transaction, the next thing you should see is a Broadcast Transaction button. If you don’t see that, your connection may have been lost.

Check the slider at the very bottom right corner in Sparrow. If it's gray, you have lost your connection. This can happen sometimes, especially after restarting.

To fix this, click on the slider to reconnect.

Learn more: addresses

Bitcoin receive addresses are unique identifiers (strings of letters and numbers) that bitcoin can be sent to, by anyone. One private key has many different addresses. Addresses should never be reused, because that makes your transactions much less private.

In Sparrow, in the Bob wallet, click on the blue Addresses button on the left. Notice that you don’t have just one section for addresses.

Instead, you have two sections for addresses, the Receive and the Change addresses, and they both have multiple addresses. And that’s not all—there’s essentially an unlimited number of addresses that can be generated, via some complex math, by the extended private key, which is represented by your seed phrase.

The **receive address** in Bitcoin is an address that’s designed for incoming transactions.

The **change address**, on the other hand, is specifically set up for when you send bitcoin, and then receive change back from the transaction. Because of some of the internals of bitcoin, you almost always send a larger amount than what you want to spend. It comes back as “change”, to one of the change addresses in your wallet.

It’s like paying for a $1 pack of gum with a $100 bill, and receiving $99 dollars back in change.

Almost all of your addresses in Bob are unused right now, except for

*   the one used for the first receive into the Alice wallet
*   one or more change addresses, that happen as a result of your first send in this exercise

Exercise 8: Review the Alice to Bob transaction

Let’s review the transaction you just made.

1.  In the Bob wallet, click on the blue **Transactions** button on the left. There is a Balance at the top of the Transactions. You can see the total either in Bitcoin or sats. (A sat is a fraction of a bitcoin, each 1 bitcoin has 100 million sats.)
2.  Your transaction may not have any confirmations yet. As it gets confirmations, the circle next to the Value begins to fill in. When it gets 6 confirmations (in about one hour) it will be considered “final settlement”, and the text for the transaction will switch from gray to black.
3.  To the right of the Balance label, **click** **on the actual number amount**. Notice that the numbers switch, from sats to BTC and back. My preference is to see the balance in sats, because it’s easier to read small amounts. The transaction you just made will be at the top.
4.  You also see the transaction amount in USD (or whatever you have set up as the currency in the Settings menu).
5.  Open the Alice wallet and click on the blue Transactions button. Again, the transaction you just made will be at the top. But it will not show the exact amount that you sent in sats. Instead it will show more. You spent more from Alice than what Bob received. The difference is the fee you paid, to get the transaction processed.  
    How much was the fee for this transaction?
6.  Still in the Alice wallet, hover your cursor on the transaction date/time of the transaction you just made. There will be a little magnifying glass to the right. **Click on the magnifying glass**, to pop up transaction details.

*   This screen is similar to what you saw in the previous exercise, when you were creating the transaction. But now you’ll see a Blockchain section at the bottom. (This is visible once the transaction has at least one confirmation).
*   The Blockchain section shows you the status of the transaction, how many confirmations there are, and also some information about the block containing your transaction—the block height, and timestamp.  
    Also, below the Blockchain section you see a section with a lot of colored numbers and letters, which is how the transaction appears in the blockchain. You can ignore it.

Learn more: permissionless transactions

You control both the Alice and Bob wallet, so sending a transaction between them is just sending to yourself. But you could just as easily have sent bitcoin to a wallet owned by someone else. It would have been the exact same process.

There are only four things you need to make bitcoin transactions to any corner of the globe.

*   Bitcoin that you truly own, and have the private key for
*   Bitcoin wallet software
*   An internet connection
*   The bitcoin address you want to send to

If you have these things, you can send bitcoin to anyone, anywhere, anytime. The Bitcoin network is running 24/7.

One of the most important benefits of bitcoin is that no permission is needed, in order to make transactions. Bitcoin is what’s called a “bearer asset”. Whoever actually owns the bitcoin (in other words, has the seed phrase/private key) can spend them, with no intermediaries like government, banks or any other financial institution. In this way it’s similar to cash or gold bars.

Government currencies like the US dollar—often called fiat currencies—are tightly regulated. With government currencies, there are many ways that you could be blocked from accessing your own money. For example, during protests like the Canadian Truckers Protest, some protesters, or those people who wanted to donate to protesters, found their bank accounts frozen or restricted.

Also, transactions between different countries are frequently controlled. These types of regulations are called capital controls. If there’s a way for access to your money to be blocked, it’ll probably happen at some point. Capital controls and events like the Canadian Truckers Protest of 2022 have demonstrated that the only assets that _truly_ belong to you, are the ones that you control.

Luckily, there’s Bitcoin. And with Bitcoin, it’s impossible for someone to prevent you from accessing and spending your bitcoin—assuming you control your private keys.

# Exercise 9: Explore the Settings window of the Alice wallet

In this exercise, we’re going to get familiar with a few of the items in the Settings window of the Alice wallet. We won’t go into all of these settings in depth—this is just to get an overview of the settings you’re most likely to use.

1.  In Sparrow, make sure you have the Alice wallet open. The first option is **Policy Type**. With Policy Type you can choose between Single Signature and Multi Signature. Single Signature is the most common and simplest, and that’s what we’ll be using in this book.  
    Multi Signature is much more complex, and requires multiple different private keys. It’s for people with significant assets in bitcoin, who need more security.  
    (Warning: If you’re experimenting and switch to Multi Sig, it’ll look as though you lost your seed. Just close and reopen the wallet, and it'll be fine)
2.  Next is **Script Type**. Native Segwit is what we’ll be using now, and that’s the default in Sparrow and most bitcoin wallet software. But it’s useful to know that using different or incorrect script types can cause problems. This happens occasionally when trying to restore a wallet.
3.  The **Descriptor** is a way of encoding information about your wallet, in a way that it can be easily transferred between two different bitcoin wallet applications. We’ll be using it in upcoming exercises.
4.  Inside the Keystore area on the Settings window, you can click on the **View Seed** button and easily see the seed phrase you wrote down earlier.  
    This isn’t secure, of course, but since this is a low-risk wallet (both temporary and containing only a small amount of bitcoin), you don’t need to worry about it now. Later on, you’ll want more security, and we’ll review other options.
5.  The **Label** is mostly a way of distinguishing between different wallets. By default with this type of wallet, it’s set to BIP39, but you can change it. It’s used mostly with Multi Signature wallets.  
    The **Master Fingerprint** is similar to the Label, in that it uniquely identifies the wallet. But Master Fingerprint is system generated, as opposed to being something you can edit.
6.  The **Derivation** field is basically the method that Sparrow uses, in order to figure out how to create addresses from the seed phrase. We’ll mostly be using the default. But if you’re recovering a wallet and the derivation for a wallet isn’t correct, then the addresses won’t be correct either. And then no transactions will be found.
7.  At the bottom, there’s a field labeled **xpub/zpub**. This is usually called the **public key**. We’ll be using it in the next exercise.

**Congratulations!**

You've completed the beginner exercises, and have mastered some basics.

Are you enjoying this book so far? I'd love for you to share your thoughts with a review on Amazon!

If you have feedback on the exercises, please let me know. Contact me at [feedback@BitcoinHandsOn.com](feedback@BitcoinHandsOn.com).

Exercise 10: Create watch only wallet based on Alice

In this exercise you’ll create a special kind of wallet, a watch only wallet. It’ll be based on the Alice wallet you created earlier.

Why create a watch only wallet? The main reason is to keep your seed phrase—that extremely important set of words—secure, private, and not exposed very often.

In a watch only wallet you can do many of the tasks that you need to do in a wallet, like receive bitcoin, and monitor transactions. The only thing you can’t do is spend bitcoin.

It’s common to create a watch only wallet for your main wallet. A watch only wallet is not a “hot wallet”. This means that it does _not_ hold your private key. And there’s no “View Seed” button in the wallet, like we saw in exercise 9.

However, you can still see the transactions and addresses, though you can’t spend. So, it’s more secure to have a watch only wallet set up on your computer than it is to have an actual “hot” wallet, which is what your Alice wallet is.

To create the wallet, follow these steps:

1.  Open Sparrow. Close all wallets except the Alice wallet.
2.  Click on File > New Wallet. Name it “Alice Watch Only”.
3.  In the new wallet, you’ll end up on the Settings window. In the Keystore section, click on **xPub / Watch Only Wallet**.
4.  Now, open your Alice wallet, if it’s not already open. Click on the blue **Settings** button to go to the Settings window in your Alice wallet.
5.  In the Keystores section of the Alice wallet, at the bottom, is the xpub/zpub, which is the public key. **Copy the public key**, and then switch to the Alice Watch Only wallet. **Paste it** in the xpub/zpub text box.
6.  Click **Apply,** to create the Alice Watch Only wallet.
7.  On the Wallet Password screen, click **No Password**.

You’ve now successfully created a new watch only wallet in Sparrow. You should be able to see, in the Transaction window of the Alice Watch Only wallet, the same transactions that you see in the Alice wallet.

Learn more: Public keys, watch only wallets, and privacy

A watch only wallet is created, as you saw above, with the public key. Sometimes in more technical discussions, it’s called extended public key, or master public key, but I’ll use the term public key in this book.

In Bitcoin, your public key is similar to an account number. From it, you (or anyone) can generate addresses, and use those addresses to send you bitcoin. And because they see your addresses, they can track your transactions on those addresses.

Your public key is generated _from_ your private key with some complex math, but can't be reversed to reveal your private key. And without your private key, your bitcoin cannot be spent. Still, you don’t want to expose your public key, because anyone who knows it can track all your bitcoin addresses, and all your transactions.

So, for the sake of privacy, make sure that you keep your public key a secret.

One common use of watch only wallets is to generate receive addresses. We’ll talk about this more in an upcoming exercise.

# Exercise 11: Explore the Alice Watch Only wallet

In this exercise, we’ll explore the Alice Watch Only wallet, and compare it with the original Alice wallet.

1.  In Sparrow, open the newly created Alice Watch Only wallet, and also the original Alice wallet.
2.  In the Alice Watch Only wallet, click on the blue **Transactions** button on the left. You should see two transactions there. The first is when you received bitcoin from your original source. The second is from sending bitcoin from Alice to Bob.
3.  Look for labels in the Transactions. Do you see any?
4.  Now switch to the original Alice, and click the blue **Transactions** button. You’ll see the two transactions there, with identical amounts. What do the labels look like?
5.  If the transactions are visible, then the Alice Watch Only wallet should be set up correctly. But let’s check the addresses anyway. So, switch to the original Alice wallet, and click on the blue **Addresses** button on the left. Do the same in the Alice Watch Only wallet.
6.  **Review** that the first few Receive addresses are identical, between the two wallets. If the addresses are identical, and you see the previous transactions, then the watch only wallet is set up correctly. (The labels will be missing on the watch only wallet, though, just like they’re missing for the transactions.)

Learn more: Why are the labels missing?

Why do the labels only show up in the Alice wallet? It’s because the label isn’t part of the bitcoin blockchain. The label is stored inside the Sparrow wallet file, and not on the blockchain.

When you’re recovering a wallet from a seed phrase, or creating a watch only wallet, all the information you see comes from the bitcoin blockchain, because that’s where it’s fetched from. Recovering a wallet from the seed phrase, or creating a watch only wallet—both of these will generate a list of addresses. When those addresses are checked in the bitcoin blockchain, it gives you any transactions (along with the amounts and dates) associated with the addresses.

What you’re explicitly _not_ getting is information that’s stored in the Sparrow wallet file, such as labels from transactions or addresses.

Here’s another thing to note about the label—the transaction gets the label from the original address. For instance, when you set up your initial receive transaction, from the exchange to your Alice wallet, you entered a label for the receive address. This label shows up as the label for the transaction as well.

Learn more: checking receive addresses

The last step in this exercise was to compare addresses. What’s the point of comparing the receive addresses between the Alice wallet, and the Alice Watch Only wallet? You did the same thing in Exercise 5: Recover your Alice wallet.

Here’s the reason you compare the addresses. If any of the settings of the wallet are different (such as the script type, or derivation path), then the addresses will be different. In order to make sure that it’s set up correctly, you check to make sure that the first few addresses are the same between the two wallets.

In this case, it’s not strictly necessary because you already see the transactions in the watch only wallet. This means that Sparrow used the correct addresses, and found the correct transactions. But it’s definitely a good idea to remember to check addresses, whenever creating a watch only wallet.

# Exercise 12: Receive bitcoin via a watch only wallet

Getting receive addresses is one of the most important uses of a watch only wallet. This exercise demonstrates how to receive bitcoin to a wallet, without even having it open (and potentially exposed).

In order to do this, we use a watch only wallet.

1.  In Sparrow, open the Bob wallet, and the Alice Watch Only wallet. Close all other wallets, especially the Alice wallet.
2.  Go to the Alice Watch Only wallet. Click on the blue **Receive** button on the left. For the Label field, type in “Send from Bob to Alice Watch Only”. And now, copy the contents of the Address field.
3.  Now switch to the Bob wallet, and click the blue **Send** button on the left. Into the Pay to field, paste the address you just copied from Alice Watch Only. Type the same text in the Label, “Send from Bob to Alice Watch Only”.
4.  In Amount, enter the number of sats that you’ll be sending to Alice Watch Only—about half of your balance.
5.  Click **Create Transaction** on the bottom right. On the next screen, click **Finalize Transaction for Signing.**
6.  Now click **Sign**, in the bottom right corner. Then click **Broadcast Transaction**. Remember, if the Broadcast Transaction button is not visible, you may need to reconnect with the slider at the very bottom right.

This sends the transaction that you just created to the bitcoin mempool. Because you have the two wallets that are involved in this transaction open, you’ll get two pop-up notices from Sparrow. One will have a negative amount for the Bob wallet, the other will have a positive amount for the Alice Watch Only wallet.

From there, the transaction will soon get added to a block, and be incorporated into the blockchain. You’ll receive two more notices (one for each open wallet) when the first confirmation happens, usually in around 10 minutes.

Learn more: Receive addresses from watch only wallets

Getting receive addresses via a watch only wallet is very common. For instance, say that somebody wants to pay you in bitcoin. If you have your watch only wallet set up, you can give them a receive address, using _only_ the watch only wallet. You may want to do this because as you acquire more bitcoin, you’ll set up your wallet much more securely than your current wallets. You may have it hidden away somewhere, or in a safe.

In general, you want to keep your bitcoin wallets secure, and that means not opening them frequently. A watch only wallet, set up with the public key of your main wallet, can prevent you from needing to open your wallet just for a receive address.

Of course, before relying on a watch only wallet like this, make sure that the watch only wallet is set up correctly. It’s important to check that the receive addresses are identical to the original wallet.

# Exercise 13: Use the Alice Watch Only wallet to send a transaction

In this exercise, you’ll explore what happens when you try to actually send a transaction, using the Alice Watch Only wallet. This will deepen your understanding of the situations in which you might choose to use watch only wallets.

1.  Make sure the Alice wallet is closed. (If you don’t close it, this exercise won’t show the expected results.)
2.  Make sure the Alice Watch Only and Bob wallets are open.
3.  In the Bob wallet, click on the blue **Receive** button on the left, and copy the Address that’s shown.
4.  Switch to the Alice Watch Only wallet, and click on **Send** on the left. In the Pay to field, paste the receive address you got from the Bob wallet. Also add an amount—make it about half of what’s currently in Alice. For Label, type in “Send via Alice Watch Only”.
5.  Click **Create Transaction** at the bottom right, then **Finalize Transaction for Signing**.
6.  Now click **Sign**. What happens?

If you’ve done all the previous steps, Sparrow will pop up this message “Connect Hardware Wallet”.

Here’s why this is happening. Sparrow is not able to provide signing authority for the Alice Watch Only wallet, because it doesn’t have the private key for it, since it’s a watch only wallet. Often, to provide a private key to send from a watch only wallet, you would connect a hardware wallet.

For a watch only wallet, Sparrow only has the public key, from which it can look up the addresses associated with that key. But it cannot sign any transactions to send from those addresses.

Try again

Now, try the exact same process, using the same steps above, with one change—make sure the Alice wallet is _open_, instead of closed.

Notice that when you’re on the screen that has the “Finalize Transaction for Signing” button, there’s a “Signing Wallet” dropdown, just above the button. Sparrow has determined that the Alice wallet has signing authority, and makes it the default signing wallet, even if you created the transaction from the watch only wallet.

Now, after you click Sign, Sparrow _does_ allow you to sign. If you choose to, you can continue and actually click **Broadcast Transaction** to complete the transaction. Even though the transaction was started from Alice Watch Only—as long as the Alice wallet is open in Sparrow, it will be used to do the signing.

# Exercise 14: Create wallet Bob Legacy Script Type

This exercise will show you what happens if you restore a wallet via a saved seed phrase, but use a Script Type that’s different from what the wallet was created with.

It’s important to understand this situation, because many people have “lost” bitcoin, through recovering the wallet with the wrong script type. The funds aren’t truly lost, it’s just that the wallet needs to be set up correctly. Relying on another person to help you in this situation introduces risk—it’s best to understand how to fix it yourself.

The seed phrase you’ll be working with is the one for the Bob wallet.

1.  Open Sparrow, and close all open wallets. Click on **File > New Wallet**. For the wallet name, type “Bob Legacy Script Type”, and click **Create Wallet**.
2.  Next in the Settings window, for the first time we will change one of the defaults. Click on **Script Type**, and choose **Legacy (P2PKH)**.
3.  Below in the Keystores area of the Settings window, choose **New or imported software wallet**. Now look for the button on the top right that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.
4.  Enter the 12 words you wrote down in the exercise “Create a wallet in Sparrow—Bob”. Don’t create a passphrase. Click the **Create Keystore** button.
5.  Leave the derivation path at the default of m/44’/0’/0’. Note that it’s different from the derivation path you saw in other wallets. Click on **Import Keystore**.
6.  Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the Wallet Password screen.

With these steps you’ve created another wallet, based on the Bob seed phrase (private key). You’ve basically “recovered” a wallet, like you did in a previous exercise.

However, this wallet uses a different script type. Let’s do some checks here, to see how the script type affects the wallet.

1.  Open up the original Bob wallet.
2.  Click on the blue Transactions button in the original Bob wallet, and compare the transactions to those in the new Bob Legacy Script Type wallet. What do you see?
3.  Compare the addresses in Bob to the Bob Legacy Script Type wallet. Notice that they’re in a different format. In the original Bob wallet, they all start with bc1. Also, the rest of the address is different as well.

The Transactions screen in the new wallet should be empty, with a zero balance. Even though you used the same exact seed phrase, the addresses are different if the script type is different. Sparrow checks the blockchain only for those addresses that it knows about. And it uses the script type to generate the addresses, so it gets different addresses when the script type is different.

Learn more: Script type problems

The most important thing to remember about script type is that whenever you’re recovering a wallet, or using a watch only wallet, you _must_ match the script type (and other settings, like the Derivation) with the original wallet.

Bitcoin script types define address formats and spending rules. The default now, in 2025, is Native Segwit, but earlier it was different.

This should happen by default, in most modern bitcoin wallet software, but it’s best to check.

This situation—having different script types when you’re trying to recover a wallet—has caused many people anxiety. Maybe you _know_ that you wrote down and entered the seed phrase correctly, but you just don’t see any transactions when you know there should be some.

But it may be that when you created your wallet, the software you used had one particular default script type. And then in the software you used to recover it, the default script type is different. That causes the addresses to be different, which causes the transactions to not be found. When the transactions can’t be found, your wallet shows a balance of zero.

You won’t have an exercise on this, but the derivation setting is similar to script type. If you restore your wallet with an incorrect derivation, you will get different addresses, and will not see your bitcoin.

It’s important to know that getting the Script Type or Derivation wrong is not bad in the same way as losing your seed phrase. If you have completely lost your seed phrase, there is no chance at all of recovering your bitcoin. But if there’s a script type mismatch, you just need to fix that one thing, and you’ll be fine.

# Exercise 15: Create wallet Alice With Passphrase

In this exercise, we’ll be exploring what happens when you add a passphrase on top of your seed phrase.

Remember, the passphrase is different from the password. A passphrase actually _changes_ your private key. It’s as though you had a completely different seed phrase. But the password, in Sparrow, just unlocks the wallet file so it can be opened.

Awareness of the potential complexity of a passphrase in bitcoin goes a long way in avoiding problems.

1.  Open Sparrow. Close all other wallets, and go to **File > New Wallet**. For the wallet name, type “Alice With Passphrase”, and click **Create Wallet**. Leave everything at the defaults in the Settings window.
2.  Below in the Keystores area of the Settings window, choose **New or imported software wallet.**
3.  In the top right of the next window, look for the button that says Use 24 words and **click the arrow to the right.** Choose **Use 12 words** instead.
4.  Enter the 12 words you wrote down in the step “Create a wallet in Sparrow—Alice”.
5.  Here’s the critical step—this time, go ahead and **click the “Use passphrase?” checkbox**, at the bottom of the words you wrote down. A window titled “Add a passphrase?” will pop up, with some warning text. Sparrow will ask you to confirm that you want to create a passphrase. Click **Yes** to confirm.
6.  Now enter your passphrase. The passphrase is not limited to the BIP39 word list, you can type anything you want in there, including numbers and symbols. It’s also case-sensitive. For now, keep it simple by putting in “**MyPassphrase1234**”. Write down the passphrase on a sheet of paper, and label it “Passphrase for wallet Alice With Passphrase”.
7.  Click the **Create Keystore** button, then the **Import Keystore** button. You’ll be asked to re-enter the passphrase. Re-enter and click **OK**.
8.  Now at the bottom right corner of your screen, click the **Apply** button. On the next screen, click **No password** on the “Wallet Password” screen. (Remember, this is the _password_ on the wallet file, it’s not the _passphrase_.)
9.  Now click on the Transactions button. Do you see any transactions? There should be none.

Learn more: passphrase and password

The reason you don’t see transactions in the step above is that with the passphrase on the original seed phrase, you’ve created a completely different private key, with different addresses. When Sparrow looks up those addresses on the blockchain, there’s no transactions associated with them.

The _password_ (as opposed to passphrase), in Sparrow, is just an extra piece of security that you can put on your wallet file. If you lose the password, but still have the seed phrase, you can easily restore the wallet.

In contrast, the passphrase is a special concept in bitcoin. When you create a wallet with a certain seed phrase, and no passphrase, you generate a specific private key. But when you create a wallet with the exact same seed phrase, and add a passphrase, you get a completely different private key.

Beginners and experts alike often have problems with passphrases. It can seem like a good idea to get some extra security on the seed phrase.

But apparently this particular issue—setting up a passphrase and then forgetting it—is _the most common problem_ that causes people to lose their bitcoin in self custody. People think they’ll always remember the passphrase, then their memory fails them.

The bottom line? **Don’t use a passphrase unless you’re an expert**, and completely understand the risks.

# Exercise 16: Review some transactions

In this exercise we’ll be reviewing some of the transactions that have occurred, and learning more about how transactions work. You don’t need to know every single detail on this topic, this is just to get an overview.

Understanding how transactions work will give you a better grasp of how to begin optimizing for lower fees and privacy.

Review your initial transaction into the Alice wallet

Let’s take a more detailed look at the very first transaction that you made, when you received your first bitcoin into the Alice wallet.

1.  In Sparrow, open the Alice wallet. Click on the blue **Transactions button** on the top left in Sparrow. Go to your earliest transaction.
2.  Hover your cursor over the date of that transaction, and a little magnifying glass will pop up on the right. Click on the **magnifying glass** to view details about the transaction.
3.  The fee is at the bottom. The fee is what’s left after the recipients have been paid, and the change has gone back to the change address. The fee goes to the bitcoin miners.
4.  If you purchased the bitcoin from an exchange, it can look somewhat complex. It’s likely that there will be one input (from your exchange), and many outputs, as the exchange splits the payments to many different people’s addresses.  
    One of these outputs is the one you received, into your address. Your output has a downward pointing arrow icon, the others have what looks like a paper airplane.

Explore an address in Mempool.space

Now you’re going to use the blockchain explorer [https://mempool.space](https://mempool.space) to view transactions. What exactly is a blockchain explorer? It’s a website that allows users to view everything that’s available on the bitcoin blockchain, like transactions, addresses, etc. Mempool.space is the most well-known bitcoin blockchain explorer. Another blockchain explorer is Blockstream.info.

This exercise helps you gain a fresh perspective on blockchain data. By reviewing transactions through a tool other than Sparrow, you develop a clearer understanding of the blockchain. It reinforces the idea that the transactions you’re seeing are part of a global network powered by tens of thousands of bitcoin nodes, all working together to maintain the blockchain network’s stability.

1.  Go to Sparrow, where you have the transaction open for the very first bitcoin you received into Alice. Go to your receive address (the one with a downward pointing arrow icon). Right-click (or Control-click on a Mac), and then click on **Copy Address**
2.  Now in a browser, go to [https://mempool.space/](https://mempool.space/). In the top right, where it says Explore the full Bitcoin ecosystem, **paste in the Address** you just copied. Click the **magnifying glass** to the right, to run the search.
3.  You’ll see a screen full of information about your receive address. It has the current balance, which may not be the same as the original one. You may see more than one transaction, related to this bitcoin address.
4.  Under the Address section, there will be a Transactions section. It will probably say **2 of 2 Transactions**. Click on the **Transaction ID** that’s the same as the TXID you saw earlier in Sparrow. This should also be the _earliest_ transaction for that address.
5.  In Mempool.space **find the number of confirmations** for that transaction. This should be identical to what you see for the same transaction, in Sparrow. The Block (called Block Height in Sparrow, the number of the block that the transaction got into) should also be the same between Mempool.space and Sparrow.  
    The timestamp may not be identical, because of time zone differences.
6.  Scroll down in Mempool.space to the Flow section. This is where you get a comprehensive layout of the entire transaction, with all inputs, all outputs, and fees. Your address will be among the outputs.
7.  Notice that you can see, in the Flow section, any additional transactions that your address (and other addresses that were in the transaction) were involved in.

Learn more: Never reuse bitcoin addresses

As you saw in the exercise above, it’s simple to track bitcoin, if you know the bitcoin address. The fact that no history is lost in the bitcoin blockchain is another reason to be careful about your privacy. One of the ways to improve your privacy in bitcoin is to never use a bitcoin address more than once.

Never reuse bitcoin addresses

If someone happens to know one of your bitcoin addresses, and if you use that address again and again, they know exactly how much bitcoin you have in it. They also know when you received it, and how much you received in each transaction.

Fortunately, most modern bitcoin wallet software makes it difficult to reuse a bitcoin address. For instance, in Sparrow, when you click Receive, you are given a new receive address, and not one that you’ve used before.

Learn more: Expanding on the Blockchain

In a previous exercise, you learned some of the essentials about the bitcoin blockchain. It’s basically a public ledger, stored and duplicated on an enormous, decentralized network of computers running bitcoin software, all around the world. It records every single bitcoin transaction that has ever taken place, in chronological order. In it you can see all the addresses in the transactions, and the amount of bitcoin associated with each address. And also, it’s completely open to the public—if you had a spare computer, you could run a bitcoin node in your home.

About every 10 minutes on the blockchain, a new block is added on top of the last block. This has been happening with almost 100% reliability ever since bitcoin was first started up in January 2009. When a new block is created and attached to the bitcoin blockchain, it’s like a new link on a metal chain—the new block is attached to the previous block via a mathematical fingerprint.

There’s a popular saying among bitcoiners, “Tick tock, next block”

Tick tock, next block

This saying captures the mindset of bitcoiners. The price might be up or down, but Bitcoin will keep on going. And it will gradually but steadily replace other types of money. No government or corporation in the world can stop bitcoin from being transacted, and new blocks from being added to the blockchain.

# Exercise 17: Send bitcoin from Alice to Bob—review fees

In this exercise you’ll again send some bitcoin from Alice to Bob. Along the way and in the next exercise, we’ll look at fees in more detail. You want to minimize fees in your transactions, and the next exercises will teach you some fundamentals of bitcoin fees.

1.  Open both the Bob wallet and the Alice wallet.
2.  In the Bob wallet, click on the blue **Receive** button on the left. In the Label field, type in “receive from Alice”. Then go to the Address field, and copy it.
3.  In Alice, click on the **Send** button on the left. In the “Pay to” text box, paste the receive address that you just copied. In the Label, type “Send to Bob”. In the Amount field, enter about half the bitcoin you have in Alice.
4.  Now, let’s do some experimentation with fees and amounts to get a sense of how they work.

*   Go to the website [https://mempool.space/](https://mempool.space/) and look at what the estimated transaction fees are, on the bottom left. They range from No Priority to High Priority.
*   Back in Sparrow, take a look at the Fee field. What is the fee? By default, it appears that Sparrow tries to set the fee amount to get your transaction in the “High” or “Medium” priority range. Sparrow is receiving information about the current bitcoin market rate fees from mempool.space, in order to make these recommendations.
*   Change the transaction amount, make it as low as possible. Does Sparrow allow you to spend more on the fee, than you do on the transaction?
*   There’s a slider going from 1 to 50+, to the right of the label **Blocks**. Sparrow often starts out with a setting of 4 blocks—in other words, it sets a transaction fee that’s as low as possible, while still getting the transaction in the blockchain sometime within the next 4 blocks (approximately 40 minutes).

1.  Experiment with this slider. Unless fees are already very low, try moving it to the right, so that it takes longer, but the fees are lower. Only do this for transactions that are not urgent.
2.  After these experiments, you’re ready to actually create the transaction. But first, switch the Amount back to the original amount (about half of what you have in Alice).  
    In the bottom right corner, click **Create Transaction**. Then click **Finalize Transaction for Signing**, and then **Sign** button. By clicking Sign, you’re authorizing the transaction, with your private key.
3.  Now click the **Broadcast Transaction** button. You’ve just sent the transaction to the bitcoin mempool. You’ll get the same pop-up messages that you’ve received before in Sparrow, when sending a transaction.
4.  Check the latest transactions in the Transactions window, in both the Alice wallet and the Bob wallet. You should see the transaction you just made, in both wallets. They will be in light gray instead of black, until they’re confirmed.

**Learn more: Amounts too small to usefully spend—“dust”**

In Step 4, you experimented with lowering the transaction amount—did you notice Sparrow lets you spend more on fees than the actual transaction amount? While possible, you should generally avoid this.

Amounts too small to spend economically are called “dust”. Dust happens when leftover Bitcoin (UTXOs) becomes worthless to move, because the fees exceed the value. It’s like packaging up and mailing a penny, but spending $1 on postage. Whether or not a chunk of bitcoin is “dust” depends on how high transaction fees are at the time.

If you're interested, consider exploring this topic online (search for UTXO and dust).

# Exercise 18: Bitcoin fees—what you pay, and why

Now’s a good time to learn more about bitcoin fees. Transaction fees, of course, directly affect how much you need to pay to process your bitcoin transactions.

This is a good time to remember that we’re paying fees all the time, to process our transactions. For instance, when you use a regular credit card at a grocery store, you’re usually paying around 2 to 5% in fees. We think that it’s the merchant who’s paying the fees, but in the end, it all comes from the customers.

The good thing about bitcoin fees is that unlike credit card fees, it’s not a percentage of the transaction amount. Instead, it’s based on how much digital space the transaction would take in a block. So, you could potentially transfer huge amounts of bitcoin for a tiny fee.

The metric for the transaction fee in bitcoin is sats/vByte, or sat/vB. A low transaction fee rate would be 1 or 2 sats/vByte. Occasionally, transaction fees can go up very high, but transaction fees are low now (early 2025).

The front page of the website [https://mempool.space](https://mempool.space) has good information on what the current fee rates are. It’s divided up into No priority, Low Priority, Medium Priority, and High priority. The High priority ones will usually make it into the next block.

Mempool.space also has great historical information on fees. To access it, go to [https://mempool.space/](https://mempool.space/) and then click the white Graph icon at the top, then the blue Mining dropdown on the left, and choose Block Fee Rates. Or you can go directly to [https://mempool.space/graphs/mining/block-fee-rates](https://mempool.space/graphs/mining/block-fee-rates).

Do some exploration on the Block Fee Rates page, using the time ranges at the top right (24h, 3D, 1W, etc.), and the bar sliders on the bottom, to learn more about bitcoin fees. Answer the following questions.

1.  In the past 24 hours, at around what time were the highest fees paid? How about the lowest?
2.  For the past month, when were the lowest fees paid?
3.  When were some notable spikes in bitcoin transaction fees, looking at all of the historical data you have available?

Sometimes it’s hard to see the overall patterns because of seemingly random spikes in the fees. Often there’s a spike when there’s a lot of interest in bitcoin and the price is appreciating. Another cause may be NFTs and Ordinals (see below for more info), which are digital items that can cause congestion on the bitcoin blockchain.

In some of the following exercises, you’ll experiment with different fee rates.

Learn more: Bitcoin transactions that are not on the blockchain

It’s important to know that not all transactions have to be logged directly on the bitcoin blockchain. There are other options for sending and receiving bitcoin, on what’s called Layer 2. These transactions are not directly or immediately on the blockchain.

The most popular Layer 2 is the Lightning network. Most smaller bitcoin transactions happen on the Lightning network. There’s more information about Lightning in the [Resources](#Resources) chapter at the end of this book.

Learn more: NFTs, Ordinals, and Runes

When Bitcoin transaction fees spike up, it’s usually from either increased interest in bitcoin, or increased interest in NFTs, Ordinals, and Runes.

NFTs, Ordinals, and Runes are digital items that live on the bitcoin blockchain. Some fans like to buy and trade them—the hope is that like trading cards, they may appreciate in value.

These items take up much more space on the block than a regular transaction, so they make regular transactions expensive. Trading in NFTs, Ordinals, and Runes tends to come in waves. You can see (on mempool.space) a huge spike in bitcoin transaction fees in late 2023 and early 2024. This was caused by trading in NFTs, Ordinals, and Runes.

Learn more: Paying the lowest fees possible

For practical purposes, here’s what you need to remember about bitcoin transaction fees:

*   In the past few years (2024-2025), bitcoin fees have been generally low. They probably won’t cause you much concern.
*   In general, for low transaction fees, do them in the morning on weekends. There’s not as many transactions happening, so competition is lower. Sunday morning in the Eastern Standard time zone can be particularly cheap—you can check historical fees and see that fees at this time are usually low.
*   If you don’t want your transaction to go through immediately, you don’t have to pay the recommended fee amount. In periods of high transaction fees, I’ve input a lower fee, and the transaction has still gone through. It will just take longer, I’ve waited anywhere from an hour to a week.  
    But remember, if a transaction needs to happen quickly, you need to pay the fee to get it included in the next block.
*   If you have a stuck transaction because you set the transaction fee too low, there are some options. One of them is what’s called a RBF (Replace By Fee), another is CPFP (Child Pays For Parent). We won’t get into the details here, but do a search online for either term, along with the keyword Sparrow, and you’ll find some information.  
    **Warning**: I just did the same search that I mentioned above, and the fake, look-alike scam site came up in the search results (sparrowwallet.net). Always be careful where you’re clicking!

**Well done!**

You've completed the advanced beginner exercises, and have developed a good understanding of some important concepts in bitcoin—and of course practical skills.

Are you enjoying this book so far? I'd love for you to share your thoughts and post a quick review on Amazon!

If you have feedback, I'd like to hear from you. Please email me at [feedback@BitcoinHandsOn.com](feedback@BitcoinHandsOn.com).

# Exercise 19: Install Blue Wallet and create the Carol wallet

Your next exercise is to install the Blue Wallet app on your phone, and create a new wallet with it. Blue Wallet is a widely used bitcoin wallet that has a long track record.

Why bother working with another wallet? Wouldn’t it be easier to just stick with Sparrow, since you’ve learned so much about it? Yes, it would be easier. But you wouldn’t learn as much. And you wouldn’t have practiced your ability to restore a seed phrase and test a wallet in an entirely different system. And that’s a _very_ important skill to have, and practice regularly.

Also, learning how a different type of wallet software operates will solidify your understanding of some of the basic concepts of bitcoin—private keys, addresses, and transactions. Comparing two different products helps illustrate these concepts.

Blue Wallet is mostly a mobile wallet, but also has a desktop version for MacOS. We’ll use it on the phone to generate a new wallet, Carol. Just like Alice and Bob, Carol represents a new user of bitcoin. Then we’ll send bitcoin to Carol, and do some other exercises.

Go to the website ([https://bluewallet.io/](https://bluewallet.io/)). Towards the bottom there are links to install it via Google Play or the Apple App Store. Also, you can install it directly on an Android phone, via the APK.

Choose whichever mobile option you prefer, and complete the install. The version that I installed was 7.1.6.

Now, set up the Carol wallet using the following steps:

1.  On a fresh install of Blue Wallet, you’ll see an **Add now** button, to start a new wallet. Click it.
2.  In the Name field at the top, type **Carol**.
3.  There’s an option to choose between a regular Bitcoin wallet, and a Multisig Vault—basically between a single sig wallet, and a multisig wallet. Keep the default of Bitcoin, and click **Create**.
4.  In the next screen “Your wallet has been created”, you’re presented with the seed phrase (Blue Wallet refers to it as a mnemonic phrase). **Write them down** on a sheet of paper, labeled Carol Seed Phrase. Keep this paper safe.  
    **Warning**: Blue Wallet does _not_ ask you to check your seed phrase, unlike Sparrow. Be sure to double check that you wrote it down correctly, because it’s easy to be careless. I just made this mistake myself. One of my words was “two”, and for some reason I wrote down “too” instead of “two”. I would have been without a good backup. Luckily, I had a feeling that I was going too quickly, so I double-checked and figured it out in time.
5.  To make it easier to read amounts, switch from the default, of using BTC as the unit, to sats. To do this, click on the Carol wallet to bring it up. Click on the label that says BTC to the right of the amount field. This will switch between BTC, sats, and USD (or whatever currency you have set up in the Settings).

Learn more: Blue Wallet

Notice that Blue Wallet has many fewer options than Sparrow. There’s only one option for the number of words in your seed phrase (12). And the script type (which Blue Wallet calls Type) is not customizable. You can view the Type, Addresses, and other settings by clicking the three dots in the top right corner, when the wallet is open.

But Blue Wallet is very straightforward to use, and probably has all the functionality you need for a mobile phone wallet. Like Sparrow, Blue Wallet is also open source, which means that the code is publicly available for review ([https://github.com/BlueWallet/BlueWallet](https://github.com/BlueWallet/BlueWallet)).

Here’s a security tip to keep in mind: Whenever you install any bitcoin related software, be very sure that the site you’re installing it from is the real one. For Sparrow, you went to the right site—[https://SparrowWallet.com](https://SparrowWallet.com).

If you’re downloading an app, make sure it’s the real thing as well. Often scammer apps will get onto the Google Play Store, or Apple App Store. These apps are designed to look just like the real app. Always double-check with reputable people or established websites to be sure you’re installing the real thing.

Learn more: what is logged in the bitcoin blockchain?

In this exercise you created a new wallet in Blue Wallet. Consider for a moment—is there anything in the bitcoin blockchain, right now, that registers that this wallet has been created?

No, there’s not. This step just creates the wallet in Blue Wallet. You’ve basically just had Blue Wallet create a very large random number for you—your private key, encoded by your seed phrase. You could do this even without an internet connection.

But no actual transactions have taken place. And it’s only the transactions that are broadcast, and logged in the blockchain. The creation of a wallet is not logged in the blockchain.

# Exercise 20: Send bitcoin from Bob in Sparrow to Carol in Blue Wallet

In this exercise, Bob will send some bitcoin to Carol. To simulate this, you’ll transfer from the Bob wallet in Sparrow to the Carol wallet in Blue Wallet. This will be your first transaction into the Carol wallet.

It will also be your first time transacting with a new bitcoin wallet application. These transactions between different bitcoin applications help you learn how to do the essentials using different systems, and strengthen your understanding of Bitcoin as a whole.

Preparing the transaction

1.  In Sparrow, open the Bob wallet, and click on the **Send** button. Close all other wallets.
2.  Switch to the Blue Wallet app on your phone. Click on the **Carol** wallet. It will have zero transactions. Click the **Receive** button at the bottom. You’ll see a QR code, and the matching bitcoin address below that.
3.  When getting the address from Blue Wallet to Sparrow, it’s easiest to use your computer’s webcam, to scan the QR code for the receive address. Switch back to Sparrow. You scan the QR code by **clicking the icon of a camera**, to the right of the “Pay to” text box. Then put your phone screen in front of the webcam, so the webcam can see your phone and **scan the QR** code. You’ll have to experiment with moving your phone around in front of the computer webcam, so it can be read.  
    If your computer doesn’t have a webcam, you can get the bitcoin address from the phone to the computer via sharing (in email, or whatever you normally use). But if possible, use the QR code, it’s easier and more private.
4.  For the **Amount** to send from Bob to Carol, choose about half of the amount of bitcoin that you have in Bob. And instead of sending a rounded amount—for instance, 50,000 sats—remember to send something like 50,924.
5.  In Sparrow, label the transaction **Send to Carol on Blue Wallet**.
6.  Continue in Sparrow to follow all the steps you normally do when sending bitcoin. Click **Create Transaction**, then click **Finalize Transaction for Signing**, then **Sign.**
7.  Before you click Broadcast Transaction, you can review everything about the transaction in the screen above. This can be a good practice in general, to make sure you have the fee and the receive address correct.  
    Once you’ve checked, click **Broadcast Transaction**.

Review the transaction in Blue Wallet

As the transaction gets processed, you can check it in Blue Wallet.

*   Just after the send from Sparrow, you may get a “pending” notification in Blue Wallet.
*   Open the Carol wallet. A transaction should show up in Blue Wallet, once it’s confirmed.
*   If the transaction doesn’t show up, especially after Sparrow shows that it’s been confirmed, you may need to close and reopen Blue Wallet.
*   Click on the new transaction in Blue Wallet. On that screen, you can click on the Details button at the top right. That will give you extra info about the transaction, like the input address, output addresses, etc. It should match exactly what you see in the transaction details, in Sparrow.

# Exercise 21: Send bitcoin from your exchange to Blue Wallet Carol

When you first moved bitcoin from your exchange to your own wallet on Sparrow, you sent about half the amount you purchased on the exchange. This time, you will move the other half, and leave zero bitcoin on the exchange.

In the below instructions, I’m using Strike, on my phone. These are just example instructions—if you’re not using Strike, the sending process will be different from your exchange.

1.  I open Blue Wallet on my phone, and open the Carol wallet
2.  I click the **Receive** button on the bottom. A QR code will pop up, along with the bitcoin address that the QR code points to (starting with bc1). Next, I click on the **bitcoin address**. This will automatically copy it to the clipboard.
3.  Back in the Strike app, I make sure I’m in the Bitcoin section, by clicking **Bitcoin** in the bottom left. I scroll down in the screen and click the **Send button**, then I click on **Bitcoin Wallet.** (The other option is Username, which is an internal Strike send.)
4.  Still in Strike, I click **Paste** at the bottom, to paste in the bitcoin address I copied from Blue Wallet. (There’s also the option to scan a QR code for the bitcoin address here, which I ignore because I’m using two phone apps).
5.  The next screen in Strike is for the amount. I click the **Max** button to transfer the entire amount. Next is the screen to “Select delivery time”, where you can choose Priority, Standard, or Flexible. To avoid high fees, I choose the **Flexible** option for the transfer, which is free in Strike, but of course takes longer. Then I click **Next**.
6.  The final screen is Confirm send. Click **Confirm**. The transaction will either go through very quickly, or be in a pending status for a while, depending on the priority you choose.

You may now get a notification about receiving bitcoin in Blue Wallet. This depends on how quickly your transaction happens, and whether you’ve set up Blue Wallet to receive notifications.

# Exercise 22: Import the Alice wallet to Blue Wallet via the public key

In this exercise we’ll take the public key from Sparrow, and use it to create a new watch only wallet in Blue Wallet. You’ll learn how this works in general, and some of the pitfalls to avoid in the process.

1.  In Sparrow, close any other wallets and open the Alice wallet. Click on the **Settings** button.
2.  In the Keystores section at the bottom, look to the right of the xpub/zpub field for the QR code symbol. Click on the **QR code symbol**, to pop it up for this xpub.
3.  Now open Blue Wallet, on your phone. Click on the **plus symbol** in the top right corner, to add a wallet.
4.  Skip the Name field, and do not click the Create button. Instead, at the very bottom, click **Import**.
5.  In the Import screen, at the bottom, click the **Scan or import a file** button. On your computer, go back to the QR code you brought up in Sparrow, and scan it.
6.  Blue Wallet immediately creates a new watch only wallet for you, with the xpub you imported by scanning. If the transactions don’t appear within a few minutes, close and reopen the app and you should see them.  
    The name of the wallet will be Imported Watch-only, it’s okay to leave it like that.
7.  Do you see transactions in this watch only wallet? You should have the same transactions that you see in the Alice wallet in Sparrow.

Learn More: Different derivation paths = different address

In an older version of Blue Wallet, the steps you just went through would not have worked. You wouldn’t have seen any transactions. This was because if you imported an xpub in Blue Wallet, the wallet would have been set up with a different script type and derivation path. This means the transactions would never have shown up, because different addresses would have been generated.

This caused lots of problems and stress for people who set up a watch only wallet to get receive addresses. They did this to easily receive bitcoin, while not having their seed phrase in Blue Wallet.

But if they used a receive address that they copied from Blue Wallet, the transaction would never have shown up in Sparrow because of the difference in derivation path.

Happily, this problem has now been resolved by Blue Wallet. But always remember to do some checking when setting up a watch only wallet.

*   If there are existing transactions in the wallet, you should be able to see them. If you can’t, there’s a problem.
*   Check that the first few addresses are the same. You know where to find the addresses in Sparrow. In Blue Wallet, click on the three dots at the top right, and then click on Show Addresses.

Before the next exercise, the wallet that you just created needs to be deleted. To do that, follow these steps:

*   Click on the wallet to open it (the name will be Imported Watch-only).
*   Click on the three dots in the top right corner, to get to the settings screen. Click on the three dots in the top right corner again, and you’ll find a red Delete option. Click it.
*   Blue Wallet will ask you to confirm. Click “YES, DELETE” to confirm.

# Exercise 23: Import the Alice wallet to Blue Wallet via the descriptor

Now you’ll take the public key from Sparrow via the descriptor field, and use it to create a new watch only wallet.

The descriptor in Sparrow is like an expanded version of the public key, which gives complete details about the setup of the wallet. Not only does it include the public key (xpub/zpub), it also includes the derivation path, the script type, etc. It makes interoperability between different wallet applications much easier.

When creating a watch only wallet, use the descriptor when possible. This means you don’t need to worry about compatibility, and matching all the settings exactly.

1.  Open Blue Wallet, on your phone. Click on the **plus symbol** in the top right corner, to add a wallet.
2.  Ignore everything but the **Import wallet** button at the very bottom. Click on it.
3.  In the Import screen, at the bottom, click the **Scan or import a file** button.
4.  On your computer, go back to the QR code you brought up in Sparrow, and scan it with your phone.  
    If you have a problem scanning it, try changing the density of the QR code (with the Decrease Density/Increase Density button at the bottom).
5.  Blue Wallet immediately creates a new watch only wallet for you, with the descriptor you imported by scanning. If the transactions don’t appear within a few minutes, close and reopen the app and you should see them.
6.  The name of the wallet will be Imported Watch-only, and it’s okay to leave it like that.

Do you see transactions in this watch only wallet? You should have the exact same transactions that you see in the Alice wallet in Sparrow, just like with the previous exercise.

# Exercise 24: Set up password protection on Blue Wallet

Blue Wallet offers a password feature similar to Sparrow. However, it’s not exactly the same because in Sparrow, you’re putting the password on one wallet file. In Blue Wallet, though, you’re putting the password on the whole application. Having a password on Blue Wallet gives you an extra layer of security.

Note that the password on Blue Wallet is not like a passphrase. It does not change the private key, and you can still restore the wallet using just the seed phrase, in case you lose or forget your Blue Wallet password.

Follow these steps to set a password on Blue Wallet:

1.  Open Blue Wallet and make sure you’re in the home screen, where all the available wallets are shown.
2.  **Click the three dots** in the top right corner, and choose Security.
3.  Enable the option for **Encrypted and Password Protected**.
4.  Blue Wallet will give you a confirmation screen (about only protecting the data on your phone, and not actually the seed phrase). Click **I Understand**.
5.  Next, enter a secure password, then re-enter it, and click **OK**. Your Blue Wallet data on your phone is now encrypted and password protected. Be sure to keep the password safe. (But remember, you can still restore the wallet with the backed up seed phrase).

Learn more

What are you actually protecting in this step? You’re protecting the data linked with Blue Wallet on your phone. So if your phone were lost or stolen, anyone who has the phone wouldn’t be able to access your Blue Wallet data (depending on how secure your password is).

But it _only_ provides protection for the Blue Wallet data on your phone. What it is _not_ doing is providing any sort of protection for your seed phrase, outside of the phone.

For instance, assume you back up your seed phrase in a secure location, as you should. However, someone with bad intentions still finds that seed phrase. In that situation, the fact that you have a password on Blue Wallet doesn’t help you. Anyone with the backup seed phrase could just restore it to another wallet software, and steal your funds.

# Exercise 25: Recover the Bob wallet in Blue Wallet

In this exercise you’ll practice an emergency recovery, recreating the Bob wallet (created in Sparrow) onto the Blue Wallet app on your phone. In any bitcoin wallet software you use, you should always practice an emergency recovery. That way, if the emergency does occur, you’ll be prepared.

Note that this does _not_ create a watch only wallet. Instead, because you’re using your seed phrase, it’s recreating the private key. That means that this wallet will have full signing and spending ability.

1.  Open up Blue Wallet. In the top right is a plus sign, to add a new wallet. **Click on the plus sign**.
2.  On the Add Wallet screen, under Type, make sure to stick with the default of Bitcoin (not Multisig Vault).
3.  Do _not_ click on Create, which is the default. (That creates a brand new wallet.) Instead, click on **Import**. This will give you the opportunity to enter the seed phrase.
4.  Enter the 12 seed phrase for the Bob wallet in the free form field. Make sure to enter them in the right order, with the correct spelling, and a space between each word. Click **Import**.
5.  The transactions will show up soon, if everything was entered correctly.  
    You may need to close and reopen Blue Wallet, to make the transactions appear.
6.  The default name for an imported wallet starts with “Imported”. Click on the three dots at the top right, and rename the wallet **Bob Recovery**.

Did you get a message “No wallets were found”? This usually means that you typed in the seed phrase incorrectly. Check the words very carefully, make sure the spelling is exact, and that there’s a space between each word.

**Checking the recovered wallet**: To double-check that the recovered wallet was set up correctly, do two things:

1.  **Review transactions**: You should be able to see the same transactions in the Bob Recovery wallet in Blue Wallet as you do in the original Bob wallet in Sparrow.
2.  **Review Addresses**: Assuming you see the transactions, everything should be good. But in general (and especially if the original wallet has no transactions) you want to review addresses between the original and a recovered wallet.  
    In the Bob wallet in Sparrow, click on the blue Addresses button to see the addresses. In the Bob Recovery wallet in Blue Wallet, click on the three dots at the top right. At the very bottom of the dropdown, there’s a **Show Addresses** option. Compare a few of them with the Sparrow addresses. They should be the same. (Blue Wallet makes it difficult to review the addresses that are already used, so just look at the unused ones.)

Learn more: the private key is portable between wallet applications.

As you know by now, you see identical transactions in Blue Wallet and Sparrow because you used either the public key (for a watch only wallet) or the seed phrase (to recover a wallet).

For the recovered wallet, you entered the seed phrase that was generated for the first Bob wallet. That seed phrase translates to the same private key, and that private key is linked to the same addresses (assuming the script type, etc., is set up correctly).

When Blue Wallet looks up the addresses in the blockchain, it finds the same transactions as Sparrow did, looking up those same addresses in the blockchain.

One of the beautiful things about bitcoin is that you don’t need any _specific_ software. As long as you hold your own private key (which is the whole point of self custody), nobody can prevent you from switching to a different bitcoin software wallet. For instance, if you didn’t like Sparrow, you might decide to work with Blue Wallet.

Compare this to traditional banking. Switching banks requires a lengthy process—transferring funds, closing your old account, submitting ID documents to open a new one, and waiting for approvals. You need permission from financial institutions and government agencies at every step.

Or, consider people living in countries where it’s difficult or impossible to get a bank account. They are often forced to use actual paper currency, which is always losing value, sometimes rapidly. So, they’re completely unable to save money for their future.

Bitcoin can be a lifeline in these situations, if you know how to use it. Nobody can prevent you from saving, sending, or receiving bitcoin.

# Exercise 26: Send all bitcoin from the Bob Recovery wallet in Blue Wallet to Alice in Sparrow

Once you’ve created your recovery wallet, what’s the next step?

Your next step would be to test it, to make sure you can actually spend from it. After all, that’s the moment of truth—if everything was done correctly, you can send bitcoin from your recovery wallet.

So in this exercise, you will send bitcoin from the Bob Recovery wallet (in Blue Wallet) to the Alice wallet, in Sparrow.

You’ll send _all_ the bitcoin in this step, because we’re nearing the end of the book, and you don’t necessarily want to have bitcoin scattered across different wallets.

1.  Open Sparrow. Open the Alice wallet, and click the blue **Receive** button on the left, to bring up a receive address. You’ll be using the QR code, to transfer the receive address to Blue Wallet.
2.  In Blue Wallet, open the Bob Recovery wallet. At the bottom of the screen, click **Send**. On the Send screen, click **Scan** to the right of the address, to bring up the camera.
3.  Use Blue Wallet on your phone to scan the receive address in Sparrow. It should populate the address field, to the left of the Scan button.
4.  In Blue Wallet on your phone, instead of entering the amount of sats to send, click on the three dots at the top right corner. Then click on the option **Use Full Balance**. Blue Wallet will ask you to confirm.
5.  The default fee in Blue Wallet is set to get your transaction into the next block. You can click on it, to adjust the fee. I lowered mine to 2 sats/vB, because fees were low in general, and I thought it would still go through quickly enough.
6.  Enter in the Note to Self field: “**send to Alice in Sparrow**”, and click **Next.** On the next screen, click **Send now**.

After you hit Send now, you’ll see that in Blue Wallet, in the main screen, you have a pending transaction. It shows with the amount you sent, plus the fee, and starts out as Pending, because it hasn’t yet been confirmed.

Whenever the transaction gets confirmed, you’ll see the “Pending” disappear in Blue Wallet. Also, it will now show up with a confirmation in the Alice wallet in Sparrow.

Learn more: recovery after a potential seed phrase theft

What would you need to do in a real emergency recovery? For instance, in a situation where your laptop has been stolen, and you had Sparrow set up on that laptop, with a “hot” software wallet on it?

If the thief understood bitcoin, and knew you had Sparrow installed with a software wallet, you might be out of luck. The thief would probably have instantly sent all the bitcoin from your wallet to a different wallet, one that he controls.

In case the thief didn’t know these details, you may have more time. However, you still need to move your bitcoin. You need to send the entire amount from your old wallet, with the old seed phrase, to a new wallet with a new seed phrase. Moving all the funds from one bitcoin wallet to another is called “sweeping”.

Note that if you do this, you will lose all the labels for your transactions and addresses, because they’re saved in the Sparrow wallet file, not on the blockchain. This can be a serious issue, because knowing where your sats came from (through the labels) can be important for privacy. If you’d like to learn more, read up on the topic of “coin control in bitcoin”.

# Exercise 27: Bonus—use Blockstream wallet

In these exercises, the bitcoin wallet software we’ve been using has been mostly Sparrow. You also did a few exercises with Blue Wallet.

You used multiple wallets because by doing tasks like recovering seed phrases, setting up watch only wallets, and sending bitcoin _across_ different wallets, you end up with a better understanding of the fundamentals of bitcoin.

When you do this, you learn about seed phrases and what they truly represent, the blockchain and transaction fees, and privacy and security for your bitcoin—all at a deeper level.

In this bonus exercise, you’ll install another bitcoin wallet application—Blockstream. Like Sparrow and Blue Wallet, it’s also open source. Here, instead of splitting out all the different tasks into different exercises, I’ll give you a list of the tasks, and you’ll figure out how to do it. You have done similar tasks in Sparrow and Blue Wallet, so you’ve got a good background.

In this exercise, you’ll set up your final separate wallet, with a new seed phrase. This wallet represents another bitcoin user, Dan.

*   Install Blockstream from the Blockstream site: [https://blockstream.com/app](https://blockstream.com/green/). There are versions both for desktop and mobile.
*   Create a new wallet with Blockstream. Instead of the term _seed phrase_, Blockstream uses _recovery phrase_. A 6-digit PIN is required. Create the wallet Dan, a standard single sig wallet, and use the defaults.
*   To get some sats into Dan, do a send from the Carol wallet on Blue Wallet, to Dan on Blockstream. You can completely empty the Carol wallet with this send. That way, you don’t need to worry about having leftover sats in Carol.
*   Use your Alice seed phrase to recover your Alice wallet in Blockstream. The default settings should be correct, and you should see all your transactions if you recovered the seed phrase correctly.
*   As your last step with Dan—send _all_ the bitcoin in Dan (on Blockstream), to Alice. You can get the receive address for Alice either via the recovered wallet in Blockstream, or directly from the Alice wallet, in Sparrow.

So now you’ve had extensive experience in three bitcoin wallet applications—Sparrow, Blue Wallet, and Blockstream. Sparrow can be fairly straightforward, and gives you access to many tools and options. Blue Wallet is very simple, with limited options, but its simplicity makes it easy to use. And Blockstream is somewhere in between the two.

This hands-on experience with multiple different bitcoin wallets gives you a more comprehensive understanding of bitcoin, and also the flexibility to adapt to different tools. You’ve become a much more informed user.

# Exercise 28: Clearing practice wallets and creating a long-term wallet

If you’ve followed all the steps in the exercises, all wallets should be cleared out and empty, _except_ for the Alice wallet. That’s the only one that should contain bitcoin.

If this isn’t the case, go ahead now and do that. You don’t want to have bitcoin sitting around in multiple wallets, unless you have a specific purpose in mind. If you always want a place to experiment and practice with bitcoin transactions, you could leave a small amount of bitcoin in the Alice wallet. Otherwise, you can transfer it to a new wallet.

You’ll probably want to create a “real” wallet now, a long-term one, and one that may potentially hold a substantial amount of bitcoin. Go ahead and do that, using what you’ve learned. Below are some best practices to consider.

Keeping your seed phrase safe

The guidelines that you follow when working with this new wallet will be different—you’ll need to think more about privacy and security.

The wallet you’ll be creating—unlike the ones you just used in the exercises—is _not_ a short-term wallet for learning purposes. So, treat the seed phrase more carefully. Here are some of the ways to keep your seed phrase secure and private:

*   Never tell anyone your seed phrase. Anyone who asks for it is a scammer.
*   Never take a photo of your seed phrase. Don’t create or use a seed phrase anywhere with any cameras (webcams, security cameras, doorbell cameras, etc.).
*   Never type your seed phrase online. There are numerous websites that will ask you to type in your seed phrase to “check” it. These are run by scammers, they will immediately steal your bitcoin.
*   Never send your seed phrase via text or email.
*   Never speak your seed phrase out loud, especially where there are listening devices (like Alexa devices, phones, etc)
*   Keep a backup of your seed phrase in a safe place. Consider having multiple backups in different locations. Also think longer term—what if a flood or fire damages your home? Some people write their seed phrase on metal plates.
*   Don’t talk about how much bitcoin you own. That information is best kept private.
*   Understand that making your bitcoin security _too_ complex can also be a problem. Apparently a large amount of bitcoin has been lost through over-complicated security schemes.

Final notes and next steps

Completing the exercises in this book is a major milestone. You have a rock-solid understanding of the mechanics of bitcoin private keys and transactions. You’ve practiced with them in many different ways. This familiarity is important. It lessens the fear that most people have, of making some kind of mistake and losing bitcoin.

The confidence that develops through following the exercises and gradually understanding the concepts—that confidence is critical. The most important thing it allows you to do is _take action,_ and avoid the “analysis paralysis” caused by fear.

So, congratulations! And let’s talk about some of the next topics you’ll be interested in learning more about.

Security and privacy

At the beginning, when you were working with small, temporary wallets, you didn’t need to worry very much about security. The amounts were small, and the wallet was temporary.

Now you need to think about security differently. The realization should have become crystal clear—your seed phrase, and the private key it represents, is the key to your bitcoin. So if anyone with bad intentions were to find it, they could very easily steal your bitcoin. They would do this in the exact same way that you moved bitcoin around, in the exercises.

Also, the Alice and Bob wallet have been opened in multiple different tools—Sparrow, Blue Wallet, Blockstream. As practice exercises, it’s good to work with multiple wallets, to develop skills and a better understanding of transactions.

But for a wallet that contains larger amounts of bitcoin, and that will be a long-term holding wallet, you want to expose it as little as possible. It’s like telling a secret to three trustworthy friends. Sure, they’re trustworthy, but it would be far more private and secure to not tell the secret to anyone.

Privacy and security go together like hand and glove. If you’re private about your bitcoin holdings, then your security is far, far better. Most of the physical attacks related to bitcoin have been on people who have somehow been in the public eye because of bitcoin.

Talk about bitcoin, if you want. But never tell people how much you own, and don’t post anything online or on social media about how much you own.

Privacy is very important. For instance, in Sweden there are laws that put all tax records in the public domain, including names and addresses. Criminals have searched those records, and then linked them to social media mentions of bitcoin. Those searches provided the criminals with good targets, and there have been multiple attacks on bitcoiners in Sweden. ([https://cointelegraph.com/news/swedish-bitcoiners-targeted-by-armed-criminals](https://cointelegraph.com/news/swedish-bitcoiners-targeted-by-armed-criminals), retrieved 2/6/2025)

Remember: good security habits are built over time. Don’t rush into complex setups before mastering the basics. Your security approach should evolve over time, just like your knowledge and assets in bitcoin.

Threat model

Of course, when you self custody your own bitcoin, you are immune to _the_ most common threat to your bitcoin, which is when the exchange that you hold your bitcoin on is hacked, or if the exchange itself has stolen the funds. Another major threat if you don’t self custody is that the government can force the exchange to hand over all the bitcoin that it holds—bitcoin that you thought was yours.

But assuming your bitcoin is in self custody, you want to consider the concept of “threat model”. For instance—in your particular situation, what is the most likely threat to your bitcoin stash? Then, based on that, you make decisions about how to best protect it.

Let’s consider some of the most commonly recognized threats:

*   Losing your seed phrase
*   Fire, flood, or other disaster destroying your seed phrase backup
*   Robbery and physical coercion, to reveal your seed phrase
*   Malware on your computer that captures your keystrokes, and watches for anything like a seed phrase
*   A scammer convinced you to reveal your seed phrase
*   User error, making a mistake because your security setup is too complex. For instance, adding a passphrase to the seed phrase, and forgetting the passphrase
*   You die, and your heirs don’t know how to access your bitcoin

These are situations you need to consider, and guard against.

Or let’s say you’re a refugee, escaping a war. You have managed to scrape together some bitcoin, and need to cross multiple borders with it. What’s your main concern, in this situation? It’s to make sure that you don’t have anything on you to indicate you might own bitcoin. No hardware wallets, no software wallets on your phone, no suspicious looking lists of 12 words as you pass through various immigration checkpoints. In this case, you’d want to carefully memorize your seed phrase, and then set up your wallet again when you’re settled in a safe place.

If you live in an area where forest fires are common? In that situation, you definitely need to have a backup of your seed phrase in a different location, or maybe a multisig setup.

If you have a lot of bitcoin to secure

You might be in a situation where need to secure a substantial amount of bitcoin. In that case, there’s a whole separate set of strategies to consider.

The maker of Sparrow Wallet, Craig Raw, has some suggestions about what kind of security and privacy considerations you need to take, as you put more of your assets into bitcoin. See what he has to say here: [https://sparrowwallet.com/docs/best-practices.html](https://sparrowwallet.com/docs/best-practices.html).

Here’s some additional strategies to consider:

**Multiple backups**: If you have just one backup of your seed phrase, you’re vulnerable to losing access to your bitcoin. Especially if you have larger amounts to worry about, you will want to consider having another copy of your seed phrase, perhaps given in encrypted format to a close friend or family. The danger, of course, is that there’s another copy of your seed phrase out there.

**Multisig wallets**: These are usually done as a 2 of 3 setup, in which there are 3 seed phrases, and 2 of them are needed to sign a transaction and spend bitcoin. The seed phrases are usually stored in different physical locations, so it would be much more difficult for thieves to get access to 2 of them. The tradeoff is that they’re more complex to set up and maintain.

**Bitcoin Timelocks**: Timelocks are a bitcoin security feature that restrict spending until a certain condition is met, such as when a specific time has passed. This is a mostly unexplored area, but I predict that it’ll start becoming much more popular as more bitcoin wallet software starts supporting it.

**Have a “cold storage” vault**: If you have substantial assets in bitcoin, consider having separate wallets for different purposes. The “cold storage vault” gets the most security, of course.

*   Cold storage vault: You have the majority of your assets here. It’s rarely accessed except to receive bitcoin, and it’s accessed via a watch only wallet except in case of emergency. This would be like a safe, with gold bars in it, kept very secure.
*   Spending account: This is where most transactions occur. This is more like a checking account, or a debit card, or cash in your wallet. Security isn’t as much of a concern. You may also choose to do smaller transactions in the Lightning network (see the section on Lightning in the [Resources](#Resources) chapter).

**Run your own bitcoin node**: If you have substantial assets in bitcoin to protect, you should consider connecting to a private bitcoin node that you control. When connecting to public bitcoin nodes, which is the default in Sparrow, there’s the potential that you’re exposing private information—not the seed phrase, but information about what IP address is linked to a particular bitcoin address. And often an IP address can be linked to a street address.

Another option if you can’t run a bitcoin node is to run a Tor proxy in Sparrow, which also gives better privacy. You can find more info on this topic online.

Hardware wallets

**What is a hardware wallet?** A hardware wallet is a small, specialized device that has one purpose only—to store the private keys needed to access your bitcoin. When you want to send bitcoin, you need to get the hardware wallet, and usually unlock it with a PIN. Then your hardware wallet transmits the digital signature to the computer where the bitcoin transaction is being managed. The transaction can be set up with Sparrow, but usually the hardware wallet will have its own software. The signature is usually sent via a USB cable, or sometimes with QR codes.

**Do you need to buy a hardware wallet immediately?** Hardware wallet manufacturers would like you to buy one, of course. And these manufacturers are very influential, and advertise heavily in bitcoin podcasts and videos.

But my answer would be no, you don’t need to. Not until your stash of bitcoin is more substantial, or unless you have special requirements. It’s okay to begin with a hot wallet on Sparrow or Blue Wallet, assuming the laptop or phone is properly secured.

Think of it this way—you need to consider the security and privacy of your bitcoin in a step-by-step approach. You wouldn’t purchase an expensive safe if you only have a small piece of silver to secure, right? You would purchase that safe only if you have a gold bar that you want to secure—something much more valuable. The same principle applies with holding a smaller amount of bitcoin.

**There’s some negatives to hardware wallets as well.** Hardware wallets can offer some protection for bitcoin storage when everything works well, but they aren’t the perfect solution. Yes, they can protect private keys from malware. At the same time, they also introduce their own risks, like closed-source software, and mandatory firmware updates.

And hardware wallets remain completely out of reach for many people in poorer countries, because of cost, availability, and import barriers. It’s almost impossible to find any hardware wallet for less than about $75.

But maybe the most important factor is that once you’ve purchased a hardware wallet, you’re advertising to the world that you probably own bitcoin. And there have been _major_ data leaks. In 2020, the largest hardware wallet company, Ledger, was hacked and the entire customer database, including name, address, and order details, was published. These types of issues happen over and over, and make people very nervous.

The standard advice is to not have hardware wallets shipped to your home address, only to a post office box. But that option introduces extra expense, complications, and delay.

**Recommendations:** So, I don’t necessarily recommend hardware wallets to beginners, when they first start their bitcoin journey. Until you accumulate an amount of bitcoin that would cause serious pain if you lost it, consider this setup:

*   A hot wallet in Sparrow, with a password on the wallet file. Or a hot wallet on a phone, also with a password.
*   Make sure your computer or phone is well secured.
*   Back up your seed phrase well, potentially in multiple locations

Then as you learn more about bitcoin and security and accumulate more, you may decide that you should get a hardware wallet, and store your seed phrase on the hardware wallet.

Make sure the one you buy is bitcoin only, and doesn’t use proprietary software (in other words, it should be open source). Below are some of the most well-known options.

| SeedSigner | https://seedsigner.com/ |
| --- | --- |
| Coldcard | https://coldcard.com/ |
| Foundation Passport | https://foundation.xyz |
| Blockstream Jade | https://blockstream.com |

The SeedSigner is a hardware wallet that you can put together yourself, with a Raspberry PI and a few other components. You can also purchase a fully assembled one on the SeedSigner website.

Some people have also gone the DIY approach, by using TailsOS on a USB stick, or similar options. Here’s a post that has more information on that method: [https://stacker.news/items/569901](https://stacker.news/items/569901). Make sure you do some research before you choose this option.

I suggest that you continue to use Sparrow to manage and coordinate transactions—it’s more secure than the software provided by the hardware wallet vendor. Also, you now have a very good understanding of Sparrow, after going through these exercises.

Keep on learning

As you’ve learned throughout this book, the basics of Bitcoin are straightforward. There are many details that can make the process of dealing with wallets, and sending and receiving bitcoin challenging. But think of this: you now know more about the practical use of bitcoin than the vast majority of the world’s population. The skills you’ve developed, in working with this revolutionary monetary technology, are ones that most people haven’t begun to grasp. These skills allow you to take control of your financial future as a sovereign individual.

There’s a popular phrase in Bitcoin, about “_going down the rabbit hole_”. Most bitcoiners have, at one point or another, become obsessive about learning as much as possible about Bitcoin (the [Resources](#Resources) section in this book is a good place to start). They spend hundreds of hours, reading books and articles, listening to podcasts and videos, and talking to other bitcoiners both in person and online. And one topic leads to another—it’s really an endlessly fascinating journey.

This is just the beginning of your journey. As you grow more comfortable with Bitcoin’s concepts and tools, you’ll discover new ideas and tools. Start small, experiment often, and build on each success. Many people began learning about Bitcoin with only NGU in mind (a bitcoin term “_Number Go Up_”, in other words, just a raw desire to make money). Then later, they find themselves going deeper and deeper into Bitcoin’s fascinating economic and technical layers.

Take your time, stay curious, and keep learning—the rabbit hole goes as deep as you dare to explore. I’ll leave you with a favorite saying of bitcoiners everywhere:

Fix the money, fix the world.

This is Bitcoin’s promise: an alternative to broken money and theft via inflation. By reclaiming control of your wealth through self-custody, you’re not just protecting your future—you’re opting out of a broken system. Bitcoin restores money as a tool of freedom, not force.

The revolution starts in your wallet.

What did you think of Bitcoin Hands-On?

First of all, thank you for purchasing this book. I hope you're feeling more comfortable with actually using Bitcoin. I would truly appreciate if you could post a review on Amazon. As an independent author with a marketing budget of zero, your review helps me tremendously.

To write a review, you can go to the Amazon website, click on Orders in the top right, and find your order of Bitcoin Hands-On. Click on your order to find a link to write a product review.

I learn so much from your feedback and comments, and continue to improve this book. Please email me at:

[**feedback@BitcoinHandsOn.com**](feedback@BitcoinHandsOn.com)

Resources

Books, articles, and videos

**The Bullish Case for Bitcoin by Vijay Boyapati**

Many people have been introduced to the “why” of bitcoin through one article published on Medium: [The Bullish Case for Bitcoin](https://vijayboyapati.medium.com/the-bullish-case-for-bitcoin-6ecc8bdecc1). It’s an inspiring introduction to Bitcoin, including a review of money throughout history. Boyapati writes a primer on the value of Bitcoin, and why it’s superior to government currency, and even gold. He’s also expanded the article into an entire book, which is also a good read.

**The Bitcoin Standard by Saifedean Ammous**

This classic book is the one that everyone even remotely interested in Bitcoin should read. Ammous goes into great depth on what makes a good money, and why. He writes about the best monies throughout history, and how when one type of money replaces another, those who hold on to the old form of money are impoverished.

**Bitcoin University YouTube channel**

One of the YouTube channels that I recommend for learning about Bitcoin is Bitcoin University ([https://www.youtube.com/@Bitcoin\_University](https://www.youtube.com/@Bitcoin_University)). The creator, Matthew Kratter has solid information on self custody as well as many other aspects of Bitcoin.  
A reminder—with YouTube channels, the comments section will often have scammers, so be cautious.

The Lightning Network

Bitcoin’s blockchain is secure and reliable, but it can be inconvenient and expensive for small transactions. This is especially a problem when the transaction fees are high. To solve this, developers have created what’s called “Layer-2” solutions. These work on top of the Bitcoin network, to make transactions faster and cheaper.

The most popular layer 2 is the Lightning Network. The Lightning Network lets users open payment channels, to send bitcoin instantly with very low fees. Instead of recording every transaction on the blockchain, lightning handles them off-chain, and only settles the final result on the bitcoin blockchain. This makes it perfect for small transactions.

If you’re using lightning regularly, be aware that it evolves quickly, and wallet apps sometimes disappear. In the United States, some of the most popular lightning wallets have been removed from app stores because of financial regulations. So, it’s important to stay informed, and avoid keeping large amounts in your lightning wallet.

Lightning wallet apps fall into two categories—custodial and non-custodial.

**Custodial Lightning**

The custodial ones take custody of your bitcoin on the app, and don’t allow you to manage it directly. But they also don’t require you to know the details of payment channels and nodes, which can be very challenging. These types of app charge a small fee for sending transactions. Also, since it’s not self custody, it’s best to avoid storing larger amounts on them.

Some of the more popular ones are:

*   CoinOS ([https://coinos.io/](https://coinos.io/))
*   Aqua ([https://aquawallet.io/](https://aquawallet.io/))
*   Wallet of Satoshi ([https://www.walletofsatoshi.com/](https://www.walletofsatoshi.com/), not available in the US).

If you purchased your bitcoin with the Strike app, you already have a lightning wallet built into it. However, it’s KYC, and thus tied to your identity.

**Non-custodial Lightning**

The non-custodial apps do not take charge of your bitcoin, instead you work with your own bitcoin on the app. They require you to understand and manage your own lightning channels and nodes. You still pay a fee, but it’s lower and you have much more control over fees. Lightning is a fascinating area to learn about, but self custody with lightning is challenging for beginners. So, I’d recommend lots of research before setting up a lightning channel. Some of the more popular non-custodial apps are

*   Zeus ([https://zeusln.com/](https://zeusln.com/))
*   Breez ([https://breez.technology/](https://breez.technology/))
*   Phoenix ([https://phoenix.acinq.co/](https://phoenix.acinq.co/))

Support

If you need more support for any of the tools you’ve worked with, a good place to go is the sites recommended on the official website. Often these are hosted on Telegram.

For instance, if you need help with Sparrow, go to the official Sparrow website ([https://sparrowwallet.com/](https://sparrowwallet.com/)), and look for the Telegram link, right above the Download button. The hardware wallet SeedSigner also has a link to their Telegram group on the FAQ page.

One thing to note about any public bitcoin group, especially in Telegram, is that they are _very_ heavily targeted by scammers. If you ever post on one of these, you’ll immediately get multiple people sending you private messages. They’re all from scammers, so never respond to any private messages. Everything that’s legitimate is in public chat on these groups. And of course, never give anyone your seed phrase.

Never search for bitcoin related telegram groups by searching directly in Telegram. There are many groups out there that have official sounding names, but are actually run by scammers.

For instance, there’s a Telegram group called Sparrow Technical Support, run by scammers. If you post there, the administrators will try to get you to reveal your seed phrase. When looking for a support group on Telegram, only go to the Telegram group link from the official website.
