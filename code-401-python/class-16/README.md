# Cryptography
the practice and study of techniques for secure communication in the presence of adversarial behavior. More generally, cryptography is about constructing and analyzing protocols that prevent third parties or the public from reading private messages.

Encryption, decryption, and cracking
One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.

The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.


## Decrypting a message

With Caeser Cipher it is the act of unshifting the letters by the certain amount of letter of the encrypting.

### Cracking the cipher

There are three main techniques he could use: frequency analysis, known plaintext, and brute force.

### Frequency analysis

Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.

### Known plaintext

Another term for the original unencrypted message is plaintext. If the enemy already knew some part of the plaintext, it will be easier for them to crack the rest of the encrypted version.



### Brute force

There are only 25 possible shifts (not 26 — why not?). The enemy could take some time to try out each of them and find one that yielded a sensible message. They wouldn't even need to try the shifts on the entire message, just the first word or two.

# Refrences
1. https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking
2. https://en.wikipedia.org/wiki/Caesar_cipher