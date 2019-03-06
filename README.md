# hearing-enhancement-project

## Crowdsourced Hearing Enhancement

The basic idea is that all the users share their experiences in order to improve each others hearing. 
They share: 
  1) sound environments 
  2) their hearing deficiencies and 
  3) success/failure of enhancement provided to them. 
  
Sharing is accomplished using the Cloud for storage and for processing.

Each user has earbuds and a smart phone and a connection to the internet and thus the Cloud. The earbuds provide the actual speaker that introduces enhanced sound to the user’s ears. The enhancement is tailored to the user and is based on the shared experiences of the other users.

The problem to be solved: 
Hearing quality is affected by the sound environment and the capabilities of the listener. A noisy environment can reduce   the quality of hearing as does a reduced capacity (being “hard of hearing”). Every sound environment is different as is every hearing disability. However there are similarities to be taken advantage of, when working to enhance the quality of hearing for individuals with normal or reduced hearing capability. Currently there is no hearing aid nor voice enhancing earbud that has sufficient flexibility, or adaptability to achieve real enhanced speech. 

### Overview:
  1) The users wear earbuds and have a smart phone with internet access.
  2) The Cloud is available to provide storage and processing
  3) The current sound environment is captured by the earbuds and phone and passed up the the Cloud for identification.
  4) The Identification process identifies and classifies the sound and sound components. 
        (watching TV, in Joe’s Pub, in the weekly company conference, in math class..)
  5) The Cloud process selects a sound target to be enhanced, based on past experiences, which were provided by
        feedback from the user as well as feedback from the community of users (particularly when the sound environment 
        is new to the user.
  6) Using knowledge of the user's hearing capabilities and the proposed sound target, a set of required enhancement 
        tools is determined.
  7) Using knowledge of the users hearing capabilities and the proposed sound target, a set of enhancement parameters 
        for the selected tools is constructed and passed to the earbuds.
  8) Tools not currently present in the user’s earbuds are downloaded to the user’s earbuds.
  9) The parameter set is passed to the user’s earbuds.
  10) The earbuds process incoming sound and enhances the target.
  11) The user provides feedback as to quality of enhancement as well as selections of the target sound.
  12) Cloud adapts to the response with improvements or confirms that the decisions have been made correctly and 
        records that information for future reference.


### System Components:
#### Earbuds:
- Provide the speaker that delivers enhanced sound to the user.
- Take environmental sounds from onboard microphones, blue tooth mic., bluetooth connection to smart phone, bluetooth transmitter plugged into sound system (like Zvox, or room sound system)
- Use stored filters and enhancer tools to produced enhanced target sounds.
- Provide the latency dependent execution of toolset.
- Produces enhanced target sounds through processing input sounds using the customized toolset and associated parameters
- Open Standards are provided for all data access, tools and API used on the earbuds

Note: Processing may be done in the Smart Phone in order to avoid having to create earbuds with processing capability. 

#### Smart Phone:
- Provides internet access for communicating with Cloud.
- Transmitting current sound environment up to Cloud
- Receiving new tool sets 
- Receiving parameter sets
- Provides user interface to:
- Give feedback on quality of enhancement
- Provide input on target sounds
- Provides initial testing of user’s hearing capabilities.
- Provides latency tolerant processing needed for enhancement
- Open Standards are provided for tools, data access and APIs used on smart phones
#### Cloud Storage:
- Provide storage sound environments accumulated from all users.
- Provide security and privacy for the users’ data and identity.
- Provide tools and parameter sets 
- Keep history of success and failure of enhancement 
- Keep user specific record of capabilities and current state
- This storage is OPEN to all users and providers. 
- The community history is a growing collection of data that can serve as training data for new toolsets and for improving existing strategies.
- Open standards are provided for storage and API for accessing data
#### Cloud Processing:
- Recognizes current sound environment with emphasis on specific user’s history, but also utilizing community of users history.
- Deconstructs environment into components parts
- Determines target sounds, from user’s history or request as well as community of users history.
- Determines strategy for enhancing target sounds using:
- Current user’s hearing capability
- History of successful enhancement (this user as well as community)
- Toolset available to the user.
- Feedback when provided by the user.
- Simulation of enhancement when history does not provide guidance.
- User experience as well as community experience assists in selection of enhancement strategy.
- Deep Learning techniques are expected to be used in sound separation as well as enhancement strategy assembly.
- Open Standards are provided for tools and tool APIs.

#### Community of Users:
By collecting the experiences of a large community of users, each individual user gains. 
Strategies that have been successful in others can be used.
Experiences new to an individual user may exist in the larger community and already been processed to enhance hearing.

#### Community of Developers:
Developers of devices, algorithms and tools can take advantage of the potentially vast array of data available for sound experience.
Developers can provide tools and algorithms as open source or perhaps objects available in the hearing community equivalent of the App Store. 

#### Service Provider:
The speech enhancement service is provided for a small fee in order to fund the cloud storage and processing. 

#### Security & Privacy:
Given that users are providing environment information which includes sample sounds, privacy must be maintained. When environments are used to support a user that has not provided the specific environment sample, the providder must be anonymous. However, a user should have access to the environment samples they provide. Some form of encryption must be used regarding identity. 

#### Scenarios:
##### Math Class: 
Sitting in class the start of lecture is captured and sent to the Cloud. Since you have been attending math class now for several days, the sound environment is recognized. It is a lecture and the speaker is Mr Brown. A set of enhancement tools and parameters is selected and sent to the earbuds to enhance Mr Brown’s speech. He is coming in clearly and you acknowledge it.

Midway through the lecture Mr. Brown introduce Ms. Jones to discuss differentiation. The environment changes. The enhancement must change. Ms. Jones is new to you. However, she taught in the class down the hall where your friend attended and her speech characteristics are recognized and a new set of enhancement tools and parameters customized for you are created and passed to your earbuds. Enhancement is acceptable but not as good as for Mr Brown. You indicate that and the Cloud looks for improvements.

##### Driving:
You are listening to the news on the radio on the way to work. Your earbuds pickup the current environment, pass it to the Cloud and a toolset and parameter set are passed back to the earbuds. Sound is good. Now you get on the expressway and are driving at 65 with the window down. The new environment is captured by your earbuds and you smart phone sends it up to the Cloud. It is recognized, since you do this every day. A tool set and parameters are passed to your earbuds and the news becomes enhanced in the new environment. You switch from news to Lady Gaga on Pandora. The sound environment changes, is passed up to the Cloud and a new set of tools and parameters if easily found since you are a Lady Gaga fan.  Next a guitar solo comes on. It’s new. The sound is captured and sent to Cloud for recognition. Performer unknown, but guitar recognized. Updated tools and parameters are sent and all is good.

##### Partying:
You are at Vescio’s restaurant with a group of friends. It is Saturday night and the place is full of patrons. There is also an Italian concertina musician playing. Your earbuds pick up the environment and pass it to the Cloud processing. The sound components are identified. The sound sample does not compare identically with anything stored, but is does resemble a class of restaurant sounds with the exception of the concertina. Your friends voices are identified from past samplings and will be isolated. The required tools and parameter settings are selected for isolation of the friends voices from the surrounding noise and music. Some additional tools had to be downloaded, since you have not been in a restaurant setting with a group of friends for a few weeks. Thus the set of cached tools does not contain all that are needed. You are now able to hear your friends conversations clearly. The waiter comes to take your order. This is a new voice, but need not be identified specifically since it is in the class of human voices at close range and can thus be sufficient enhanced or at least not removed. You decide to listen to the music, so you indicate that on the smart phone and the concertina is no longer removed from the sound environment. Your general satisfaction (since you did not complain) is recorded in Cloud storage. Your friend Joe has the same enhancement equipment, but has no hearing disability, thus his tools and parameter settings are different, but the process is the same.   

