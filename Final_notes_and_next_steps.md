---
layout: default
title: Final notes and next steps
---
# Final notes and next steps

Completing the exercises in this book is a major milestone. You have a rock-solid understanding of the mechanics of bitcoin private keys and transactions. You’ve practiced with them in many different ways. This familiarity is important. It lessens the fear that most people have, of making some kind of mistake and losing bitcoin.

The confidence that develops through following the exercises and gradually understanding the concepts—that confidence is critical. The most important thing it allows you to do is _take action,_ and avoid the “analysis paralysis” caused by fear.

So, congratulations! And let’s talk about some of the next topics you’ll be interested in learning more about.

### Security and privacy

At the beginning, when you were working with small, temporary wallets, you didn’t need to worry very much about security. The amounts were small, and the wallet was temporary.

Now you need to think about security differently. The realization should have become crystal clear—your seed phrase, and the private key it represents, is the key to your bitcoin. So if anyone with bad intentions were to find it, they could very easily steal your bitcoin. They would do this in the exact same way that you moved bitcoin around, in the exercises.

Also, the Alice and Bob wallet have been opened in multiple different tools—Sparrow, Blue Wallet, Blockstream. As practice exercises, it’s good to work with multiple wallets, to develop skills and a better understanding of transactions.

But for a wallet that contains larger amounts of bitcoin, and that will be a long-term holding wallet, you want to expose it as little as possible. It’s like telling a secret to three trustworthy friends. Sure, they’re trustworthy, but it would be far more private and secure to not tell the secret to anyone.

Privacy and security go together like hand and glove. If you’re private about your bitcoin holdings, then your security is far, far better. Most of the physical attacks related to bitcoin have been on people who have somehow been in the public eye because of bitcoin.

Talk about bitcoin, if you want. But never tell people how much you own, and don’t post anything online or on social media about how much you own.

Privacy is very important. For instance, in Sweden there are laws that put all tax records in the public domain, including names and addresses. Criminals have searched those records, and then linked them to social media mentions of bitcoin. Those searches provided the criminals with good targets, and there have been multiple attacks on bitcoiners in Sweden. ([https://cointelegraph.com/news/swedish-bitcoiners-targeted-by-armed-criminals](https://cointelegraph.com/news/swedish-bitcoiners-targeted-by-armed-criminals), retrieved 2/6/2025)

Remember: good security habits are built over time. Don’t rush into complex setups before mastering the basics. Your security approach should evolve over time, just like your knowledge and assets in bitcoin.

### Threat model

Of course, when you self custody your own bitcoin, you are immune to _the_ most common threat to your bitcoin, which is when the exchange that you hold your bitcoin on is hacked, or if the exchange itself has stolen the funds. Another major threat if you don’t self custody is that the government can force the exchange to hand over all the bitcoin that it holds—bitcoin that you thought was yours.

But assuming your bitcoin is in self custody, you want to consider the concept of “threat model”. For instance—in your particular situation, what is the most likely threat to your bitcoin stash? Then, based on that, you make decisions about how to best protect it.

Let’s consider some of the most commonly recognized threats:

·       Losing your seed phrase

·       Fire, flood, or other disaster destroying your seed phrase backup

·       Robbery and physical coercion, to reveal your seed phrase

·       Malware on your computer that captures your keystrokes, and watches for anything like a seed phrase

·       A scammer convinced you to reveal your seed phrase

·       User error, making a mistake because your security setup is too complex. For instance, adding a passphrase to the seed phrase, and forgetting the passphrase

·       You die, and your heirs don’t know how to access your bitcoin

These are situations you need to consider, and guard against.

Or let’s say you’re a refugee, escaping a war. You have managed to scrape together some bitcoin, and need to cross multiple borders with it. What’s your main concern, in this situation? It’s to make sure that you don’t have anything on you to indicate you might own bitcoin. No hardware wallets, no software wallets on your phone, no suspicious looking lists of 12 words as you pass through various immigration checkpoints. In this case, you’d want to carefully memorize your seed phrase, and then set up your wallet again when you’re settled in a safe place.

If you live in an area where forest fires are common? In that situation, you definitely need to have a backup of your seed phrase in a different location, or maybe a multisig setup.

### If you have a lot of bitcoin to secure

You might be in a situation where need to secure a substantial amount of bitcoin. In that case, there’s a whole separate set of strategies to consider.

The maker of Sparrow Wallet, Craig Raw, has some suggestions about what kind of security and privacy considerations you need to take, as you put more of your assets into bitcoin. See what he has to say here: [https://sparrowwallet.com/docs/best-practices.html](https://sparrowwallet.com/docs/best-practices.html).

Here’s some additional strategies to consider:

**Multiple backups**: If you have just one backup of your seed phrase, you’re vulnerable to losing access to your bitcoin. Especially if you have larger amounts to worry about, you will want to consider having another copy of your seed phrase, perhaps given in encrypted format to a close friend or family. The danger, of course, is that there’s another copy of your seed phrase out there.

**Multisig wallets**: These are usually done as a 2 of 3 setup, in which there are 3 seed phrases, and 2 of them are needed to sign a transaction and spend bitcoin. The seed phrases are usually stored in different physical locations, so it would be much more difficult for thieves to get access to 2 of them. The tradeoff is that they’re more complex to set up and maintain.

**Bitcoin Timelocks**: Timelocks are a bitcoin security feature that restrict spending until a certain condition is met, such as when a specific time has passed. This is a mostly unexplored area, but I predict that it’ll start becoming much more popular as more bitcoin wallet software starts supporting it.

**Have a “cold storage” vault**: If you have substantial assets in bitcoin, consider having separate wallets for different purposes. The “cold storage vault” gets the most security, of course.

·       Cold storage vault: You have the majority of your assets here. It’s rarely accessed except to receive bitcoin, and it’s accessed via a watch only wallet except in case of emergency. This would be like a safe, with gold bars in it, kept very secure.

·       Spending account: This is where most transactions occur. This is more like a checking account, or a debit card, or cash in your wallet. Security isn’t as much of a concern. You may also choose to do smaller transactions in the Lightning network (see the section on Lightning in the [Resources](file:///C:/Sylvia/_PracticalBitcoinBook/TEST%20GITHUB%20BitcoinHandsOn.docx#Resources) chapter).

**Run your own bitcoin node**: If you have substantial assets in bitcoin to protect, you should consider connecting to a private bitcoin node that you control. When connecting to public bitcoin nodes, which is the default in Sparrow, there’s the potential that you’re exposing private information—not the seed phrase, but information about what IP address is linked to a particular bitcoin address. And often an IP address can be linked to a street address.

Another option if you can’t run a bitcoin node is to run a Tor proxy in Sparrow, which also gives better privacy. You can find more info on this topic online.

### Hardware wallets

**What is a hardware wallet?** A hardware wallet is a small, specialized device that has one purpose only—to store the private keys needed to access your bitcoin. When you want to send bitcoin, you need to get the hardware wallet, and usually unlock it with a PIN. Then your hardware wallet transmits the digital signature to the computer where the bitcoin transaction is being managed. The transaction can be set up with Sparrow, but usually the hardware wallet will have its own software. The signature is usually sent via a USB cable, or sometimes with QR codes.

**Do you need to buy a hardware wallet immediately?** Hardware wallet manufacturers would like you to buy one, of course. And these manufacturers are very influential, and advertise heavily in bitcoin podcasts and videos.

But my answer would be no, you don’t need to. Not until your stash of bitcoin is more substantial, or unless you have special requirements. It’s okay to begin with a hot wallet on Sparrow or Blue Wallet, assuming the laptop or phone is properly secured.

Think of it this way—you need to consider the security and privacy of your bitcoin in a step-by-step approach. You wouldn’t purchase an expensive safe if you only have a small piece of silver to secure, right? You would purchase that safe only if you have a gold bar that you want to secure—something much more valuable. The same principle applies with holding a smaller amount of bitcoin.

**There’s some negatives to hardware wallets as well.** Hardware wallets can offer some protection for bitcoin storage when everything works well, but they aren’t the perfect solution. Yes, they can protect private keys from malware. At the same time, they also introduce their own risks, like closed-source software, and mandatory firmware updates.

And hardware wallets remain completely out of reach for many people in poorer countries, because of cost, availability, and import barriers. It’s almost impossible to find any hardware wallet for less than about $75.

But maybe the most important factor is that once you’ve purchased a hardware wallet, you’re advertising to the world that you probably own bitcoin. And there have been _major_ data leaks. In 2020, the largest hardware wallet company, Ledger, was hacked and the entire customer database, including name, address, and order details, was published. These types of issues happen over and over, and make people very nervous.

The standard advice is to not have hardware wallets shipped to your home address, only to a post office box. But that option introduces extra expense, complications, and delay.

**Recommendations:** So, I don’t necessarily recommend hardware wallets to beginners, when they first start their bitcoin journey. Until you accumulate an amount of bitcoin that would cause serious pain if you lost it, consider this setup:

·       A hot wallet in Sparrow, with a password on the wallet file. Or a hot wallet on a phone, also with a password.

·       Make sure your computer or phone is well secured.

·       Back up your seed phrase well, potentially in multiple locations

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

### Keep on learning

As you’ve learned throughout this book, the basics of Bitcoin are straightforward. There are many details that can make the process of dealing with wallets, and sending and receiving bitcoin challenging. But think of this: you now know more about the practical use of bitcoin than the vast majority of the world’s population. The skills you’ve developed, in working with this revolutionary monetary technology, are ones that most people haven’t begun to grasp. These skills allow you to take control of your financial future as a sovereign individual.

There’s a popular phrase in Bitcoin, about “_going down the rabbit hole_”. Most bitcoiners have, at one point or another, become obsessive about learning as much as possible about Bitcoin (the [Resources](file:///C:/Sylvia/_PracticalBitcoinBook/TEST%20GITHUB%20BitcoinHandsOn.docx#Resources) section in this book is a good place to start). They spend hundreds of hours, reading books and articles, listening to podcasts and videos, and talking to other bitcoiners both in person and online. And one topic leads to another—it’s really an endlessly fascinating journey.

This is just the beginning of your journey. As you grow more comfortable with Bitcoin’s concepts and tools, you’ll discover new ideas and tools. Start small, experiment often, and build on each success. Many people began learning about Bitcoin with only NGU in mind (a bitcoin term “_Number Go Up_”, in other words, just a raw desire to make money). Then later, they find themselves going deeper and deeper into Bitcoin’s fascinating economic and technical layers.

Take your time, stay curious, and keep learning—the rabbit hole goes as deep as you dare to explore. I’ll leave you with a favorite saying of bitcoiners everywhere:

Fix the money, fix the world.

This is Bitcoin’s promise: an alternative to broken money and theft via inflation. By reclaiming control of your wealth through self-custody, you’re not just protecting your future—you’re opting out of a broken system. Bitcoin restores money as a tool of freedom, not force.

The revolution starts in your wallet.

  

### What did you think of Bitcoin Hands-On?

First of all, thank you for purchasing this book. I hope you're feeling more comfortable with actually using Bitcoin. I would truly appreciate if you could post a review on Amazon. As an independent author with a marketing budget of zero, your review helps me tremendously.

To write a review, you can go to the Amazon website, click on Orders in the top right, and find your order of Bitcoin Hands-On. Click on your order to find a link to write a product review.

I learn so much from your feedback and comments, and continue to improve this book. Please email me at:

[feedback@BitcoinHandsOn.com](file:///C:/Sylvia/_PracticalBitcoinBook/feedback@BitcoinHandsOn.com)