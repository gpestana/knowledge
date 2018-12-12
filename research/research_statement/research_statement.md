---
title: "Research Statement - Privacy Preserving Decentralized Systems"
author: "Gonçalo Pestana (gpestana@protonmail.com)"
date: Dec 2018
---

This document motivates and summarizes my research goals for the short and long term. In addition, it outlines initial ideas for potential research topics, leaving literature review and further details for a later document. 

## Research goals
 	
As a researcher and engineer, my long term goals are to study and build privacy preserving technologies that are secure and private by design. Given how pervasive Internet is in today's society, I believe that a free and ethical Internet is synonym with a free and ethical society. Thus, I am committed to help building an Internet that respects our fundamental rights to privacy and freedom.

Decentralized and peer-to-peer (P2P) systems have demonstrated their potential as the underlying paradigm for building online systems that respect it users' privacy [@tor]. Recent episodes such as the Snowden leaks have clearly reaffirmed the urgency to replace, complement or fix current online systems with respect to protecting users against private data and metadata leaks, pervasive online surveillance and also online censorship. While decentralized and P2P systems may be part of the solution, it has been discussed and demonstrated that naive implementation of decentralized systems may harm privacy more than centralized systems [@systematizingdweb], [@crawlingdht], [@pcdn]. I am highly motivated to investigate how current decentralized systems may harm user privacy and to design and develop privacy enhancing mechanisms to address those problems. Moreover, I am interested in designing and developing privacy preserving and decentralized alternatives to current systems deployed at large scale, such as communication systems, authentication infrastructure, search engines and service discovery. 

As P2P networks and decentralized systems (re)gain popularity among researchers and industry alike, I believe that it is important to design and implement decentralized systems that not only preserve users' privacy but also deliver on scalability, performance and usability. Failing to deliver on those properties will render decentralized systems unusable and unattractive for mass adoption or as a viable alternative to centralized systems.

The short term goals of my research are to study, design and help to implement privacy enhancing mechanisms and protocols for decentralized systems. The focus would be on studying and implementing privacy in the building blocks of P2P systems, while considering their security, scalability, performance and usability. From this starting point, I would expect the research to cover topics such as distributed systems, applied advanced cryptography (e.g. zero knowledge proofs, multi-party computation, threshold crypto, homomorphic encryption) and incentive design for agent collaboration in P2P networks.

## Initial research directions 

This section outlines ideas and initial thoughts for research directions. Note that there may be overlapping between topics.

**Privacy preserving and censorship resistant search engines**: Search engines have been (literally) the engine of the Internet and are the backbone of online services. Due to their importance, there has been interest in designing privacy preserving and censorship resistant web search engines [@dwebsearch] and to study current implementations regarding their security and privacy [@censorshipresistantdwebsearch]. There are, though, many challenges ahead to fulfill the vision of decentralized, private and censorship resistant search engines. Open challenges remain in terms of storage and communication constraints [@feasibilitydwebsearch], indexing and ranking mechanisms that suit the decentralized context and scalability [@censorshipresistantdwebsearch].

This research topic would consist of 1) investigating the challenges of indexing, discovering and distributing content in decentralized networks; 2) study and design mechanisms for privacy preserving and censorship resistant search engines; 3) build primitives for indexing and querying data in a decentralized system at scale. I expect this topic to require research on anonymous computation techniques (e.g. homomorphic computation), privacy preserving content discovery and routing, anonymous communication systems and incentive design in P2P networks.

**Practical privacy preserving DHTs**: [@octopus], [@shadowwalker], studied protocols and mechanisms to achieve secure and anonymous low latency communication systems. Many other research studies focus on the the same topic [@routingsurvey]. However, real-world implementation of DHTs such as, for example, IPFS [@ipfs] and Hyperswarm do not seem to adopt any of the privacy preserving mechanism studied in recent literature. My hypotheses are the following: 1) the penalty to paid for the added complexity and protocol performance is large; 2) current secure and private protocols assume centralized infrastructure (e.g PKI infrastructure); 3) there is no incentive and trust models to make sure peers collaborate to enhance the network privacy. I propose to study and measure privacy of deployed systems using DHTs. Based on the results and previous research, investigate novel privacy enhancing mechanisms, protocols and primitives that could improve privacy of DHTs, taking into consideration scalability, performance and security. 

**From centralized to privacy preserving decentralized systems**: Decentralized networks are becoming sound alternatives to centralized systems due to advances in P2P and incentive protocols, the constant increase of computation power and storage in edge devices and recent public cases disclosing how current systems are harming user privacy and security. Ledgers [@bitcoin], contracts [@ethereum] file systems [@ipfs], file sharing [@bittorrent], in-band PGP key distribution [@claimchain] are examples of decentralized systems which aim to replace analogous centralized services. However, as [@systematizingdweb] shows, while decentralization can potentially improve privacy, integrity and availability, naive implementations may be counterproductive in regards to those properties. ClaimChain [@claimchain] is a sound example of how to replace centralized and brittle infrastructure and processes with advanced cryptographic primitives, while adding interesting security and privacy properties which can be used in a decentralized context.

This research topic would focus on answering the question of "which centralized infrastructure can be replaced by privacy preserving decentralized systems and how?". PKI infrastructure, search engines [@dwebsearch], DNS infrastructure are examples of infrastructure that have the potential for improvement in terms of privacy, availability and censorship resistance with a decentralized design.

**Systematization and privacy vulnerability research**: It has been shown how lack of systematization and how to define and measure privacy in decentralized systems make it hard to design and implement such systems [@systematizingdweb]. Research work analyzing privacy vulnerabilities in decentralized systems are vital and wide spread [@pcdn], [@torattack], [@routingdark].

Similarly, I propose to investigate how data and metadata are leaked in decentralized systems. The main goals are 1) define a framework to study privacy in decentralized networks 2) to investigate and enumerate privacy vulnerabilities in current systems; 3) design and implement protocols and/or primitives to address the privacy vulnerabilities found. 
 
**Incentives in privacy preserving decentralized systems**: Cryptocurrencies and smart contracts have - at least theoretically - shown the potential of game theory and incentive design for aligning interests of participants in P2P networks [@incentives], [@incentives2], [@incentives3], [@bitcoin]. Instead of focusing exclusively on incentives in decentralized networks as research topic, I believe it to be transversal to all the research directions mentioned previously.

**Open research topics**: I am open to relevant topics focusing on privacy preserving networks, privacy enhancing technologies (PETs) and applied cryptography in the context of PETs.

---

## References