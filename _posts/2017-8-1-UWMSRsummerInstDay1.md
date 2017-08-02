---
layout: post
title: UW Allen School MSR Summer Institute 2017 (Day 1)
---

# Schedule and slides available on: 
[https://www.cs.washington.edu/mssi/2017/schedule.html](https://www.cs.washington.edu/mssi/2017/schedule.html)

## Introductions Victor Bahl (MSR) & Shyam Gollakota (UW)
![Introductions](/images/2017/IMG_3710.JPG)

IoT as in interdisciplinary topic, hence a range of skills and expertise involved in this summer institute. Important to get interaction across disciplines. The industry is on a race to deployment, and academia is working on visionary projects. It is important to get conversation going between the two. 

There are infrastructure questions: AI, Intelligent Edge, IoT, etc. While academia has been discussing this for a while, a push from huge industry partners will drive this forward, while privacy & security are of importance here. This Institute aims to drive collaborations, joint projects and publications, while highlighting the risks and challenges. 

![Introductions](/images/2017/IMG_9801.JPG)

## Keynote: Affan Dar, Principal Group Software Engineering Manager, Azure IoT Platform, Microsoft
[Simplifying IoT with Cloud and Edge](https://www.cs.washington.edu/mssi/2017/abstracts.html#dartalk)

![Affan Dar](/images/2017/IMG_9807.JPG)

IoT is not a technology evolution, rather a business revolution enabled by technology. Real customers have interests in this space for cost saving, maintenance, analytics, and fault-finding. However currently there is high barrier to entry due to diverse ecosystem of devices, OSes, capabilities, protocols, standards. No winner in the space yet. The cloud and device app models are completely different hence scalability and customisation is challenging. 

[Azure IoT platform](https://azure.microsoft.com/en-us/services/iot-hub/) aims to address some of these challenges, supporting easy-to-build building blocks and supporting a range of protocols and frameworks, including an Edge SDK for local decision making and processing. Though it is difficult to maintain cohesive security,  as devices can be deployed in untrusted environments. However having integrated platforms can help with securing applications, and hardware/software attestations and trust. 

Edge computing was highlighted: constrained network resources, high latencies, unreliable networks. Understanding disconnectivity in operational state is an important challenge for a self-sustaining system. We need to go away from mission-criticality. Audience engaged heavily in discussions of the cloud versus edge processing and compromises to be made there. Container-based management and workload control nd local storage are being explored. Scalability in number of devices, throughput and burst scenarios is another challenge faced in this space.

## Session 1: The Intelligent Edge

### Evan Welbourne, Amazon: [Learning at the Edge](https://www.cs.washington.edu/mssi/2017/abstracts.html#welbournetalk)
Presented a case for running machine learning models at the Edge of the network with an example from prior work at Samsung Research.  Also presented key challenges and brainstorming topics for learning new models at the Edge: decentralized learning algorithms, diverse device resource constraints, device-cloud security, soliciting feedback or labels from end users, and peer-to-peer device coordination to learn at the Edge. Closed with a note on hiring for Machine Learning at Amazon Alexa Smart Home.

### Anind Dey, Carnegie Mellon University: [GIoTTO: An Open-Source IoT Framework](https://www.cs.washington.edu/mssi/2017/abstracts.html#deytalk)
CMU GIoTTO aims to enable an IoT ecology for enabling security & privacy, end-user programmability, machine learning, and large-scale deployability. The goal is to improve HCI and human interaction in user-driven queries, while supporting privacy with role-based ACL. Anind demoed a number of ubiquitous applications of the platform for training and performing inferences. See more on [https://iotexpedition.org](https://iotexpedition.org)

### Artur Laksberg, Microsoft: [Programming IoT Edge Devices: Cloud-Client Duality](https://www.cs.washington.edu/mssi/2017/abstracts.html#laksbergtalk)
Cloud latency, privacy, reliable connectivity, and security are important challenges in IoT for legal requirements, transmission costs, and user experience. Hence there is clear need for local processing and connectivity. Today’s workloads are based on data filtering and aggregation, but tomorrow this could be ML, computer vision, and security. More hardware manufacturers will support new features to enable this. Edge devices minimise transit latencies for many analysis types. AWS greengrass and Azure IoT edge are examples in this space. These challenges, in addition to the power requirements and performance overhead imposed by message-based APIs (container, API, crypto, etc) make the cloud-based approaches less appealing for critical applications. Will the two approaches (edge & cloud) be in contrast, or do we have to maintain both platforms for consumers, developers, and applications?

### Suman Banerjee, University of Wisconsin: [Intelligent Edge for Education](https://www.cs.washington.edu/mssi/2017/abstracts.html#banerjeetalk)
![Suman Banerjee](/images/2017/IMG_3721.JPG)

Suman presented challenges in education and teaching resources, and how the teaching labs can be maintained by using a cloud-hosted platform to democratise software access. This browser-based system allows VM access over VPNs for software access.The platform can use any cloud offering, but currently is mostly hosted bat Microsoft Azure. This introduces new challenges as software systems use in scalability grow in needs of interactivity, complexity, and various types of dependencies. Various optimizations are possible that allow reduced costs for academic institutions.

## Session 2: Prototyping & Connecting the Next Billion Devices

### Steve Hodges, Microsoft Research: [Building connected devices](https://www.cs.washington.edu/mssi/2017/abstracts.html#hodgestalk)
Steve presented the early work in [his group](https://www.microsoft.com/en-us/research/group/sensors-and-devices/) on the [.NET Gadgeteer](https://en.wikipedia.org/wiki/.NET_Gadgeteer) prototyping platform, which brought together three key elements: modular pluggable hardware, modern programming metaphors and tools, and support for custom form factors. The talk presented the aims and challenges of developing this platform and an unanticipated success for the technology as a tool for teaching computer science in schools. This experience, coupled with other work showing that the tactile, tangible nature of physical computing engages students, shaped the direction of the [BBC Micro:bit](https://makecode.microbit.org/) which Steve briefly demoed. Finally, Steve mentioned [a new prototyping platform](https://microsoft.github.io/azure-iot-developer-kit/) which extends the Micro:bit with additional sensing, a bitmapped display, and WiFi connectivity with the aim of empowering web developers to explore programming for embedded connected devices. 

### Vamsi Talla, Jeeva Wireless: [Enabling cheap and reliable connectivity for the next billion devices](https://www.cs.washington.edu/mssi/2017/abstracts.html#tallatalk)
[Jeeva Wireless](https://www.jeevawireless.com/) is reimaging connectivity by reducing the cost, size and power consumption of wireless communication. The key challenge with current radios is that the analog RF front end and RF signal generation consumes tremendous amount of power. Jeeva’s solution presented by Vamsi relies on using only digital and backscatter communication to synthesize WiFi (or ZigBee/BLE) or LoRA packets by reflecting a carrier signal using tiny small devices and these packets can be received on any standards compliant receiver. This greatly reduces the complexity of the solutions and results in orders of magnitude reduction in power consumption. 
This approach can bring connectivity between passive backscatter devices (e.g., contact lenses or credit cards) and smartphones/tablets/routers. The use of long-range backscatter technique gives a coverage of 100s of metres allowing a number of devices to get connected with at a low data rate using backscatter method.

### Vikram Iyer, University of Washington: [3D Printing Internet Connected Objects](https://www.cs.washington.edu/mssi/2017/abstracts.html#iyertalk)
Today 3D printed objects are separate from connectivity modules (e.g., WiFi chips). It would be ideal to 3D-print IoT/connected devices using mechanical motion to reflect WiFi waves to encode a message. This requires printing an antenna (e.g., small dipole antenna printed using a composite copper-plastic material. On-off or encoding switches are also printed using an ordinary 3D printer. Power can be gained using energy-harvesting methods (e.g., an anemometer) or interaction-based devices.

### Alanson Sample, Disney Research: [Rethinking the RF physical layer to enable the next generation of IoT sensors](https://www.cs.washington.edu/mssi/2017/abstracts.html#sampletalk)
UHF RFID tags offer a means of minimally instrumenting “dumb” objects and bring them into the virtual world. By monitoring changes in the communication channel parameters between the RFID reader and tags and using machine learning techniques it is possible detect users object interaction event which can enabling activity inferencing applications in the home and workplace. To solve the battery charging problem, room scale wireless power using quasi-static cavity resonance can seemly deliver large amounts of safe wireless power anywhere in room. Lastly, energy harvesting sensor nodes using ultra-wideband ambient backscatter techniques reduce power consumption by backscattering ambient radio broadcasts source such as FM, TV and Cellular broadcasts to a universal backscatter reader.

### Saman Naderiparizi, University of Washington: [Battery-free Cameras and Low-power Machine Vision for IoT](https://www.cs.washington.edu/mssi/2017/abstracts.html#samantalk)
Wireless cameras are increasingly present in the environmental monitoring scene. Going battery-free can reduce the maintenance complexity here. The main idea here is how to bring the power consumption of, traditionally known to be power-hungry, wireless streaming cameras to a level (sub-mW) that energy harvesting from ambient sources, such as WiFi or RFID readers, can enable fully battery-free streaming cameras. Analog backscatter communication is used here to stream the video data from the camera and allows for eliminating the need for power hungry components such as ADC and amplifiers. The experiment showed that traditional face detection algorithms can be applied to the received videos and result in a high-accuracy of face detection at up to 100ft away from the access point.

### Joshua Smith, University of Washington: [Battery-free Cellphone](https://www.cs.washington.edu/mssi/2017/abstracts.html#smithtalk)
Exponential improvements in the energy efficiency of microelectronics is helping enable battery-free sensing/computing systems. Josh presented a battery-free cell phone that transmits voice signals using analog backscatter, transmits dialing information using digital backscatter, and receives voice and call-control data in a passive fashion. These scaling trends and novel sensing/computing systems could lead to much larger numbers of edge-devices, larger quantities of sensor data, improved environmental sustainability (by eliminating batteries), and also reduced maintenance complexity. 
 
## Session 3: Emerging Applications and Use Cases of IoT

### Ranveer Chandra, Microsoft: FarmBeats: [AI and IoT For Data-Driven Farming](https://www.cs.washington.edu/mssi/2017/abstracts.html#chandratalk)
Understanding farm conditions (nutrients, mositure, temperature) level is important for dynamic farming and precision agriculture to optimise use of water, pesticides, etc to improve yield & sustainability. [FarmBeats](https://www.microsoft.com/en-us/research/project/farmbeats-iot-agriculture/) aims to help with this challenge using data-driven sensing platforms. They use TV White Spaces for connectivity, and sensors and drones with ML-based computer vision to monitor the farms. For areas with legal issues around drone-usage, they use balloons for imagery acquisition. Hence sparse sensor data and the image can be mixed up to provide insights to the farmer. Edge processing and offline ML is used for analytics in case of network connectivity issues. 

### Klara Nahrstedt, University of Illinois, Urbana-Champaign: [Exploring IoT Co-dependencies in Electro-Mobility](https://www.cs.washington.edu/mssi/2017/abstracts.html#nahrstedttalk)
Klara presented the dynamic wireless charging for electric cars on highways. The interdependence between the car companies, the energy sector, the road infrastructure, and telcos make this a challenging task. Many sensors are involved in the ecosystem from all these players. The positioning of coils, their efficiency and quality, and load shaping is important for different times of day and different vehicles. Key management, authentication in short time, and location privacy are important. Privacy-preserving billing is an important aspect. 

### Edward Wang, University of Washington: [Changing the way we diagnose health using mobile and IoT technologies](https://www.cs.washington.edu/mssi/2017/abstracts.html#wangtalk)
Healthcare and clinical infrastructure are an obvious area where IoT can make a big impact. Continuous monitoring and sensing can provide us with valuable health data. As an example, edward presented HemaApp which can be used for hemoglobin monitoring.Wearables such as glasses can also be used for blood pressure and heart rate monitoring. This can lead to correlations between other sensors such as activity recognition, or for personalisation of medication. 

### Deepak Ganesan, UMass Amherst: [Towards continuous measurement of cognitive state and addictive behavior in natural environments](https://www.cs.washington.edu/mssi/2017/abstracts.html#ganesantalk)
Addictive behaviour monitoring is considered as an epidemic and is a costly task for the health system. Accuracy in drug usage detection is of importance and the cues, triggers, and individuals’ routines are important for understanding the habits and providing potential interventions. Using smart glasses, eye closure rates can be monitored for fatigue and dopamine level sensing with high accuracy. Wearable ECG can also be used for drug usage detection. Though simple models can be developed in the lab, in-the-field detection from addicted users is difficult. 

## Round Table Presentations #1

### Rahul Bhattacharyya, MIT: [Low-cost, pervasive sensing leveraging existing wireless infrastructure](https://www.cs.washington.edu/mssi/2017/abstracts.html#rahultalk)
Rahul talked about low-cost sensing research. E.g., use of RFID tags with probe interface to traditional paper-based anemia detection can only costs a few $s. Other modalities include use of sensors in vehicular monitoring, for example wheel imbalance.  RFID sensors can be adapted for a bunch of other modalities like crack section, soil moisture sensing and fluid level sensing. Use of time-windowing techniques and PCA techniques form FFT features can lead to highly accurate detection techniques for presence of imbalance. Mobile sensors are pretty useful here. Moving to intelligence to peripheral devices and offboard computation leads to easy deployment.  

### Jean Camp, Indiana University: [Risk Communication as Security Interaction in the IoT](https://www.cs.washington.edu/mssi/2017/abstracts.html#camptalk)
Jean presented the tussle between security & privacy. Communicating privacy and data exchange deals and incentives, usability, and awareness of risk is highly ignored. Novel HCI and interaction methods should be used to enable security and risk communication to the ordinary users. 

### Anat Caspi, UW Allen School: [Independent mobility in the Connected City: IoT-enabled Pedestrian-Centered Mobility for People with Disabilities and Older Adults](https://www.cs.washington.edu/mssi/2017/abstracts.html#caspitalk)
Anat presented IoT for the public good challenge. Sensing in cities and built environments includes interaction between a number of agents and stakeholders. The need for specialised equipment and environment for accessibility in the cities is a challenge for making the cities easy to navigate for those with mobility impairments. Consumption of the sensor data through apps is being developed. Proprietary data formats are an obstacle to gaining access to larger datasets and data collusion. Combination of wearable devices for different users, and mobile apps, can help with more useful feedback to the users. Optimal routes are not necessarily the shortest paths, hence tagging paths and routes with data about condition of the paths, elevation, pollution, etc is being enabled in their effort in this space.

### Aakanksha Chowdhery, Princeton: [Video analytics at scale for mobile Internet-of-things platform](https://www.cs.washington.edu/mssi/2017/abstracts.html#chowdherytalk)
Video cameras are increasingly appearing for surveillance and connected cars and other areas. The local processing versus cloud-based approaches are used in this space, though this depends on the type of analytics which are of interest (summaries, anomalies, highlights, etc). Edge computing can provide more efficient bandwidth provision here. Bandwidth constraint, the energy trade offs, low-latency, and analytics are of interest here. Local processing and adaptive algorithms can help with achieving the right tradeoff.  

### James Fogarty, UW Allen School: [The Data is the Interaction](https://www.cs.washington.edu/mssi/2017/abstracts.html#fogartytalk)
IoT presents new challenges for interaction because of the unprecedented volumes of personal data. As we work to understand new technologies and opportunities, we often copy forward prior designs, with limited success. New designs require reconsidering prior assumptions about benefits, burdens, and control. What is the data, and how does an individual get genuine personal value from that data?

### Hamed Haddadi, Imperial College London: [Containing Personal Data Processing with the Databox](https://www.cs.washington.edu/mssi/2017/abstracts.html#haddahitalk)
Presented the [Databox](https://www.databoxproject.uk/) – open source project; personal data ecosystem; 
Challenges: data security, privacy, scalability, energy – platform for curation of data; open source personal networked system , mediate access to data; apps, data stores, everything is docker container; 
Databox – give temporary access to data; runs analytics; and then kill container, and remove it; 
Databox and apps ecosystem – personalize cooking program (demo); using analytics; data ecology & use; 
Data negotiability; app communicates with user about risks and benefits; 
Discussion – who puts infrastructure for databox (it is setup-box provider) ; there is some regulation on what data we can collect; 



