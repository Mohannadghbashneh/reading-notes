# Cryptography

## Reading:
### What is Cryptography?
- Cryptography is the practice and study of techniques for secure communication in the presence of third parties called adversaries. More generally, cryptography is about constructing and analyzing protocols that prevent third parties or the public from reading private messages; various aspects in information security such as data confidentiality, data integrity, authentication, and non-repudiation are central to modern cryptography. Modern cryptography exists at the intersection of the disciplines of mathematics, computer science, electrical engineering, communication science, and physics. Applications of cryptography include ATM cards, computer passwords, and electronic commerce.

### Types of Cryptography
1. Hashing
2. Symmetric Cryptography
3. Asymmetric Cryptography
4. Key Exchange Algorithms

### Types of cryptographic functions
1. Authentication
2. Nonrepudiation
3. Confidentiality
4. Integrity

### Caesar cipher
In cryptography, a Caesar cipher, also known as Caesar's cipher, the shift cipher, Caesar's code or Caesar shift, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on. The method is named after Julius Caesar, who used it in his private correspondence

### Encryption, decryption, and cracking
- Encryption: scrambling the data according to a secret key (in this case, the alphabet shift).
- Decryption: unscrambling the data according to the same secret key. 
- Cracking: guessing the secret key by trying all possible keys until the correct one is found.

- Cryptography requires numbers that attackers can’t guess. We can’t just use the same numbers over and over. We want to generate these numbers in a very unpredictable way so attackers can’t guess them. These random numbers are essential for secure encryption, whether you’re encrypting your own files or just using an HTTPS website on the Internet.

### How computers generate random numbers
- To generate a “true” random number, the computer measures some type of physical phenomenon that takes place outside of the computer. For example, the computer could measure the radioactive decay of an atom. According to quantum theory, there’s no way to know for sure when radioactive decay will occur, so this is essentially “pure randomness” from the universe. An attacker wouldn’t be able to predict when radioactive decay would occur, so they wouldn’t know the random value.