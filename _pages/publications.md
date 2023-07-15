---
title: "Publications"
permalink: /publications/
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


I have had the opportunity to work on a number of interesting research projects during my Ph.D. My research combines system design, signal processing, computer vision, and machine learning methods to investigate security and privacy threats on emerging computing platforms and then proposes methods for securing modern mobile and IoT devices and protecting users’ privacy. Here is a summary of some of my research efforts.

<!---
My research has shown multiple new privacy leakages resulting from sensor data available on mobile devices, introduced secure and usable authentication mechanisms for mobile users and IoT devices, proposed usable authorization protocols for mobile developers, demonstrated attacks and defenses against IoT anomaly detection systems, and built secure communication system between humans and cameras through mobile devices. Here is a summary of some of my efforts.

--->

## Enabling Usable Authentication on Commodity Mobile and IoT Devices [MobiCom'20, S&P'23]

<!-- <p style="text-align: justify"> -->
<b>I developed two systems, <a href='/files/FaceRevelio.pdf'>FaceRevelio</a> and IoTCupid to enable reliable and secure user and device authentication to protect users’ private information (e.g., contacts, messages, credit card details) on commodity mobile and allow secure communication between IoT devices.</b>

 <a href='/files/FaceRevelio.pdf'>FaceRevelio</a> is a novel liveness detection system that protects facial authentication mechanisms on commodity smartphones from spoofing attacks, without requiring effort from the users or any external hardware. It leverages the smartphone screen as a light source and illuminates different portions of the screen with random lighting patterns for a short duration (∼1 second) to simulate multiple lighting conditions. The reflection of the light from the screen is recorded and then used to extract stereo images of the face and its 3D surface through a photometric stereo technique. The reconstructed 3D surface differentiates a real human face from its 2D counterpart and defends against spoofing attacks. This work was presented at MobiCom 2020.
<!-- </p> -->
 
 <p align="center">
 <a href='https://youtu.be/zGlbclBXQ8Y'><img src="/files/facerevelio_teaser.png"
     alt="FaceRevelio - Teaser Video"
     style="display:block;
        margin-left: auto;
        margin-right: auto;" /></a>
 <br>
 <em>MobiCom 2020 - FaceRevelio Teaser Video</em>
 </p>

<!-- <p style="text-align: justify"> -->
More recently, I developed, IoTCupid, a new secure, and usable decentralized group pairing system for IoT devices with heterogeneous sensing modalities. My work demonstrates that two devices can use the time interval between the subsequent occurrences of a commonly observed event type (e.g., coffee-machine-on events sensed by the microphone and power meter) as proof of co-presence and use them as evidence to establish a symmetric key. IoTCupid proposes a novel group key establishment protocol that enables dynamic group generation among devices and is resilient to man-in-the-middle, offline brute force and denial of key exchange attacks. This work was recently accepted to IEEE S&P and will be available online soon.
 
<b>Impact: </b> My work on liveness detection has gained recognition from both academia and industry, and a patent has been approved for it. Our work on IoT device pairing has encouraged the integration of secure and usable pairing mechanisms in emerging decentralized IoT systems such as Thread/OpenThread. To this end, the tools and algorithms I have developed allow developers to implement effective systems for improving users’ security and privacy. 
<!-- </p> -->