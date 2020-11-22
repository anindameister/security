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

- calculating public and private key [[2]](#2).

![Keys](https://github.com/anindameister/security/blob/master/snaps/270.PNG)

- visualising in a practical scenario

![Keys](https://github.com/anindameister/security/blob/master/snaps/271.PNG)

#### three questions as below came up, which led to the origin of certificate

![Keys](https://github.com/anindameister/security/blob/master/snaps/272.PNG)

- question 1: so Philip Jallion is working in ecoleD'mines now and someone(an ex student) sends an email to him. Considering that the email account was never deleted, so the email is processed and would be attempted to be downloaded to Philip's Jallion computer which has been put on charge-connected to network and left alone forever. This downloading would happen because the publicKey is being handled by the Linux operating system and not by the user.
- here's one thing that Professor mentioned, is that windows dont trust public keys
- question 2. The owner couldn't be trusted because based on the answer to Q1 we understand that owner has left. So the user who's available or not, cannot be trusted any longer.
- Q3. yeah valid or not , but all the above questions give birth to certificate.

# certificate

![Keys](https://github.com/anindameister/security/blob/master/snaps/273.PNG)

- the below diagram is just represneting the above with no additional info

![Keys](https://github.com/anindameister/security/blob/master/snaps/274.PNG)

- Classification of certificates, so this is really what lets us know about what a certificate is a represntation of

![Keys](https://github.com/anindameister/security/blob/master/snaps/275.PNG)

- 
- for apps: in my personal computer, suppose we're trying to install an app so this app's code is verified by the private key present within windows os which would decrypt(possibly) the certificate that comes with the app to verify the app.
- the decryption of the certicate of the app by os in the client computer, because we dont want someone else to project themself fasely and get their app installed in our computer.

- Situation: I download eclipse, change the internal code of eclipse and upload it to my personal repository. I wont be able to hack people unless anyone downloads the app from my site.
- so it's advisable to download eclipse from official website, so that once app is downloaded then it's certificate can be decrypted by some private key present within my os.

- The most commonly used certificate usage is in regards to accessing some website.
- certificate validity of a website is required because it's on the network, and this network can never be trusted.
- let's say today, I replicate eclipse website but even then it's not gonna show up in the search engine because the certificate can be just one and not two, maybe, so two website cannot have the same certificate. Something like this.

![Keys](https://github.com/anindameister/security/blob/master/snaps/276.PNG)

- user authentication: so if a client wants to access my folder available on my computer which is also hosted in the website then this client must have anindaFolderCertificate which was provided while creating an account in my website.
- now, Pauline is a client who pays to watch tutorialVideos in my website. Pauline friend Aditya copies the certificate from Pauline's computer and attempts to access from his computer.
- Aditya wont be able to access because Paauline's ip is integrated in her certificate.
- Now Aditya, manipulates his computer to have the same global ip as Pauline, it wouldn't work because no two computers in the world can have the same ip
- Again, Aditya makes Pauline go offline and then assigns Pauline's global ip to his computer; now probably he has access if other factors are not considered when certificate is generated for a particular ip address.
- so Aditya gets into anindaFolder, and that's it. But he can only view and not edit; because of the permission as of right now.
- Anyway, since this section is an example section for certificate, the concept for downloading... and electronic commerce remains the same

 ![Keys](https://github.com/anindameister/security/blob/master/snaps/277.PNG)
 
- The slide is self-explanatory.
- I can sign my own certificate if am the ultimate with my own private key. This kind of certificate is the root certificate

 ![Keys](https://github.com/anindameister/security/blob/master/snaps/278.PNG)
 
- self explanatory slide.
- so let's consider Eclipse certificate.
- this Eclipse certificate would contain info such as, "I am signed by eclipseCommunity".. check the smide, very simple.. 
- To trust a certificate, we got to trust the root certificate of the chain.
- Me trying to act like EclipseCommunity, wouldn't be able to get the signature who verifies me. Let's consider that PierreMaret is my boss, and I need him to verify me by signing by pen.(14:42)

 ![certificate content](https://github.com/anindameister/security/blob/master/snaps/279.PNG)
 
- There are two parts: Data and Signature
- Data part contains the whatever in slide
- Issuer is whoever has issued the certifcate
- Subject is: Philip Jallion from ecoleD'mines
- Subject Public Key: RSA
- so the data part cannot be changed
- if someone is able to able to change the data part, then the signature algorithm wouldn't run in the signature part and this certificate wouldn't be able to be verified
- so if an app, wants to validate this certificate then it needs to trust the issuer.


## References
<a id="1">[1]</a> 
https://www.gatevidyalay.com/cryptography-symmetric-key-cryptography/#:~:text=In%20symmetric%20key%20cryptography%2C,secret%20keys%20would%20be%20needed.

<a id="2">[2]</a> 
youtube.com/watch?v=0T0LdzQ9L6g

