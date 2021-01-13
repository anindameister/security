### Describe the global infrastructure (with required equipment placed) of your solution (take into account all different users populations: general population, administration, medical teams)

- My proposal for contact tracing app would be something that can be downloaded in apple and android phones.Once installed to start it will ask for location access and phone number verification would be done with One time password. Once the user is authenticated. Few questions related to Covid 19 will be asked. Like if the user travelled to any of the foreign countries?, if user is facing any symptoms of coughing,feverish,lack of smell. User needs to give the answer honestly. Based upon the user answers user will be marked safe , might be affected and need a test or is Covid positive and needs to be either admitted or self quarantine. The contact tracing app will have 4 tabs. which is 
- **Status**  of the user which can be safe, might be infected,is infected.
- The 2nd tab would be **Media** to get some videos which are trending related to covid-19. 
- The 3rd tab would be **Covid Update** in this tab all information related to the contry status like Total infected count, Recovered count, deceased count will be present. Even user can select which region of the country she belongs to. The covid infected patient in 500m,1km,10km,20km. The user will be traced by BLE and location only Covid positive user. 
- The last tab would be **E-Pass** if users are travelling via flight or via train. There is no need to have a physical tickets in paper. User can provide there booking id and get the ticket QR code in the smart phone. In this way there will be no physical contact between two person. The ticket purchasing will be completely digitalised. For the app to work properly 60percent to 70percent of the population should  install.
 
- Now, I will propose about the data access the user location data will be deleted from the central server after 45days.
- Government will have limited access to the only covid positive infected person details, only for 45days. 
- User details will not be conveyed to the other user. 
- But if person X who is covid positive came in contact with Person Y in the last 7 days, then Person Y will be notified to take a covid test. 
- Suggestions for nearest covid test center will be shown based on user's location.
- The medical teams would only get the data access like medical history of the infected patient which would be available for 45days.

### What are the main security points you should take into account in your solution and explain how you solve it?

- The key protocol will be based on DP3T protocol.The decentralised protocol is more secured. The main privacy key points that my proposed app will follow is:
1. Data Minimization: Only the anonymous id of the infected person is captured here. This will decrease the eavesdropping.
2. Prevent abuse of data: Since only minimum information is captured,it prevents misuse of data.The data will also be deleted after 45days from the central server and also from the user's device.
3. Prevent the tracking of non-infected users: The infected users need to proactively update in the app that they are covid positive.Only then the contact tracking of that user will be activated. No, entity including the backend server can track non infected user based on broadcasted identifiers.
4. Ensure Graceful Dismantling: As mentioned earlier data on the server is removed after specific number of days,for example 45Days.
The contact tracking app will work on both BLE and location tracking. The location tracking will only be activated when user submits himself as positive.For non infected user it wont be tracked. User Alice updates that she has been tested positive.User Bob's phone would be alerted as he had enough messages from Alice's phone.Bob needs to down the file that has been alerted. If the file from the centralised server will be matched with the local messages.If matches are found based on the alert either Bob can take necessary action. Meanwhile, hospitals will be alerted of Alice's infection but they would not have the information until and unless Alice want them to see. The UID of the users are never shared. Only the secret key if user wishes to can be shared to the centralised server in order to report Covid infection. 
- The messages exchanged between Alice and Bob are EphId which is updated every few minutes.Some that eavesdropper could not listen to the message.The number of EphID will vary from the psuedo generator.In this way neither the hospital, nor any admin or other fellow user will get to know any user details.


## Me

- Let me consider myself to be App developer, so, my first consideration would be putting across  the  best  design.   Best  design  can  be  put  across  my  choosing  the  right  colours.There’s a complete domain about Colour Science, maybe, I should consult a colour Sci-ence expert to do a proper design. There’s a reason, that I am giving preference to colour and design, and my reason is to create a willingness by the user to use this app. The mostpopular apps, like Facebook, makes sure that the design is good. I used to be an addictive Facebook user.   In order to lose this addiction,  I moved to using Facebook in phone’sbrowser which would help me interact with ugly interface thereby helping me to reducethe Facebook time.  A couple of months ago, one fine day, I found out that the browserexperience has become exactly the same as the app.  Based on this, it is very important to note that designs matter.   Just another point,  the application should be very easy to use.  People dont like writing a lot of information, specially elderly people, so I wouldprefer letting users allow the app to take information from social-ID. Now, if I have to talk about below the poverty-line users, illegal immigrants who have just been introducedto smart phones during this pandemic, then they need to type manually in their preferredlanguage.  So, my app should support multiple language because poverty doesn’t have acast,creed,language or religion. This concludes the first page of the app. 
- The second page of the app would be filled with the medical details the user has, and this information would be derived from the social-ID which is linked to medical profile, most of the time. This page would also have more details with the title, **How are you feeling today**.. We would try to include check boxes in regards to the Covid-19 symptoms like the follows

![symptoms](https://github.com/anindameister/security/blob/master/snaps/2274.PNG) [[1]](#1).

- The idea is not to make the user, panic, about the symptoms and efforts would be put to ease on the questions. Several testing would be done before the app release. Moreover, based on the user information, he/she would be notified if that person needs to visit a testing center, stay in home quarantine for some number of days. Efforts would be also put, to display the current appointment status of the testing centers and facities would be provided to add an appointment for self.

- The third page of the app, should have a simple interface, where government authorised body can post information about the advantages of using natural ingredients during this pandemic.  We have to make sure, that this interface is free from any kind of advertisement.This app should be non-profit app. There would be other information like Total infected count, Recovered count, deceased count in regards to area of coverage starting from 2 kms to the end, as much as possible.

- There would be a fourth page, where the user needs to go to before getting out of the house. In this page, camera activation facility to make payments, storing-deleting options in regards to keeping credit-card information for contact-less payments to shops, train stations and so on. 

- All the user details would be stored in a central server, which would not be accessible by ay government bodies. The user details would be deleted from the central server after 30 days.

- There would be a fifth page, where the user would be notified if he/she has come in contact with a Covid 19 and would be suggested to go to a testing center. This page would also contain the option to self proclaim being Covid-19 positive. This page would also contain the option to facilitate priority based appointment for such users.
- This part was all about the user experience.
- About the technical part, the app should be compatible with ios, android, windowsand linux based phones. Ios, android phones captures user-location irrespective of user’s knowledge.  The idea would be to use these features and also notify the users about the vulnerabilities.  Some techies find ways to stop the location services in their phone, sosuch techies should be notified that this app works best with location services, so they can choose to switch on the location services.

###  What are the main security points you should take into account in your solution and explain how you solve it.

- As a contact-tracing app developer, I have chosen the Robert Protocol. 
- I would set the settings of the Robert Protocol to standards.  
- I completely understand the vulnerabilities. A regular phone is made vulnerable by the phone manufacturer, network provider and theapps.  So, if we understand, the biggest vulnerability is choosing to use a smart phone.
- A  contact  app  designer  doesn't have any self-ulterior motive. 
- Anyway,the backend design would be put in place to support the standard settings of the Robert protocol.
- So, we have a concept of introducing premium versions of same apps.  Given the opportunity, I would design the premium version of this app with the same facilities but with DPT3 protocol. The premium version would be available only to the army personnels. Right now, I understand that a single app cannot be designed for different security protocols. So, I would strongly recommend that my app with Robert Protocol is not used by army personnels.
- My points are:
    - Data: All the data of the user would be in the device itself. The cypher text version of the data would be stored in the central server. Absolute efforts would be given to prevent any data-leak or eaves-dropping by any un-authorised personnel or government bodies.Moreover, the data would be also deleted from the user's phone and the central server at the end of 30 days, and it would be made mandatory to fill in the same details as before by the user. 
    - Trust and Privacy: This app would not be able to gather any information from other apps. However, text message services can be accessed only with user permission.


## In the two protocols, a server is required at exposure verification and infection declaration.
- Imagine you are the owner (administrator) of the server and be able to observe all communications
with your server at any time.
- Imagine you are a telcom operator and be able to to observe all communications, you are also able
to localize cell phone.
- in these two situations, explain how the flows could be exploited, what the attacker could
learn and what protocols’ properties cannot be respected.

## Answer
- Location traceability. The decentralized design limits the potential for location tracking to users who have received a positive diagnosis and for the course of the contagious period.In centralised systems in which keys are generated on the server, access to server-sidekeys  (e.g.,  the  backend  itself  or  law  enforcement)  enables  linking  ephemeral  EphIDs to the corresponding permanent app identifier.   This enables tracing/identifying people based  on  EphIDs  observed  in  the  past,  as  well  as  tracing  peoples’  future  movements.When keys are generated on the phone and not used directly as EphIDs.

    - Location data: The decentralized design prevents location tracking of Covid-19 postive patients during their contagious period.In centralised systems, keys are genenerated on the server. Access to these server side keys, enables linking EphIDs to app indentifier which in turn facilitates the user identification and enables tracking their further movements.

- COVID-19 positive status.   The centralised and decentralised proximity tracingsystems share the inherent privacy limitation that they can be exploited by a tech-savvyuser to reveal which individuals in their contact list might be infected. However, the cen-tralised designs hide when and how often the user was in contact with a COVID-positivepatient.  As a result,  tech-savvy attackers cannot benefit from linking between EphIDsand timing information to amplify their attack.   Instead,  they need to rely on multipleaccounts. Depending on whether the centralized designs deploy dummy traffic correctly,network eavesdroppers might still learn the COVID-19 status of users of the system.

    - COVID-19 positive: The centralised and decentralised systems have the same privacy limitation which could be exploited to get the infected user list. The centralised system hides Covid-19 positive user's identity well, thus EphIDs cannot be used to pin-point Covid positive user. However, network eaves- dropping and centralised system's dummy traffic bypassing can be used.

- The type of data being collected on Bluetooth connections could reveal informa-tion about families, societies, and communities.

    - data collection: Bluetooth data could reveal family,community information.

- Fake exposure events. Triggering false alerts is easy in all centralised designs andcan be done retroactively by any tech-savvy COVID-19 positive user.

    - Fake alerts: In centralised system, a user can trigger fake Covid alert
- Suppressing at-risk contacts.  Hiding at-risk contacts is possible in any proximitytracing system.

    - Identification protection: Covid 19 patient's ,thereby at-risk user's identity can be hidden in proximitytracing system.




- Regarding the ROBERT’s authentication and access control, 
    - it is a mandatory access control, in which the access right will be set up by the central authority which will set a multiple level regards security. This is considered a high security model where it is used in sensitive organisations such as military environments. Also one of these model advantages is that classifications are assigned to the system resources and OS in which allow or deny access to specific resources based on the clearance of information security.
- While DP-3T’s access control model 
    - is a discretionary access control, 
    - because of DP-3T use decentralize protocol therefore it was the appropriate access control model. Where the users of the system will only themself allow to know the information collected on there device. In this model the owner of the system who will set the policies and define the authorized people to access the data or resource. In DP-3T the data only will be sent to the back-end server if the user wants (the user responsibility).

## References
<a id="1">[1]</a> 
https://www.cdc.gov/coronavirus/2019-ncov/symptoms-testing/symptoms.html