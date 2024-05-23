---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 🙋‍♀️ Profile 
I obtained my Ph.D. degree from Hosei University in March 2024 and my M.S. degree in September 2020. 

My **research interest** lies in _**Image Codec design**_ based on _**Compressive Sensing**_, which encompasses _**Hardware Implementation**_ and _**Deep Learning**_. 

Throughout my doctoral and master's studies, I have authored **10 papers**, most of which have been published in leading conferences and journals in the fields of image processing and hardware implementation, including **TMM, CVM, MMM, ISCAS, DCC, ICIP, IJCNN**, among others. 

I possess a strong ability for **self-directed learning** and have **independently acquired knowledge** in areas relevant to my research topic during my graduate studies, as well as in iOS application development during my undergraduate studies.

I am currently actively seeking post-doctoral or researcher opportunities and aspire to join a growth-oriented team where I can make meaningful contributions to advancement and development. 


# 📝 Publications 

**Improve the Compression Ratio: MATLAB**

 Existing Issues:
– The compression ratio achieved by the initial CS-based codec is insufficient.
– To improve the compression ratio, intra-prediction, quantization, and entropy coding are integrated into
the original framework.
– Intra-prediction results in time consumption.
– The input data lacks sufficient sparsity for quantization, resulting in noticeable quality degradation as
the quantization parameter increases, despite improved compression rates.

◦ Our Proposal:
– The previous simplified reconstruction algorithm was divided into two distinct components. It was
observed that processing the first reconstruction part yielded sparser data.
– Moving the first reconstruction part to the encoder reduces decoding time and functions similarly to
intra-prediction in other methods, with minimal complexity increase for obtaining sparser data.
– Leveraging this sparser data improves the compression ratio and reduces quantization degradation.
– This effort yielded a reduction of 16.16% in bpp, accompanied by a 38.46% increase in quality, and an
overall speedup of 165.18 × in terms of time cost.


- `TMM` [Compressive Sensing Based Image Codec With Partial Pre-Calculation](https://ieeexplore.ieee.org/abstract/document/10297548)
**Jiayao Xu**, Jian Yang, Fuma Kimishima, Ittetsu Taniguchi, Jinjia Zhou


**Speedup Reconstruction: FPGA**

◦ Existing Issues:
– Time cost of reconstruction is the Primary bottleneck in CS.
– Current reconstruction efforts aim to enhance speed while ensuring the generality of the measurement matrix.
– There’s a tradeoff between generality and speed, with hardware limitations preventing alteration of the selected sampling matrix.

◦ Our Proposal:
– Identify a sampling matrix that produces a sparse sensing matrix for reconstruction, yielding high-quality results.
– Utilize the sparsity of the sensing matrix to streamline each iteration in the reconstruction process.
– Simplify the reconstruction further, replacing iterative reconstruction with a single matrix multiplication.
– Achieve the fastest reconstruction speed of 81.92Gpixels/s while demanding minimal hardware resources

- `MMM` [Real-time FPGA Design for OMP Targeting 8K image Reconstruction](https://link.springer.com/chapter/10.1007/978-3-030-98358-1_41)
**Jiayao Xu**, Chen Fu, Zhiqiang Zhang, Jinjia Zhou

- `ISCAS` [An 81.92Gpixels/s Fast Reconstruction of Images from Compressively Sensed Measurements](https://ieeexplore.ieee.org/abstract/document/9937930)
**Jiayao Xu**, Pham Do Kim Chi, Chen Fu, Jinjia Zhou




**Improve the Image Quality: Python, Pytorch, OpenCV, MATLAB**

◦ Existing Issues:
– Higher sampling rates improve quality for high-frequency blocks, with minimal impact on low-frequency
ones.
– Adaptive sampling is introduced in existing works to tackle this issue.
– Computation of sampling rates per block in existing works is image-based, requiring two rounds of
sampling and reconstruction, leading to high time and hardware costs.
◦ Our Proposal:
– Investigating the correlation between the sampling procedure and edge detection calculation, the edge
detection method is implemented by multiplying a vector with sampled data.
– Achieving adaptive sampling calculation on the sampled data, saving hardware and time costs without
requiring additional reconstruction.
– Integrated without change into any compressive sensing-based codec framework, achieving plug-and-
play capability.
– Enhancing existing methods by 0.8-4.27dB under the same sampling rate


- `Peer Review` [Plug-and-Play Adaptive Block Compressive Sensing using Edge-Detection on the Compressed Domain]
**Jiayao Xu**, Yibo Fan, Jinjia Zhou



**Other works**

- `ICVIP` [High-speed Compressed Sensing Reconstruction using Zigzag Ordering based Parallel Processing](https://dl.acm.org/doi/abs/10.1145/3447450.3447489)
**Jiayao Xu**, Jirayu Peetakul, Muchen Li, Jinjia Zhou

- `CVM, ACCEPT` [JVCSR+: Adaptively Learned Video Compressive Sensing Reconstruction with Joint In-loop Reference Enhancement and Out-loop Super-resolution] 
Jian Yang, **Jiayao Xu**, Jinjia Zhou

- `DCC` [Zigzag Ordered Walsh Matrix for Compressed Sensing Image Sensor](https://ieeexplore.ieee.org/abstract/document/10125342)
Jinyao Zhou, **Jiayao Xu**, Jirayu Peetakul, Jinjia Zhou

- `ICIP` [Dynamic Unilateral Dual Learning for Text-to-Image Synthesis](https://ieeexplore.ieee.org/abstract/document/10223128)
Zhiqiang Zhang, **Jiayao Xu**, Ryugo Morita, Wenxin Yu, Jinjia Zhou

- `IJCNN, ACCEPT` [High Frequency Feature Distillation Network for Compressive Sensing Reconstruction]
Fuma Kimishima, **Jiayao Xu**, Jinjia Zhou

- `MMSP` [Optimizing CABAC architecture with prediction based context model prefetching](https://ieeexplore.ieee.org/abstract/document/9949499)
Chen Fu, Heming Sun, **Jiayao Xu**, Zhiqiang Zhang, Jinjia Zhou


# 🔥 Skills
• **Languages:** English - TOEIC(845/990), Japanese - JLPT N2(120/180), Mandarin - Native speaker

• **Programming Languages:** Python, C/C++, MATLAB, Verilog , Objective-C

• **Software Development:** Object-Oriented Programming (OOP), Design Patterns, Team Collaboration

• **Platform:** Visual Studio Code, MATLAB, Modelsim, Vivado, XCode, Wireshark, Git version control

• **OS (environment setting and system maintenance):** Windows, Centos 7, Ubuntu 18, macOS

# 👩‍💻 iOS Project
**Name**: iSWUST (i西科) 

**Supported users**: 3,000+ Active Users 

**Laboratory**: Mobile Web Laboratory (移动互联网实验室)

**Work duration**: Sep.2015 – Mar.2017

**Release Time**: December 4th, 2016

**Current status**: out of service.

• Introduction:

Provide on-campus student services such as checking lecture schedules, accessing library book collection information, verifying campus card balances, and processing recharges.

• Responsibility:
  
1. Contributed to API design and revised API documentation to enhance comprehension and utilization by the development team.

2. Conducted a refactoring of the existing application, employing Git version control to facilitate code collaboration and project management. Utilized various design patterns to reduce coupling and enhance code maintainability.

3. Developed and integrated functionality for library and login modules, implementing rigorous testing methods to validate code accuracy and reinforce system stability.

4. Orchestrated the implementation of the network layer, encapsulating data packets in JSON format. Collaborated closely with the backend team to conduct comprehensive testing of the network layer, ensuring seamless communication with backend services and making necessary adjustments to meet project requirements.


<img src="/images/iswust1.jpg" width="300" >
<img src="/images/iswust2.png" width="300" >



# 📖 Educations
- *2020.09 - 2024.03*, Ph.D, Hosei University, Tokyo, Japan.
- *2018.09 - 2020.09*, Master, Hosei University, Tokyo, Japan.
- *2014.09 - 2018.06*, Bachelor, Southwest University of Science and Technology, Sichuan, China.

# 💬 Invited Talks
- *2023.10*, Compressive Sensing Based Image Codec With Partial Pre-Calculation talk in Institut National des Sciences Appliquées de Rennes, INSA de Rennes.
- *2022.09 - 2024.03*, Regular seminar with Fudan University and Zhejiang University for Image Compression using Compressive Sensing.
- *2022.08*, Compressive Sensing Seminar with Osaka Univerisity.
- *2022.06*, Real-time hardware design for Compressive Sensing reconstruction talk, MMM 2022.
- *2022.05*, a hardware design reaches 81.92 GPixel/s for Compressive Sensing reconstruction talk, ISCAS 2022.
- *2020.12*, Parallel reconstruction design for Compressive Sensing reconstruction talk, ICVIP 2020.

# 🎖 Honors and Awards
- *2020-2023* Research grants from Hosei University Graduate School.
- *2020-2021* JASSO scholarship.
- *2020.12* The best presentation of all excellent presentations at the 3rd International Conference on Image and Video Processing (ICIVP 2020). 



