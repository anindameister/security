- PKI

![Intro](https://github.com/anindameister/security/blob/master/snaps/266.PNG)

- okay, so let's consider two people: me & Pauline
- I want to securely take access to her computer, without revealing her computer identity: let's consider the global ip address & key to access via a custom made app created by me to take remote access.
- The custom made app was created as a part of security project which was just associated to some topics like networkSecurity,Cryptography,InformationSecuritySystem,SecurityTrust&Privacy
- Now, considering I have read all the above topics with proper care, without missing out anything; got to check later then the app that I created has certain features apart from taking&giving remote access
- The features are authentication, confidentiality, integrity, signature(dont know which chapter this belongs to)
- We need to also take care of legitimacy, validity,usage as well
- APart from the problem of legitimacy,validity,usage; there's the problem of managing keys

![Keys](https://github.com/anindameister/security/blob/master/snaps/267.PNG)

- DES,AES they all use symmetric encryption
- symmetric encryption is about using just one key for encryption and decryption process
- In symmetric key cryptography, Each pair of users require a unique secret key. 
- If N people in the world wants to use this technique, then there needs to be N(N-1) / 2 secret keys.  [[1]](#1).
- For 1 million people to communicate, a half billion secret keys would be needed.
- so the below is the formula and it's verification.

![Keys](https://github.com/anindameister/security/blob/master/snaps/268.PNG)

#### rsa

- basic public and private key

![Keys](https://github.com/anindameister/security/blob/master/snaps/269.PNG)

- calculating public and private key

![Keys](https://github.com/anindameister/security/blob/master/snaps/270.PNG)

- visualising in a practical scenario

![Keys](https://github.com/anindameister/security/blob/master/snaps/271.PNG)

#### three questions as below came up, which led to the origin of certificate

![Keys](https://github.com/anindameister/security/blob/master/snaps/272.PNG)

- question 1: so Philip Jallion is working in ecoleD'mines now and someone(an ex student) sends an email to him. Considering that the email account was never deleted, so the email is processed and would be attempted to be downloaded to Philip's Jallion computer which has been put on charge-connected to network and left alone forever. This downloading would happen because the publicKey is being handled by the Linux operating system and not by the user.
- here's one thing that Professor mentioned, is that windows dont trust public keys
- question 2. The owner couldn't be trusted because based on the answer to Q1 we understand that owner has left. So the user who's available or not, cannot be trusted any longer.
- Q3. yeah valid or not , but all the above questions give birth to certificate.



## References
<a id="1">[1]</a> 
https://www.gatevidyalay.com/cryptography-symmetric-key-cryptography/#:~:text=In%20symmetric%20key%20cryptography%2C,secret%20keys%20would%20be%20needed.

