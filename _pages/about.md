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

I am currently a final-year Ph.D. candidate at Ubiqutous System Security Lab (USSLAB), Zhejiang University. I am co-supervised by <a href='https://scholar.google.com/citations?hl=en&user=FCsdj0YAAAAJ'>Prof. Wenyuan Xu</a>, <a href="https://sites.google.com/site/xiaoyuijh">Prof. Xiaoyu Ji</a>, and <a href="https://cyansec.com/">Prof. Chen Yan</a>.
 <!-- <a href='../docs/Xinfeng_Li_CV.pdf'>My Resume</a> -->

<!-- **I am expected to graduate in June 2024 and I'm on the job market (acadamia/industry). Consider dropping me an email if you have any suitable opportunities.** -->


<!-- My research interest covers a wide range, including Sensor and CPS Security, Audio Security, AI Security, as well as Speech Signal Processing. If you are seeking any form of <b>academic cooperation</b>, please feel free to email me at lxfmakeit(at)zju(dot)edu(dot)cn. -->
My research is broadly in the field of AI and IoT security, with a particular interest in safeguarding user privacy, intelligent audio/vision systems, and generative models against various forms of leaks and attacks.
I work toward developing dependable and secure machine learning (ML) systems and am committed to making their applications for deployment in critical infrastructures and consumer electronics. In user-oriented contexts, my investigations also encompass the interplay between protecting user privacy and enhancing the usability of machine learning systems. In model-oriented scenarios, such as the use of generative models in model-as-a-service (MaaS) applications, my work involves regulating their behavior to align with societal responsibilities.

If you are seeking any form of <b>academic cooperation</b>, please feel free to email me at xinfengli(at)zju(dot)edu(dot)cn.

I have published 10+ papers at the top-tier international security/AI/mobile sensing conferences and journals, such as USENIX Security, CCS, NDSS, TDSC, IoT-J, and ACM MM.

<!-- My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->


# 🔥 News
- *2024.05*: &nbsp;📝 **SafeGen** was accepted by CCS 2024! As T2I technologies advance, their misuse to generate sexually explicit content has become a major concern. SafeGen effectively mitigates this by removing any explicit visual representations from the model, making it safe regardless of the adversarial text input, outperforming eight other protection approaches. SafeGen adjusts the model's visual self-attention layers to ensure that the high-quality production of benign images is not compromised. More information are on our [code](https://github.com/LetterLiGo/SafeGen_CCS2024).
- *2024.05*: &nbsp;🔥 **SafeEar** got accepted by CCS 2024! To our knowledge, this is the 1st content privacy-preserving audio deepfake detection framework. Since audio deepfakes and user privacy concerns have been increasingly significant societal issues, we demonstrate how to achieve reliable deepfake detection while preventing both machine and human adversaries from eavesdropping on sensitive user speech content. To facilitate future research, we also develop a comprehensive multilingual deepfake datasets (more than 1,500,000 genuine & deepfake audio samples) using advanced TTS/VC techniques. Please check out our [demo page](https://letterligo.github.io/SafeEar/).
- *2024.02*: &nbsp;🎉 I am so excited to be awarded the NDSS 2024 Student Grant.
- *2023.12*: &nbsp;🔥 One Vision-Language Model Security paper submitted to S&P (Oakland) 2024 (Core A*, Big4, CCF-A).
<!-- - *2023.09*: &nbsp;🍀 One LLM-oriented paper submitted to NSDI 2024 (CCF-A, one of the best conference on network and system related topics). -->
- *2023.08*: &nbsp;🎉 **VRifle** got accepted by NDSS 2024! We demonstrate how to achieve completely inaudible adversarial perturbation attack via ultrasound, which achieves the farthest attack range (~10 meters away) and most universal capability (1 perturb. can tamper with >28,000 benign samples). Our novel ultrasonic transformation model can be generalized to other modality of attacks, such as laser, electromagentic.
- *2023.08*: &nbsp;🔥 I attend USENIX Security 2023 Symposium and present our work **NormDetect** in person.
- *2023.07*: &nbsp;😄 Our practical backdoor attack (**SMA**) against ASR models is accepted by ACM MM 2023!
- *2022.09*: &nbsp;🎉 **Tuner** and **UltraBD** are accepted by IoT-J 2023 and ICPADS 2022! We demonstrate a practical inaudible backdoor attacks against the speaker recognition systems.
- *2022.07*: &nbsp;💪🏻 **NormDetect** is accepted by USENIX Security 2023! We rethink the challenging topic of defending against inaudible voice attacks, and present a software-based mitigation that can instantly protect legacy and future devices in an actionable and practical manner, which is verified on 24 mainstream smart devices with voice interfaces.
- *2021.07*: &nbsp;🎉 **PROLE Score** is accepted by USENIX Security 2022! "OK Siri" or "Hey Google"? We conduct an extensive voiceprint security measurement. Our findings and designed metrics shall aid manufactures and users to DIY highly secure voiceprint phrases.
- *2020.12*: &nbsp;🔥 **EarArray** is accepted by NDSS 2021! We uncover the inherent physical properties of inaudible attack, i.e. ultrasound field distributions, and redesign microphone arrays for accurate detection and attack localization.

# 📝 Selected Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACM CCS 2024</div><img src='./images/SafeGen.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SafeGen: Mitigating Sexually Explicit Content Generation in Text-to-Image Models](https://arxiv.org/abs/2404.06666) **Xinfeng Li**, Yuchen Yang, Jiangyi Deng, Chen Yan, Yanjiao Chen, Xiaoyu Ji, Wenyuan Xu. To appear in Proceedings of ACM Conference on Computer and Communications Security, **CCS 2024** (CCF-A, Big4) [[Code](https://github.com/LetterLiGo/SafeGen_CCS2024)][[Pretrained Weights](https://huggingface.co/LetterJohn/SafeGen-Pretrained-Weights)]

As T2I technologies advance, their misuse to generate sexually explicit content has become a major concern. SafeGen effectively mitigates this by removing any explicit visual representations from the model, making it safe regardless of the adversarial text input, outperforming eight other protection approaches. SafeGen adjusts the model's visual self-attention layers to ensure that the high-quality production of benign images is not compromised. 
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACM CCS 2024</div><img src='./images/SafeEar.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SafeEar: Content Privacy-Preserving Audio Deepfake Detection](https://letterligo.github.io/SafeEar/) **Xinfeng Li**, Kai Li, Yifan Zheng, Chen Yan, Xiaoyu Ji, Wenyuan Xu. To appear in Proceedings of ACM Conference on Computer and Communications Security, **CCS 2024** (CCF-A, Big4) [[Project Page](https://letterligo.github.io/SafeEar/)]

To our knowledge, SafeEar is the first content privacy-preserving audio deepfake detection framework. Since audio deepfakes and user privacy concerns have been increasingly significant societal issues, we demonstrate how to achieve reliable deepfake detection while preventing both machine and human adversaries from eavesdropping on sensitive user speech content. To facilitate future research, we also develop a comprehensive multilingual deepfake datasets (more than 1,500,000 genuine & deepfake audio samples) using advanced TTS/VC techniques.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NDSS 2024</div><img src='./images/Vrifle.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Inaudible Adversarial Perturbation: Manipulating the Recognition of User Speech in Real Time](https://arxiv.org/abs/2308.01040), **Xinfeng Li**, Chen Yan, Xuancun Lu, Xiaoyu Ji, Wenyuan Xu., In Proceedings of Network and Distributed System Security Symposium, **NDSS 2024** (CCF-A, Big4) [[Google Site](https://sites.google.com/view/vrifle)], [[Website](https://zjushine.github.io/VRIFLE/)], [[Code](https://github.com/LetterLiGo/Adversarial_Audio_Attack-VRifle)]

<!-- [**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong> -->
- First completely inaudible adversarial perturbation attacks, increasing the attack range to 10 meters away.
- First attempt on ultrasound transformation modeling.
- Significant improvement of attack distances, universality, and stealthiness compared with prior adversarial example attacks.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">USENIX 2023</div><img src='images/normdetect.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
[Learning Normality is Enough: A Software-based Mitigation against the Inaudible Voice Attacks](https://www.usenix.org/conference/usenixsecurity23/presentation/li-xinfeng), **Xinfeng Li**, Xiaoyu Ji, Chen Yan, Chaohao Li, Yichen Li, Zhenning Zhang, Wenyuan Xu.,
In Proceedings of 32nd **USENIX Security 2023** (CCF-A, Big4) [[Google Site](https://sites.google.com/view/normdetect)]
<!-- [**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong> -->
- Unsupervised software-based mitigation that can instantly protect miscallenous legacy devices.
- Universal detection performance demonstrated on a wide range of devices.
</div>
</div>
<!-- - [CommandSense: Automating Shell Log Auditing with Proprietary Command Explanation System](), USENIX Symposium on Networked Systems Design and Implementation, **NSDI** (CCF-A, Top 1-tier System Conference, in submission) -->

- [Scoring Metrics of Assessing Voiceprint Distinctiveness based on Speech Content and Rate](), Ruiwen He, Yushi Cheng, Junning Ze, **Xinfeng Li**, Xiaoyu Ji, Wenyuan Xu. Transcations on Dependable and Secure Computing, **TDSC 2024** (CCF-A)

- [Inaudible Adversarial Perturbation: Manipulating the Recognition of User Speech in Real Time](https://arxiv.org/abs/2308.01040), **Xinfeng Li**, Chen Yan, Xuancun Lu, Xiaoyu Ji, Wenyuan Xu., In Proceedings of Network and Distributed System Security Symposium, **NDSS 2024** (CCF-A, Big4) [[Google Site](https://sites.google.com/view/vrifle)], [[Website](https://zjushine.github.io/VRIFLE/)], [[Code](https://github.com/LetterLiGo/Adversarial_Audio_Attack-VRifle)]

- [Detecting Inaudible Voice Commands via Acoustic Attenuation by Multi-channel Microphones](), Xiaoyu Ji, Guoming Zhang, **Xinfeng Li**, Gang Qu, Xiuzhen Cheng, Wenyuan Xu. Transcations on Dependable and Secure Computing, **TDSC 2023** (CCF-A)

- [The Silent Manipulator: Practical and Inaudible Backdoor Attack against Speech Recognition Systems](https://dl.acm.org/doi/10.1145/3581783.3613843), Zhicong Zheng, **Xinfeng Li**, Chen Yan, Xiaoyu Ji, Wenyuan Xu., ACM multimedia **MM 2023** (CCF-A)

- [Enrollment-stage Backdoor Attacks on Speaker Recognition Systems via Adversarial Ultrasound](https://arxiv.org/abs/2306.16022), **Xinfeng Li**, Junning Ze, Chen Yan, Yushi Cheng, Xiaoyu Ji, Wenyuan Xu., IEEE Internet of Things Journal, **IoT-J** (SCI, JCR-1)

- [Towards Pitch-Insensitive Speaker Verification via Soundfield](https://www.researchgate.net/publication/371918855_Towards_Pitch-Insensitive_Speaker_Verification_via_Soundfield), **Xinfeng Li**, Zhicong Zheng, Chen Yan, Chaohao Li, Xiaoyu Ji, Wenyuan Xu., IEEE Internet of Things Journal, **IoT-J** (SCI, JCR-1)

- [Learning Normality is Enough: A Software-based Mitigation against the Inaudible Voice Attacks](https://www.usenix.org/conference/usenixsecurity23/presentation/li-xinfeng), **Xinfeng Li**, Xiaoyu Ji, Chen Yan, Chaohao Li, Yichen Li, Zhenning Zhang, Wenyuan Xu.,
In Proceedings of 32nd **USENIX Security 2023** (CCF-A, Big4) [[Google Site](https://sites.google.com/view/normdetect)]

<!-- - [A Software-based Mitigation against Inaudible Voice Attacks with Channel Awareness and Normality Guidance](), **Xinfeng Li**, Chen Yan, Xiaoyu Ji, Wenyuan Xu. Transcations on Dependable and Secure Computing, **TDSC** (CCF-A, in submission) -->

- [UltraBD: Backdoor Attack against Automatic Speaker Verification Systems via Adversarial Ultrasound](https://ieeexplore.ieee.org/document/10078010), **Junning Ze**, **Xinfeng Li**, Yushi Cheng, Xiaoyu Ji, Wenyuan Xu., In Proceedings of 2022 IEEE 28th International Conference on Parallel and Distributed Systems **ICPADS 2022** (CCF-C) [[Extended Version](https://arxiv.org/abs/2306.16022)]

- [”OK, Siri” or ”Hey, Google”: Evaluating Voiceprint Distinctiveness via Content-based PROLE Score](https://www.usenix.org/conference/usenixsecurity22/presentation/he-ruiwen), Ruiwen He, Xiaoyu Ji, **Xinfeng Li**, Yushi Cheng, Wenyuan Xu., In Proceedings of 31st **USENIX Security 2022** (CCF-A, Big4) [[Google Site, Our Interactive Demo](https://sites.google.com/view/voiceprint-sec)]

- [EarArray: Defending against DolphinAttack via Acoustic Attenuation](https://www.ndss-symposium.org/ndss-paper/eararray-defending-against-dolphinattack-via-acoustic-attenuation/), Guoming Zhang, Xiaoyu Ji, **Xinfeng Li**, Gang Qu, Wenyuan Xu., In Proceedings of Network and Distributed System Security Symposium, **NDSS 2021** (CCF-A, Big4) 



<!-- Xinfeng Li, Chen Yan, Yichen Li, Zhenning Zhang, Xiaoyu Ji, Wenyuan Xu.
A Software-based Mitigation against Inaudible Voice Attacks with Channel Awareness and Normality Guidance. IEEE Transactions on Dependable and Secure Computing (CCF-A, SCI 1区, under review) -->

<!-- 
- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020** -->

# 🎖 Honors and Awards
- NDSS 2024 Student Grant (2024)
- Merit Graduate Student Scholarship & Excellent Graduate Student Scholarship & Excellent Graduate Student Cadre (Zhejiang University, 2020-2023)  
- "Challenge Cup" National College Student Curricular Academic Science and Technology Works Competition: First prize (Zhejiang University, 2021)  
- Outstanding Undergraduates at Edison Honor Class, (Zhejiang University 2019)  
- Top-10 Students at EE College (Top 1%, Zhejiang University, 2018)   
- National Scholarship (Top 2%, Zhejiang University, 2018)  
- Meritorious Scholarship (Top 3%, Zhejiang University, 2016-2018)  


# 📖 Educations
- *2019.06 - Present*, PhD, USSLAB, Zhejiang University, Hangzhou. 
- *2015.09 - 2019.06*, Undergraduate, Electrical Engineering College, Zhejiang Univeristy, Hangzhou.
- *2012.09 - 2015.06*, Yuyao High School, Ningbo.

# 💬 Invited Talks
- *2023.08*, USENIX Security Symposium 2023 at Anaheim, California, USA.  \| [\[Slides\]](https://www.usenix.org/conference/usenixsecurity23/presentation/li-xinfeng)
- *2024.02*, NDSS 2024 at San Diego, California, USA.  \| [\[Paper\]](https://www.ndss-symposium.org/ndss-paper/inaudible-adversarial-perturbation-manipulating-the-recognition-of-user-speech-in-real-time/)  \| [\[Code\]](https://github.com/LetterLiGo/Inaudible-Adversarial-Perturbation-Vrifle) \| [\[Video\]](https://www.youtube.com/watch?v=VD_KAU-s1oA) 
<!-- - *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

# 💻 Internships
- *2021.11 - 2022.05*, [杭州涿溪脑与智能研究所](), Hangzhou, China.

<!-- - *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->