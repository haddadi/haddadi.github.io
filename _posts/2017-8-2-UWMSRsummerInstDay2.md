---
layout: post
title: UW Allen School MSR Summer Institute 2017 (Day 2)
---

# Schedule and slides available on: 
[https://www.cs.washington.edu/mssi/2017/schedule.html](https://www.cs.washington.edu/mssi/2017/schedule.html)



## Session 4: Privacy & Security

### Lynette Millett, National Academy of Sciences: [Avoiding Predictable but Alarming Trajectories](https://www.cs.washington.edu/mssi/2017/abstracts.html#milletttalk)
Lynette has had nearly 20 years of experience in the technology policy scene in Washington. She expanded on political and technical definitions of privacy and security in different domains and the importance of making the IoT systems safe and secure, considering the existing shortcomings on the Internet. Historical perspectives from earlier reports were presented during the talk on lessons learnt from major failures in critical systems and scalability of the IoT will put major challenges ahead in this area. Maintenance and overseeing of the deployments of these long-lived systems “out there” will be important. 

### Josh Siegel, MIT: [Context and Cognition for a Secure and Efficient IoT](https://www.cs.washington.edu/mssi/2017/abstracts.html#siegeltalk)
Josh touched upon data ownership, policy issues and technical issues around IoT systems. Standardised interfaces and familiar architectures (IP, AC electricity, etc) are not yet prevalent in IoT. A common, “human-inspired” architecture is needed to isolate the access to data, from access to actual devices, based on consent, requirements, granularity, etc. A “cognitive firewall” idea has been developed for mirroring the behaviour of these systems in the cloud to address fragmentation, openness, data ownership, security, and resource management. Using the same models behind the cognitive firewall, sampling rates (and consequently bandwidth and energy) may be optimized while complying with application requirements. Additionally, data flow visualisations have been successful in improving user trust, e.g., in the vehicular systems area for vehicle health and safety monitoring. 

### Dave Thaler, Microsoft: [Trusted Cyber-Physical Systems](https://www.cs.washington.edu/mssi/2017/abstracts.html#thalertalk)
Dave discussed the economics of security in cyber physical systems in large-scale environments (e.g., factories, hospitals, industry space, smart cities). These systems are vulnerable to state actors, malware, rogue internal agents. Strong security promises are needed for making systems tamper-proof, auditable and accountable, encryption-friendly. Trusted Execution Environments (TEEs like SGX, TrustZone, TPM, etc). Physical security and cryptographic security come hand to hand in the presented framework for trust model presented in TEE from a sensor to data to an actuator or a piece of code. These systems ensure unique identifier per device, authorised code execution, hardware access, and access to trusted peripherals. Trusting the code is still a tough challenge. Though we already know how to solve it, we need it to actually happen! 

### Philip Levis, Stanford: [Safely and Efficiently Programming a 64kB Computer](https://www.cs.washington.edu/mssi/2017/abstracts.html#levistalk)
Phil focuses on securing the IoT, especially from the point of view of the Operating System. He presented Tock, an operating system whose kernel is written in a typesafe language (Rust) for auditability and safety. Capsules are included in the kernel, written in Rust, and use Rust for isolation/safety. Userland processes can be written in any language and use hardware protection for isolation/safety. The kernel dynamically allocates from processes to ensure that a process can’t exhaust the kernel heap and language mechanisms ensure references to these allocations don’t escape into the rest of the kernel. This allows programmability of edge devices (e.g., a smartwatch!) in a language of choice. Authentication of devices remains a challenge here as the app-to-app authentication in an untrusted zone remains a challenge. See more on [www.tockos.org](http://www.tockos.org)

### Ben Zorn, Microsoft: [Building an Internet of Things we can Trust](https://www.cs.washington.edu/mssi/2017/abstracts.html#zorntalk)
Ben manages the research in software engineering in MS. He discussed how the security and privacy risks of many software and hardware platforms, even those by major brands and companies, might be hidden in million lines of codes.He discussed [deepspec.org](https://deepspec.org/) project for software verification and the [Everest project](https://project-everest.github.io/) on secure software development, aiming to replace untrusted codes in services with verified trusted code. This has been evaluated on protocols such as TLS, open SSL, etc. However in the next phase in future, Ben highlighted the importance of verifying ML/AI models, mathematical reasoning about the models, and understanding data quality and its effects. We need to address human understanding, adversaries, and failsafe operation. Perhaps we could have annual software/IoT vulnerability check ups?


## Roundtable Presentations #2

### Peter Bodik, Microsoft Research
Deploying even relatively simple IoT applications is complex in current IoT frameworks; it requires stitching together containers running on the edge, through a communication pipeline to the cloud and through several cloud services. This introduces challenges in deployment, monitoring, estimating cost, and so on. Further, there are many different optimization that customers have to implement manually. This requires providing a declarative way to specifying the IoT applications and automatically optimizing and deploying them.

### Prabal Dutta, Berkeley: [Signpost: Sensors for Urban Monitoring](https://www.cs.washington.edu/mssi/2017/abstracts.html#duttatalk)
Prabal focused on urban sensing from pedestrians, sounds, etc in the city. Deployments face challenges in infrastructure and maintenance. Energy adaptivity, ease of installation, HCI, and storage/processing are important factors to consider in such deployments. Many of these problems re-emerge in different settings considering the rise of new hardware and applications.

### Dan Lieberman, Pioneer Square Labs: [Taking Enterprise IoT from Prototype to Production](https://www.cs.washington.edu/mssi/2017/abstracts.html#liebermantalk)
Dan discussed the issues and challenges in moving from proof of concept to prototypes to commercial systems. He discussed the software design process and the path to development of devices from the idea to manufacturing. 

### Chenyang Lu, Washington University: [Dependable Internet of Things](https://www.cs.washington.edu/mssi/2017/abstracts.html#lutalk)
End-to-end latency from the sensor to the edge to the cloud to an actuator is an important challenge to address in the IoT space. Use of Edge-cloud processing in virtual machines can help in addressing the demands of real time applications and event processing. The work in [RT-Xen project](https://sites.google.com/site/realtimexen/) developed demonstrates great performance improvement. 

### Steve Myers, Indiana University: [Long-lived cryptography for long-lived devices and secure updating in the IoT](https://www.cs.washington.edu/mssi/2017/abstracts.html#myerstalk)
Steve brought up the issue of long-lived smart devices entering the home and the privacy-security challenges introduced in this space. Data encryption is of importance here, hence these deployments need to be done with the next decade in mind. Advances in faster computing methods such as quantum computing makes this an imminent issues to deal with. 

### Thomas Pfenning, Microsoft
Thomas presented the [Windows IoT Core platform](https://developer.microsoft.com/en-us/windows/iot), in mobile and other enterprise devices. The platform aims to get secure systems, with capability of cloud connected solutions. The platform aims to offer scalable device management from the cloud for updates and settings. Intelligence at the edge was highlighted as an area of importance, security of gateway devices, and device capabilities giving rise to local processing capabilities which can be utilised using the platform. 

### Matt Reynolds, University of Washington: [Millimeter Wave Imaging and Long-Range Wireless Power](https://www.cs.washington.edu/mssi/2017/abstracts.html#reynoldstalk)
Battery takes up 50% of the volume and wireless hardware takes over 40% of board area in a smartphone. Hence architectural innovations are needed to improve the status-quo. IoT devices will extend to living things (people, animals) - not just non-living sensors. Using backscatter comms and wireless power systems, Matt’s group has designed a neural data telemetry system to downlink dragonfly brain activity in real time. Matt also presented their sensing efforts on security domains using millimeter wave MIMO for imaging. 

### Stefan Thom, Microsoft: [How to fight an adversary that is not bound by the linearity of time?](https://www.cs.washington.edu/mssi/2017/abstracts.html#thalertalk)
Updating devices and their maintenance in-person after firmware issues and leaks is a costly operation. The physical limitations of these systems make it difficult to do malware analytics or software checking easily or do policy verifications by the human operator. Missing the context and device state makes the application analytics challenging for event analytics. Hence a focus on bootloader and boot time code analysis per device was highlighted as a way of establishing identity and issuing certificates for devices. RIoT from MS brings more information on this.

## Invited Talk 
### Chris Diorio, CEO, Vice Chairman, and Founder at [Impinj](https://www.impinj.com/): [The Littlest Biggest Internet Opportunity](https://www.cs.washington.edu/mssi/2017/abstracts.html#dioriotalk)

Abstract: We are fast approaching a day when trillions of everyday items are connected to the Internet. This connectivity presents both challenges and opportunities for the IoT. In this talk I will review RAIN RFID's significant role in connecting everyday items and will then propose a framework for addressing those IoT challenges and opportunities.

Chris talked about motivations for connecting items, future visions, and opportunities and challenges. How would we go about connecting trillions of items in the near future? History, ownership and services will be recorded. RAIN RFID allows unique, small radio-identified battery-less tags. [RAIN RFID](http://rainrfid.org/) alliance has secured spectrum in many countries and is used by many industries. Each tag might be read 10s or 100s of times. The value is putting the data, context and analytics together. Billions of these tags are already used in industries, in consumer sectors like Delta bag tags (a $50m investment) and tracking marathon runners. 

Perhaps in the near future, these RAIN tags can be integrated into suitcases and with a phone app and airline registration, to enable a smoother check in and collection process. Though currently the lack of an IoT backend is is slowing the deployment of RAIN readers in phones.

Chris concluded by proposing some principles: items’ digital lives should mirror their physical lives, and their history, ownership and services must be kept in a journal. Services and history are atomic; ownership is chained. Applications’ access journals subject to persistent owner rights.  Items will have digital twins in the cloud for journal keeping and data storage. Connecting items should hopefully improve all our lives!


## Session 5: Experiencing the IoT
Speakers:
### James Landay, Stanford: [Out of body User Experience](https://www.cs.washington.edu/mssi/2017/abstracts.html#landaytalk)
James presented his group’s experience on visions in interaction with AR and drones. These could include personalised tours and navigation. They observed a cultural dependency on gestures and interactions with drones. They are discovering natural interaction patterns for how people will interact intuitively with objects and public drones one day!

### Rajalakshmi Nandakumar, UW Allen School: [Interacting with small devices using active sonar](https://www.cs.washington.edu/mssi/2017/abstracts.html#nandamumartalk)
Interaction with IoT devices is a challenge! [FingerIO](http://fingerio.cs.washington.edu/) is a motion-based finger tracking software for using speaker and microphone on the device to understand motions based on reflections to enable any surface as an input surface with high accuracy.

### Joe Paradiso, MIT Media Lab: [Siri/Cortanai/Alexa vs. the Other Me -- Pre-Cognitive Human Extension as the Future of IoT](https://www.cs.washington.edu/mssi/2017/abstracts.html#paradisotalk)
Joe presented the CHAIN-API, an early version of JSON-based open standards for sensor connectivity and data posting. As smart environments will become an extension of self and understand more context, naturally tunneling this information into perception becomes challenging. Joe demoed DoppelLab live visualizing different sensors which are in the Media Lab building with scrambled audio and social media. The demo highlighted the need for a unified control panel for sensor aggregation and bringing data together from different sources. Joe also demonstrated the [Tidmarsh living observatory](https://tidmarsh.media.mit.edu) as a live environmental monitoring platform. The audio enables real time classification of different animals at the site. The aim is to understand the Human-Data Interaction and manifestation of data from sensors and the individuals in the environment. He also showed examples of a room that transformed via lighting and projected imagery as a function of a user’s context and affective state.

### Gregory Abowd, Georgia Tech: Extreme Ubiquity: [De-emphasizing the importance of Moore's Law](https://www.cs.washington.edu/mssi/2017/abstracts.html#abowdtalk
Moore’s law is no longer applicable in today as the transistor packing space is saturating. However we can now move on to moving from silicon-based ICs to embedded sensors manufactured items, and computational material which can harvest information and compute, store data, and actuate. The aim of the [COSMOS project](http://ubicomp.cc.gatech.edu/research/) is to reach there soon!

## Invited Talk
### Ron Zahavi, Microsoft: [IoT Success Factors & Business Models](https://www.cs.washington.edu/mssi/2017/abstracts.html#zahavitalk)
Abstract: In this session I will describe how IoT combines elements of existing and new capabilities into systems of systems that can be highly complex, involving many new business models. I will then review issues and pitfalls to avoid, different business models, and the elements existing organizations ongoing transformation, as well as startups, need to succeed in the new IoT connected world.
![Ron Zahavi](/images/2017/IMG_3737.JPG)
