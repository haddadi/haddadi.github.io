---
layout: post
title: Workshop on Decentralized Machine Learning, Optimization and Privacy (Sep 11-12, 2017)
---

# Schedule and slides available on: 
[https://team.inria.fr/magnet/workshop-on-decentralized-machine-learning-optimization-and-privacy/](https://team.inria.fr/magnet/workshop-on-decentralized-machine-learning-optimization-and-privacy/)


I attended the INRIA Lille Magnet (MAchine learninG in information NETworks) Workshop on Decentralized Machine Learning, Optimization and Privacy. Here's a brief summary of some of the amazing talks on machine learning, edge processign, and privacy-preserving analytics.  


## Talk session (chair: Sébastien Gambs)

*   Stephen Hardy: Learning nothing but the model [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_hardy.txt&sa=D&ust=1505233712595000&usg=AFQjCNEdocsc6s2dTJI_pDAb6Htjx5AzoQ)]

Stephen talked about the problem of joint analysis of data across multiple organisations. They have done trials with organisations on this problem, for applications such as data sharing for organisations,  cross-governance-boundary analytics, PDM, and analytics across device data. Their solutions include [partial] homomorphic encryption, graph computation engine, and private entity resolutions. PER works by sharing secret salt from a hashing process.

The examples include credit scoring for example, hence sensitive data across organisations on-premises or in cloud, has to be analysed independently for predictions around credit failing. Hundreds of features can be included from the two organisations to run joint logistic regression (simple to do and explainable). However the process still reveals whether the same entity exists on both datasets hence it requires consent. Private learning is about 500x slower on encrypted data, however a score can be generated in real time.Customer feedback indicates a strong emphasis on learning the model rather than finding common users. In order to deal with this, they have created an encrypted mask in the reordering and matching stage at the broker to break the linkage possibility. They use Taylor approximation to logistic loss in order to reduce feature space size and regularise them. Some implementation code available on: <[https://github.com/n1analytics](https://www.google.com/url?q=https://github.com/n1analytics&sa=D&ust=1505233712595000&usg=AFQjCNG4vrAOIFL3tUqxAo-osaeU9IZYNQ) 



*   Borja Balle: Secure Multi-Party Linear Regression on High-Dimensional Data [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_balle.txt&sa=D&ust=1505233712596000&usg=AFQjCNGrWfa10sJguiy88PKn5AVQ_C-MXg)]

Borja presented a similar problem set, working with multi-party differential privacy to address the trusted third party challenge of access to training data. Some of the challenges have been framed as an optimization problem. The optimisation has been implemented as a multi-party Ridge regression. Borja presented the challenges in this space (MPC protocol, scalability, privacy guarantees, etc). This can be addressed by using separate crypto providers, data providers, computing providers, and data providers. Hence differential privacy can be done at the output to help with scalability. The PETS paper and the open source implementation are available online.


##  Poster spotlights [[poster list](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/09/posters.txt&sa=D&ust=1505233712596000&usg=AFQjCNGxvP6SkLHe_PbXZ8nTk1QIltALxg)]


##  Talk session (chair: Joseph Salmon)

*   Mikael Johansson: Sparsity and asynchrony in distributed optimization: models and convergence results [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_johansson.txt&sa=D&ust=1505233712597000&usg=AFQjCNGhP0cVF541XKfyXD2jx-lYZqmnRg)]

Mikael covered optimization for large-scale learning and issues such as centralised versus distributed, or asynchronous versus synchronous.

*   Peter Richtárik: Privacy preserving randomized gossip algorithms [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/09/talk_richtarik.txt&sa=D&ust=1505233712598000&usg=AFQjCNFHnPd8lfdpNiOEdmSUMoOtXK9CkA)]



##  Talk session (chair: Morten Dahl)

*   Meilof Veeningen: Distributed Privacy-Preserving Data Mining in the Medical Domain[<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_veeningen.txt&sa=D&ust=1505233712598000&usg=AFQjCNEb32Q8vD5xYVz4Xjdf8EVzCxgVOg)]

Meilof discussed the IoT and medical devices that Philips develops and their interest in data science. Decentralised ML is important for building personalised models where privacy and accuracy are both critical. Experiments are often useful for understanding workflows and hospital patient movement. Using MPC it is possible to perform privacy-preserving tracking and analytics. Examples can include multi-hospital analytics of patient data using differential privacy. PErformance and acceptance by all parties remains a challenge.



##  Talk session (chair: Aurélien Bellet)

*   Keith Bonawitz: Federated Learning: Privacy-Preserving Collaborative Machine Learning without Centralized Training Data [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_bonawitz.txt&sa=D&ust=1505233712599000&usg=AFQjCNGwZfvJTgkENpHqPDbXGhCBs3DNyg)]

Keith presented the Google Federated learning approach for learning on the device. The sensitive data stored on the phone makes the personalised training a unique challenge to build a central model to be equivalent to all the individually trained models. This can be useful for multitask learning, and learning to learn. He presented a number of papers in topics such as federated learning or distributed mean estimation with limited communications (ICML 2017). Secure aggregation (using SMPC) is an important aspect here in moving away from keeping large datasets to ephemeral data from focused trained models. Using pairwise Diffie-Hellman key agreements they enable secret model sharing across users. Hence updates can be aggregated while not being inspected. Differential privacy can be useful here for aggregating results from queries across multiple databases.

*   Dan Alistarh: Quantized Stochastic Gradient Descent [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_alistarh.txt&sa=D&ust=1505233712600000&usg=AFQjCNHge2D93siiuh_jcCJw7ewe-xdZWQ)]

Dan presented the computational challenges in large-scale model training.



##  Talk session (chair: George Giakkoupis)

*   Hamed Haddadi: Containing Personal Data Processing with the Databox [<[abstract](https://www.google.com/url?q=https://team.inria.fr/magnet/files/2017/08/talk_haddadi.txt&sa=D&ust=1505233712601000&usg=AFQjCNG25Fohoqz2l5Tf22WJTGW7PHTT4A)]

I presented the Databox Project. 

