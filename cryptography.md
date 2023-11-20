
##   Cryptography
- Cryptography is the science of secret, or hidden writing
- Crypto => Hidden/Secret | Graphy => Writing
- Used to secure your data/text.
- It has two main Components:
### a. Encryption
- i. Practice of hiding messages so that they can not be read by  anyone other than the intended recipient
### b. Authentication & Integrity
- i. Ensuring that users of data/resources are the persons 
## Encryption
### Cipher
- **Cipher is a method for encrypting message**
- Encryption algorithms are standardized & published
- The key which is an input to the algorithm is secret
- **``Key``: is a string of numbers or characters**
- **If same key is used for encryption & decryption the algorithm is called ``symmetric``**
- **If different keys are used for encryption & decryption the algorithm is called ``asymmetric``**
## Symmetric Algorithms
- Algorithms in which the key for encryption and decryption are the same are Symmetric
- Example: Caesar Cipher
● Types:
- **○ Block Ciphers**
- Encrypt data one block at a time (typically  64 bits, or 128 bits)
- Used for a single message  Stream Ciphers
-  Encrypt data one bit or one byte at a time
-  sed if data is a constant stream of information Substitution Ciphers
##  Caesar Cipher
- **Caesar Cipher is a method in which each letter in the alphabet is rotated by  three letters as shown**
- Example :-``A B C D E F G H I J K L M N O P Q R S T U V W X Y Z``
-           ``D E F G H I J K L M N O P Q R S T U V W X Y Z A B C``
…
## Substitution Cipher Using a key to shift alphabet 

- Obtain a key to for the algorithm and then shift the alphabets
- For instance if the key is word we will shift all the letters by four and remove the letters w, o, r, & d from the encryption
- We have to ensure that the mapping is one-to-one
-          A B C D E F G H I J K L M N O P Q R S T U V W X Y Z  =  is is orginal alphabet 
-        ``H E Y ``A B C D F G I J K L M N O P Q R S T U V W X Z = this is start with H E Y this means the Ciper is HEY
-          and we can not include ciper texts  EXAMPLE   JGGK FGN =  HEY and decribted =   KILL HIM 
  
- no single letter in plain text can map to two different letters in cipher text
- no single letter in cipher text can map to two different letters in plain text Website: [rot13.com]
- Replacing the letters by 1 shift 
- we can get different rotations. To do this we can use this website.
- This encoding is called ``rot encoding``
## Limitation
- Any exposure to the secret key compromises confidentiality of ciphertext
- A key needs to be delivered to the recipient of the coded message for it to be deciphered
- Some intruders can get the key  No secret anymore.

## Asymmetric Encryption 
- Uses a pair of keys for encryption
- a) Public key for encryption
- b) Private key for decryption
- **Messages encoded using public key can only be decoded by the private key**
- Secret transmission of key for decryption is not required
- ** Public key can be exposed so, if i need to send you a message i just ask you for your public key and i will encrypt the message with your public key.**
- When you get the ciphertext you can decrypt it with your private key.
- Every entity can generate a key pair(private&public) and release its public key
## Types of asymmetric encryption.
- ### Two most popular algorithms are RSA & El Gamal
##  RSA
- Developed by Ron Rivest, Adi Shamir, Len Adelman
- Both public and private key are interchangable
- Variable Key Size (512, 1024, or 2048 bits)
- Most popular public key algorithm
- It have a maths formulas for generating the keys.
## El Gamal
- Developed by Taher ElGamal
- Variable key size (512 or 1024 bits)
- Less common than RS
- Terms of Cryptography
## 1) Encoding/ decoding
a) **This is a method of creating Cipher text with our using any key**
b) This can be done by doing math on the given input/substitution
i) Examples: base64,base32,rot…
## 2) Encrypting/Decrypting
a) This is method of creating Cipher text with keys.
b) To decrypts this kind u need to have the private key
i) Example: DES,AES,RSA 
## 3) Hashing
a)**This is a method of creating Cipher text with respect to a created hash**
b) To reverse the hash, you just search for some match, you don't decrypt/decode it.
c) Salt: is a random string used for data modification for password protection.
i) Example: MD5,sha254,... 
- Kinds of encodings/encryptions
- Base2 01100010 01110010 01100101 01100001 01101011 01101001 01110100
- Base8 142 162 145 141 153 151 164
- Base16 62 72 65 61 6b 69 74
- Base32 MJZGKYLLNF2A====
- Base58 4jP4KDubX1
- Base62 22udqyscMu
- Base64 YnJlYWtpdA==
- Base85 @WH$gCM@k
- Base91 %zmfv;:YH
- URL encode: hello%20there%20%3F
- Md5: 5d41402abc4b2a76b9719d911017c592
- Sha1: aaf4c61ddcc5e8a2dabede0f3b482cd9aea9434d
- Rot : Uryyb, Frphevgl Grfgref => look for some random word that looks rotated tools
- There are lots of encodings/encryption
- To identify this we will need some 
- ools/sites
###  Tools: 
1) **hashid**
2) **hashid <hash>**
3) **(Cyber chef )(web)[https://gchq.github.io/CyberChef/]**
4) Hashes
5) Craskstation.net(non-salted)
6) Own cracking(google the name)
7) Encodings
8) Crackstation
- We use from to decrypt
- We use to to encrypt
