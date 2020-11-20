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


## References
<a id="1">[1]</a> 
https://www.gatevidyalay.com/cryptography-symmetric-key-cryptography/#:~:text=In%20symmetric%20key%20cryptography%2C,secret%20keys%20would%20be%20needed.

