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
