# Hashes

# x) Read and summarize
## Schneier 2015: Applied Cryptography: Chapter 2 - Protocol Building Blocks: subchapters "2.3 One-way Fuctions" and "2.4 One-Way Hash Functions"

### Cryptography is to solve problems.

A protocol is a series of steps, involving two or more parties, designed to
accomplish a task. Computers need formal protocols to do the same things that people do without thinking.

Protocols have characteristics like everyone involved in the protocol must know the protocol and all of the steps to follow in advance. A cryptographic protocol is a protocol that uses cryptography. It should not be possible to do more or learn more than what is specified in the protocol.

People on computer networks could be dishonest. An arbitrator is a disinterested third party trusted to complete a protocol. Because of the high cost of hiring arbitrators, arbitrated protocols can be subdivided into two lower-level subprotocols. A self-enforcing protocol is the best type of protocol. The protocol itself guarantees fairness.

Cryptographic attacks can be directed against the cryptographic algorithms used in protocols, against the cryptographic techniques used to implement the algorithms and protocols, or against the protocols themselves.
There could be active or passive attacks and active or passive cheaters.

A good cryptosystem is one in which all the security is inherent in knowledge of the key and none is inherent in knowledge of the algorithm.

Symmetric cryptosystems problems:
Keys must be distributed in secret
One revealed key could be used to encrypt all related messages
Assuming a separate key is used for each pair of users in a network, the total number of keys increases rapidly as the number of users increases

One-way function is central to public-key cryptography. One-way functions are relatively easy to compute, but significantly harder to reverse. Although there is not mathematic certainty that truly one-way function exists.

A trapdoor one-way function is a special type of one-way function. It is easy to compute in one direction and hard to compute in the other direction. When you know the secret, you can easily compute the function in the other direction.

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
