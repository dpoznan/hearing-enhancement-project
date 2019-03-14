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
Given that users are providing environment information which includes sample sounds, privacy must be maintained. When environments are used to support a user that has not provided the specific environment sample, the provider must be anonymous. However, a user should have access to the environment samples they provide. Some form of encryption must be used regarding identity. 

#### Scenarios:
##### Math Class: 
Sitting in class the start of lecture is captured and sent to the Cloud. Since you have been attending math class now for several days, the sound environment is recognized. It is a lecture and the speaker is Mr Brown. A set of enhancement tools and parameters is selected and sent to the earbuds to enhance Mr Brown’s speech. He is coming in clearly and you acknowledge it.

Midway through the lecture Mr. Brown introduce Ms. Jones to discuss differentiation. The environment changes. The enhancement must change. Ms. Jones is new to you. However, she taught in the class down the hall where your friend attended and her speech characteristics are recognized and a new set of enhancement tools and parameters customized for you are created and passed to your earbuds. Enhancement is acceptable but not as good as for Mr Brown. You indicate that and the Cloud looks for improvements.

##### Driving:
You are listening to the news on the radio on the way to work. Your earbuds pickup the current environment, pass it to the Cloud and a toolset and parameter set are passed back to the earbuds. Sound is good. Now you get on the expressway and are driving at 65 with the window down. The new environment is captured by your earbuds and you smart phone sends it up to the Cloud. It is recognized, since you do this every day. A tool set and parameters are passed to your earbuds and the news becomes enhanced in the new environment. You switch from news to Lady Gaga on Pandora. The sound environment changes, is passed up to the Cloud and a new set of tools and parameters if easily found since you are a Lady Gaga fan.  Next a guitar solo comes on. It’s new. The sound is captured and sent to Cloud for recognition. Performer unknown, but guitar recognized. Updated tools and parameters are sent and all is good.

##### Partying:
You are at Vescio’s restaurant with a group of friends. It is Saturday night and the place is full of patrons. There is also an Italian concertina musician playing. Your earbuds pick up the environment and pass it to the Cloud processing. The sound components are identified. The sound sample does not compare identically with anything stored, but is does resemble a class of restaurant sounds with the exception of the concertina. Your friends voices are identified from past samplings and will be isolated. The required tools and parameter settings are selected for isolation of the friends voices from the surrounding noise and music. Some additional tools had to be downloaded, since you have not been in a restaurant setting with a group of friends for a few weeks. Thus the set of cached tools does not contain all that are needed. You are now able to hear your friends conversations clearly. The waiter comes to take your order. This is a new voice, but need not be identified specifically since it is in the class of human voices at close range and can thus be sufficient enhanced or at least not removed. You decide to listen to the music, so you indicate that on the smart phone and the concertina is no longer removed from the sound environment. Your general satisfaction (since you did not complain) is recorded in Cloud storage. Your friend Joe has the same enhancement equipment, but has no hearing disability, thus his tools and parameter settings are different, but the process is the same.   


## Algorithms and Prototyping

### Introduction

The Crowdsourced Hearing Enhancement project has several technical components: cloud storage and processing, hearing correction, real time user interaction, machine learning, and speech enhancement/speech separation. This paper describes the speech separation work to be done as part of the Crowdsourced Hearing Enhancement Project. The project allows participants to share their experiences in order to improve each others hearing. It provides storage, processing, and interaction support that allows hearing enhancement tied to environments and experiences of the community of users. Hearing enhancement has two key components: 1) correction/amplification and 2) speech separation. Traditional hearing aid technology provides correction of received audio based on an audiogram and assists users who have a hearing impairment. Speech separation provides a user a clearer reception of voices in an environment that may  make understanding speakers difficult.

Correction is accomplished in the traditional hearing aid style of enhancement of the sound level/volume for frequency ranges for which the hearer has deficiency.

Speech separation is the underlying machine learning technique that is used to provide hearing enhancement. The support environment allows training and supervised learning to be accomplished and used to identify a user’s environment and provide specialized hearing enhancement to the individual participant. 


### Speech Separation

The goal of speech separation is to separate specific speech from sounds in the environment and therefore providing better understanding. This capability is applicable to both the hearing impaired and normal hearing participants in the project and is a key component of hearing prothesis, and speaker recognition. [1]  It is a long standing problem identified and given the name “cocktail party problem” in 1953 by Cherry [2]. DeLiang Wang and Jitong Chen’s paper [1] provides an overview of the current state of supervised speech separation. The material in this paper provides a starting point for implementing the speech separation (SS) component of the overall project. SS algorithms are divided into the following components: learning machines, training targets and acoustic features. 

### Learning Machines
Deep neural networks (DNN) have been used in in speech separation. They include Muti-layer perceptrons (MLPs), convolutional neural networks (CNNs), recurrent neural networks (RNNs), and generative adversarial networks (GANs). The DeLiang Wang paper [1] reviews these learning machines applied to speech separation. Yao, et al [6] introduce a new neural network building block, the STFNet, Short Time Fourier Neural Network

#### MLP
MLPs have improved with recent use of ReLUs instead of traditional sigmoid activation function when using large training data. Also, the use of skip connections facilitate training of very deep MLPs.

#### CNN
CNNs have been recognized as well suited for pattern recognition. The CNN architecture is a cascade of convolutional layers paired with subsampling layers. The convolutional layer consists of multiple feature maps that extract a local feature.

RNN
RNNs treat the input as a sequence and model the changes over time, and allow feedback connections between hidden layers. Speech has a strong temporal structure and thus RNNs are a natural choice. For speech long short-term memory (LSTM) is used to introduce memory cells with gates  to avoid the problem of exploding or vanishing gradients [3].

#### GAN
GANS have recently been introduced with a generative model and a discriminative mode simultaneously trained [4]. A generator learns to model the mapping from noisy speech to the clean counterparts, while a discriminator learns to classify between generated and target samples. GANs use the discriminator to shape the loss function of the generator.

#### STFNet
STFNets integrate neural networks with traditional time-frequency analysis, and designs fundamental spectral-compatible operations for Fourier-transformed representations. STFNets were shown to outperform deep-learning-models under diverse sensing modalities.


### Training Targets
In speech separation there are two groups of training targets: masking based targets, and mapping based targets. The masking based targets describe the time-frequency relationships of clean speech to background interference. 

The primary masking based targets are: 
Ideal Binary Mask (IBM)
Target Binary Mask (TBM)
Ideal Ratio Mask (IRM)
Spectral Magnitude Mask (SMM)
Phase Sensitive Mask (PSM)
Complex Ideal Ratio Mask (cIRM).

The mapping-based targets correspond to spectral representations of clean speech. 

The mapping-based targets are: 
Target Magnitude Spectrum (TMS)
Gammatone Frequency Target Power Spectrum (GF-TPS)
Signal Approximation (SA).

Wang and Chen [1] compare a number of training targets using a feed forward DNN with three hidden layers and the same input features. Evaluation of the separated speech is performed using short-time objective intelligibility (STOI) and perceptual evaluation of speech quality (PESQ) scores. 

In terms of STOI the masking based targets outperform the mapping based targets. However, a recent study shows that this holds only for higher signal to noise ratios. At lower SNRs the mapping targets are better. For PESQ ration masking performs better than binary masking.
Overall, the IRM and the SMM emerge as preferred targets. In addition, DNN based ratio masking performs substantially better than supervised nonnegative matrix factorization (NMF) and unsupervised speech enhancement.
### Acoustic Features
Features as input and learning machines can play a complimentary role in speech separation via supervised learning. The value of feature extraction has been evaluated in [1] as well as in [5] which examines 19 features for providing improvements in short term objective intelligibility (STOI). It was determined that Multi-Resolution Cochleagram (MRCG) has the best average STOI improvement, in particular for noisy environments.


### Algorithms
There is significant activity in both monaural and array separation algorithms. For the initial activity in this project the focus with start with dual channel algorithms, since the initial prototype IoT device has dual microphone, dual headset.


## Initial Speech Separation Implementation


### Integration into System

#### IoT Hearing Device
The prototype IoT device that capture sound input and delivers processed sound is a prototype hearing aid. Constructed from a raspberrypi computer, a Flatmax sound card, Roland binaural microphones/earphones and S/W including openMHA, based of information from website/Wiki by Marc René Schädler. (https://github.com/m-r-s)

#### Cloud Resources


## References

[1] DeLiang Wang, Jitong Chen, “Supervised Speech Separation Based on Deep Learning: An Overview”, 2017.

[2] E.C. Cherry, "Some experiments on the recognition of speech, with one and with two ears," J. Acoust. Soc. Am., vol. 25, pp. 975-979, 1953.

[3] R. Pascanu, T. Mikolov, and Y. Bengio, "On the difficulty of training recurrent neural networks," in Proceedings of ICML, pp. 1310–1318, 2013.

[4] I.J. Goodfellow, et al., "Generative adversarial nets," in Proceedings of NIPS, 2014.

[5]  J. Chen, Y. Wang, and D.L. Wang, "A feature study for classification-based speech separation at low signal-to-noise ratios," IEEE/ACM Trans. Audio Speech Lang. Proc., vol. 22, pp. 1993-2002, 2014.

[6] S. Yao, A. Piiao, W.Jiang, Y. Zhao, H. Shao, S. Liu,D. Liu, J. Li, T. Wang, S.Hu, L.. Su, J. Han, T. Abdelzaher, “STFNets: Learning Sensing Signals from Time-Frequency Perspective with Short-Time Fourier Neural Networks”, WWW’19, May 13-17, 2019.
