---
layout: post
title: Wearables - the Last Year's Hype
---

More and more devices, claiming to make us fitter, stronger, and healthier were flooding the marked over the last couple of years. While those devices started out as mere ‘smart’ pedometers to count our steps during the day and magically transferring the collected data to the cloud for users to view in online dashboards or on their phone. Over the years, additional sensors and metrics, such as sleep quality, heart rate, VOmax or even stress have been added to those smart gadgets. But the question remains: How smart, accurate and suitable are those wearables really? 

We were especially interested in the claim that those wristwatches can measure and track stress. The newest generation of devices from Garmin  promise to keep track of users stress levels. A lot of stuff happens within our body when we get stressed: Our heart beats faster, muscles tension increases, our skin gets sweaty to cool down our body, and respectively our surface temperature drops due to the blood flow being diverted to the centre of our body. All those things can be measured with unobtrusive sensors, such as heart rate monitors, skin conductance sensors and skin surface thermometers. Consumer wearables already contain those sensors. But are they sensitive enough to detect subtle changes in the case of stress? Let’s find out. 

We conducted a study [1] where we equipped participants with 3 consumer wearables and a professional laboratory device whilst they were performing some relaxing and stressful tasks (solving mental arithmetic tasks). To induce more real-world conditions, where people are moving around, we did this two times: once while participants were sitting still and once while walking on a treadmill. For the devices, we chose two fitness wristbands/smartwatches: the Microsoft Band and Apple Watch. We also tested the Polar H7, which is a chest strap to detect heart beats and send the data to the phone. 

What we found first of all (and not a very new finding): Wearables get more unreliable in measuring heart rate when people are moving opposed to sitting still. While people were sitting, the mean error percentage compared to the laboratory device was between 3 to 5%. Walking on a treadmill increased this error to 10 to 19%. Especially the wrist devices were prone to a higher error rate. Those wrist devices use an optical sensor to detect heart beats; they emit a green light and optically pick up the blood flow under the skin. Most fitness trackers rely on this technology, but it has its faults (like the scandal about the first gen Apple watches which had problems with heart rate readings on darker or tattooed skin [1] or the fact that it gets more unreliable under movement or when wristbands are worn to tight). The more reliable and older approach is to use electrical signals to detect the heart beats directly at the chest, like the Polar H7 does - but of course that is less convenient for a device which is worn all day.

Further, we found that the expensive reference device was the only device to show that it picked up the stress responses (increased heart rate, increased skin sweatiness and decrease in skin temperature) during our stress task in a statistically valid manner - and just while participants were seated. We could not find any statistical effects for any of the devices for when people were walking on the treadmill (due to all of the sensors, even the reference device, becoming more unreliable). 

What do we learn from this: While those nifty smartwatches and fitness trackers are convenient and comfortable, their data has to be taken with a grain of salt and the sensors are just very prone to movement and various factors. Especially such claims that a fitness tracker can tell you when you are stressed, should be further investigated and evaluated. 

 

[1] Katrin Hänsel, Romina Kettner, Hamed Haddadi, Akram Alomainy, Albrecht Schmidt,  "What to Put on the User: Sensing Technologies for Studies and Physiology Aware Systems", Proceedings of the ACM Conference on Human Factors in Computing Systems ([ACM CHI'18](https://chi2018.acm.org)), Montréal, Canada, April 21-26, 2018. ([paper](https://haddadi.github.io/papers/CHI2018sensing.pdf){:target="_blank"})

[2] [People with tattoos report the Apple Watch is having trouble determining they are alive — Quartz](https://qz.com/394694/people-with-dark-skin-and-tattoos-report-the-apple-watch-is-having-trouble-determining-they-are-alive/)



| <img src="https://github.com/haddadi/haddadi.github.io/blob/master/images/2018/Wearables.png?raw=true"  height="300" width="400"> |
|:---:|
| Illustrative schematic of the design space evaluation for our 4 test devices (Nexus, Polar, Apple Watch, Microsoft Band) in 5 criteria dimensions (data reliability, comfort of attachment, mobility, data richness, and data accessibility) |



