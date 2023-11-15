# h3 Hashes

# x) Read and summarize
## Schneier 2015: Applied Cryptography: Chapter 2 - Protocol Building Blocks: subchapters "2.3 One-way Fuctions" and "2.4 One-Way Hash Functions"

### Cryptography is to solve problems

### Protocols
A protocol is a series of steps, involving two or more parties, designed to
accomplish a task. Computers need formal protocols to do the same things that people do without thinking.

Protocols have characteristics like everyone involved in the protocol must know the protocol and all of the steps to follow in advance. A cryptographic protocol is a protocol that uses cryptography. It should not be possible to do more or learn more than what is specified in the protocol.

People on computer networks could be dishonest. An arbitrator is a disinterested third party trusted to complete a protocol. Because of the high cost of hiring arbitrators, arbitrated protocols can be subdivided into two lower-level subprotocols. A self-enforcing protocol is the best type of protocol. The protocol itself guarantees fairness.

### Attacks
Cryptographic attacks can be directed against the cryptographic algorithms used in protocols, against the cryptographic techniques used to implement the algorithms and protocols, or against the protocols themselves.
There could be active or passive attacks and active or passive cheaters.

A good cryptosystem is one in which all the security is inherent in knowledge of the key and none is inherent in knowledge of the algorithm.

### Symmetric
Symmetric cryptosystems problems:
Keys must be distributed in secret
One revealed key could be used to encrypt all related messages
Assuming a separate key is used for each pair of users in a network, the total number of keys increases rapidly as the number of users increases

### One-way
One-way function is central to public-key cryptography. One-way functions are relatively easy to compute, but significantly harder to reverse. Although there is not mathematic certainty that truly one-way function exists.

A trapdoor one-way function is a special type of one-way function. It is easy to compute in one direction and hard to compute in the other direction. When you know the secret, you can easily compute the function in the other direction.

### Hash
A one-way hash function has many names
- compression function
- contraction function
- message digest
- fingerprint
- cryptographic checksum
- message integrity check (MIC)
- manipulation detection code (MDC).

A hash function is a function that takes a variable-length input string (pre-image) and converts it to a fixedlength output string (hash value). The point here is to fingerprint the pre-image: to produce a value that indicates whether a candidate pre-image is likely to be the same as the real pre-image.

A good one-way hash function is also collision-free: It is hard to generate two pre-images with the same hash value. The hash function is public; there's no secrecy to the process. The security of a one-way hash function is its one-wayness.

# a) Billion dollar busywork

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3Keyboard1.JPG)

First I changed keyboard layout.

I followed instructions: https://terokarvinen.com/2023/trust-to-blockchain/#h3-hashes

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3a1.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3a2.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3a3.JPG)

One way to make md5 hash begin with zero: https://stackoverflow.com/questions/3180374/can-an-md5-hash-begin-with-a-zero

# b) Compare hash and Install hashcat and test that it works

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3b1.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3b2.JPG)

Small text file "test.txt". I changed one letter in file and hash changed to totally different.

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3b3.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3b4.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3b5.JPG)

https://terokarvinen.com/2022/cracking-passwords-with-hashcat/

# c) Crack this hash: 21232f297a57a5a743894a0e4a801fc3

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c1.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c2.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c3.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c4.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c5.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c6.JPG)

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/h3c7.JPG)




# d) Crack this Windows NTLM hash: f2477a144dff4f216ab81f2ac3e3207d

I tried to search info, but didnt manage to crack that hash
https://security.stackexchange.com/questions/161889/understanding-windows-local-password-hashes-ntlm

# e) Try cracking this hash and comment on your hash rate

I didnt succeeded
