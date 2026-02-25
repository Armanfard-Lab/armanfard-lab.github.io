---
title: "ASTAD - AAAI-26"
layout: gridlay2
excerpt: "ASTAD - AAAI-26"
sitemap: false
permalink: /astad3/
---

<h1 align="center"> 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) </h1>



{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
  
  <div style="border-radius: 16px; padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad_aaai26_logo.png" style="width: 500px; max-width: 95vw; height: auto; display: block; margin: 0 auto;" />
</div>


 

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}

<h2 align="center">Overview</h2>
<hr>

<p align="center">The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) at AAAI 2026 is a premier platform for researchers and practitioners at the forefront of AI-driven anomaly detection. With the proliferation of spatiotemporal data from sources like surveillance cameras, IoT sensors, and satellite imagery, the need for robust, automated systems to identify novel and unusual patterns has never been more critical. This workshop will delve into cutting-edge AI techniques that move beyond traditional rule-based methods to uncover hidden anomalies, fostering a new generation of intelligent monitoring and discovery. Join us to discuss how we can build more resilient, autonomous, and insightful systems for a safer and more efficient world.</p>

<h2 align="center"> Call for Paper </h2>
<hr>
  
<p align="left">We invite researchers and practitioners to submit their original research contributions to The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of AAAI 2026. This workshop aims to explore the latest advancements and novel approaches in anomaly detection (AD) using Artificial Intelligence techniques, with a focus on spatial and temporal dimensions. Topics of Interest :</p>
  
  <ul>
    <li> Novel deep learning and generative models for spatiotemporal AD </li>
    <li> Self-supervised, unsupervised and few-shot learning for AD with limited data </li>
    <li> Continual learning approaches for evolving anomalous patterns </li>
    <li> Explainable AI for interpreting and justifying anomaly detection decisions </li>
    <li> Foundation models for anomaly detection, including large language models (LLMs) and vision-language models (VLMs) </li>
    <li> Novel datasets, benchmarks, and evaluation metrics </li>
    <li> On-edge anomaly detection in real-time and resource-constrained settings </li>
    <li> Applications in computer vision, robotics, autonomous driving, predictive maintenance, healthcare, finance, and beyond </li>
  </ul>  

<p align="left">Submission Site: <a href="https://openreview.net/group?id=AAAI.org/2026/Workshop/ASTAD" target="_blank">OpenReview</a></p>


<h2 align="center"> Schedule </h2>
<hr>

  <ul style="list-style: none; padding-left: 0;">
    <li><span style="display: inline-block; width: 140px;"><b>09:00 – 09:15:</b></span> <b>Opening</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>09:15 – 10:15:</b></span> <b>Keynote: Dr. Ye Zhu</b><br><span style="display: inline-block; width: 140px;"></span><em>Anomaly Detection Based on Isolation Mechanisms</em></li>
    <li><span style="display: inline-block; width: 140px;"><b>10:15 – 10:30:</b></span> <b>Coffee Break</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>10:30 – 12:00:</b></span> <b>Paper Session (Oral)</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>12:00 – 13:00:</b></span> <b>Lunch Break</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>13:00 – 14:00:</b></span> <b>Keynote: Dr. Jie Ren</b><br><span style="display: inline-block; width: 140px;"></span><em>Uncertainty Estimations in LLMs</em></li>
    <li><span style="display: inline-block; width: 140px;"><b>14:00 – 15:00:</b></span> <b>Keynote: Prof. Pang Guansong</b><br><span style="display: inline-block; width: 140px;"></span><em>Anomalies Are Not a Class: Leveraging Labeled Anomalies in Deep and Generalist Anomaly Detection</em></li>
    <li><span style="display: inline-block; width: 140px;"><b>15:00 – 15:30:</b></span> <b>Poster Session</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>15:30 – 16:00:</b></span> <b>Coffee Break</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>16:00 – 16:50:</b></span> <b>Poster Session</b></li>
    <li><span style="display: inline-block; width: 140px;"><b>16:50 – 17:00:</b></span> <b>Closing</b></li>
  </ul>

<h2 align="center"> Important Dates </h2>
<hr>

   <p align="left"> The important dates are as follows: </p>
<ul>
<li> <b>Paper submission deadline:</b> October 22, 2025 </li>
 <li> <b>Author notification:</b> November 5, 2025 </li>
 <li> <b>Camera-ready deadline:</b> November 10, 2025 </li>
 <li> <b>Workshop Date:</b> January 26, 2026 (9AM - 5PM Singapore Time) </li>
<li> <b>Workshop Location:</b> Grand Mercure Roxy Hotel – Amber </li>
  </ul>

<h2 align="center"> Accepted Papers </h2>
<hr>

<table style="width: 100%; margin: 20px auto; border-collapse: collapse;">
  <thead>
    <tr style="background-color: #f5f5f5;">
      <th style="width: 6%; text-align: center; padding: 12px; border: 1px solid #ddd;">Paper ID</th>
      <th style="width: 40%; text-align: left; padding: 12px; border: 1px solid #ddd;">Title</th>
      <th style="width: 46%; text-align: left; padding: 12px; border: 1px solid #ddd;">Authors</th>
      <th style="width: 8%; text-align: center; padding: 12px; border: 1px solid #ddd;">PDF</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">1</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Unveiling the Flaws: A Critical Analysis of Initialization Effect on Time Series Anomaly Detection</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Alexander Koran, Hadi Hojjati, Narges Armanfard</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/2_Unveiling_the_Flaws_A_Critic.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">2</td>
      <td style="padding: 10px; border: 1px solid #ddd;">EngineAD: A Real-World Vehicle Engine Anomaly Detection Dataset</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Hadi Hojjati, Christopher Z Roth, Rory Woods, Ken Sills, Narges Armanfard</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/3_EngineAD_A_Real_World_Vehicl.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">3</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Generative Flow Models in Weight Space for Detecting Covariate Shifts</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Daniel Saragih, Deyu Cao, Tejas Balaji</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/5_Generative_Flow_Models_in_We.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">4</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Advancing Thermal Fault Diagnostics for Lithium-Ion Energy Storage Systems: An Autonomous Vision Foundation-Based Approach</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Huixin Xu, Chaoyu Dong, Qian Xiao, Yu Jin, Hongjie Jia</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/7_Advancing_Thermal_Fault_Diag.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">5</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Leveraging Physics Anomaly Knowledge and Contrastive Learning for Region-Agnostic Landslide Prediction</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Ren Ozeki, Hirozumi Yamaguchi</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/8_Leveraging_Physics_Anomaly_K.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">6</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Domain-Adaptive Video Captioning for Surveillance Videos</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Fengqi Zhang, Chunrui Hua, Shuaijie Li, Wen Qi</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/9_Domain_Adaptive_Video_Captio.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">7</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Anomaly-driven Reinforcement Learning</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Saurabh Varshneya, Maik Schürmann, Philipp Liznerski, Mayank Chetan Ahuja, Jan C. Aurich, Sophie Fellenz, Marius Kloft</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/13_Anomaly_driven_Reinforcemen.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">8</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Benchmarking IoT Time-Series AD with Event-Level Augmentations</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Dmitry Zhevnenko, Aleksandr Kovalenko, Fedor Meshchaninov, Anton Kozhukhov, Travnikov Vladislav, Makar Ippolitov, Kirill Yashunin, Iurii Katser, Ilya Makarov</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/14_Benchmarking_IoT_Time_Serie.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">9</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Bridging the Data Gap: Spatially Conditioned Diffusion Model for Anomaly Generation in Photovoltaic Electroluminescence Images</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Shiva Hanifi, Sasan Jafarnejad, Raphael Frank</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/16_Bridging_the_Data_Gap_Spati.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">10</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Modular Segmentation-Agnostic Framework for Object-Based Change Detection in Multi-Temporal VHR Imagery</td>
      <td style="padding: 10px; border: 1px solid #ddd;">Abdul-Rashid Zakaria, Teresa J. DiMeola, Charles Walter, Pasi Lautala, Thomas Oommen, Hong Xiao</td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;"><a href="{{ site.url }}{{ site.baseurl }}/ASTAD_Papers/20_Modular_Segmentation_Agnost.pdf" target="_blank" rel="noopener">PDF</a></td>
    </tr>
  </tbody>
</table>

  <h2 align="center"> Speakers </h2>
<hr>

{% assign number_printed = 0 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad3/YeZhu.jpg" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left; object-fit: cover;" />
  <h4>Dr. Ye Zhu</h4>
  <i>School of Information Technology, Deakin University</i>
  <p style="font-size:14px;">Dr Ye Zhu is a Senior Lecturer of computer science with the School of Information Technology, Deakin University, Geelong, VIC, Australia. He is an IEEE senior member and also a visiting faculty in Peking University and Nanjing University. He received a PhD degree in Artificial Intelligence with a Mollie Holman Medal for the best doctoral thesis of the year from Monash University in 2017. His research focuses on the fields of data mining and machine learning, particular topics including clustering analysis, anomaly detection, similarity learning, and their applications for pattern recognition and information retrieval. Dr Zhu has published over 90 papers in top-tier conferences and journals, including SIGKDD, VLDB, ICML, IJCAI, AAAI, AIJ, VLDBJ, ISJ, TKDE, PRJ, JAIR, and MLJ.</p>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad3/PangGuansong.jpg" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left; object-fit: cover;" />
  <h4>Prof. Pang Guansong</h4>
  <i>School of Computing and Information Systems, Singapore Management University</i>
  <p style="font-size:14px;">Dr. Guansong Pang is a tenure-track Assistant Professor of Computer Science and Lee Kong Chian Fellow at the School of Computing and Information Systems, Singapore Management University (SMU), where he leads the Machine Learning & Applications (MaLA) Lab. He is also a faculty member of Centre on Security, Mobile Applications and Cryptography. He was a Research Fellow with the Australian Institute for Machine Learning (AIML), University of Adelaide, Australia. Before joining AIML, he received his Ph.D. at University of Technology Sydney (UTS), Australia. His research interests include machine learning, data mining, and computer vision, with a research theme focused on recognizing and generalizing to abnormal, unknown, or unseen data for creating trustworthy AI systems.<span id="pang-more" style="display:none;"> His research has attracted 11,000+ citations and received multiple global recognition/awards, e.g., the prestigious 2020 UTS Chancellor's Award List, the World's Top 2% Scientists in 2022-2025 (the single-year or career-long category), DSAA 2023 Best Paper Award (Applications Track), and the Most Influential KDD 2023 Papers. He has been organizing a series of workshops and tutorials on anomaly and novelty detection at various conferences such as KDD, WSDM, CVPR, ICCV, IJCAI, and AAAI. He serves as Area Chair of NeurIPS, ICLR, ICML, CVPR, KDD, PAKDD, IJCAI and AAAI (Senior PC), Associate Editor of IEEE Transactions on Neural Networks and Learning Systems (TNNLS) and Pattern Recognition, and Editorial Board Member of IEEE Intelligent Systems and International Journal of Data Science and Analytics.</span> <a href="javascript:void(0);" id="pang-read-more" onclick="document.getElementById('pang-more').style.display='inline'; this.style.display='none'; document.getElementById('pang-less').style.display='inline';" style="color: #9E0918; text-decoration: none; cursor: pointer;">Read more</a><a href="javascript:void(0);" id="pang-less" onclick="document.getElementById('pang-more').style.display='none'; this.style.display='none'; document.getElementById('pang-read-more').style.display='inline';" style="display:none; color: #9E0918; text-decoration: none; cursor: pointer;"> Read less</a></p>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad3/JieRen.jpeg" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left; object-fit: cover;" />
  <h4>Dr. Jie Ren</h4>
  <i>Google DeepMind</i>
  <p style="font-size:14px;">Jie Ren is a Staff Research Scientist at Google DeepMind. She holds a PhD in Computational Biology and Bioinformatics and an MSc in Statistics, from the University of Southern California. Jie's research centers on developing trustworthy AI solutions that can be safely deployed in real-world scenarios, aiming to advance scientific discoveries and enhance human well-being. Her work spans three key areas: (1) uncertainty estimation and robustness in large foundation models, (2) out-of-distribution detection and robustness in deep learning, and (3) the development of reliable machine learning for real-world application, with a special focus on biological and medical research.</p>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>

<h2 align="center">Workshop Poster</h2>
<hr>

<div style="padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad3_poster.png" style="width: 800px; max-width: 95vw; height: auto; display: block; margin: 0 auto; border-radius: 0;" />
</div>




<h2 align="center"> Organizers </h2>
<hr>

{% assign number_printed = 0 %}
{% for member in site.data.ijcaimember %}
{% if member.name == "Narges Armanfard (Chair)" %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} - {{ member.email }}</i>
  <p style="font-size:14px;">{{ member.bio }}</p>
  <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>
{% endif %}
{% endfor %}

{% for member in site.data.team_members %}
{% if member.name == "Hadi Hojjati" or member.name == "Thi Kieu Khanh Ho" %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} - {{ member.email }}</i>
  <p style="font-size:14px;">{{ member.bio }}</p>
  <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>
{% endif %}
{% endfor %}

<h2 align="center"> Keynote Talks </h2>
<hr>

<div style="max-width: 900px; margin: 0 auto;">
  <h3>Dr. Ye Zhu</h3>
  <p><strong>Title:</strong> Anomaly Detection Based on Isolation Mechanisms</p>
  <p><strong>Abstract:</strong> Anomaly detection is a longstanding and active research area that has many applications in domains such as finance, security and manufacturing. However, the efficiency and performance of anomaly detection algorithms are challenged by the large-scale, high-dimensional and heterogeneous data that are prevalent in the era of big data. Isolation-based unsupervised anomaly detection is a novel and effective approach for identifying anomalies in data. It relies on the idea that anomalies are few and different from normal instances, and thus can be easily isolated by random partitioning. Isolation-based methods have several advantages over existing methods, such as low computational complexity, low memory usage, high scalability, robustness to noise and irrelevant features, and no need for prior knowledge or heavy parameter tuning. This talk reviews the state-of-the-art isolation-based anomaly detection methods, including their data partitioning strategies, anomaly score functions, and algorithmic details. It also discusses some extensions and applications of isolation-based methods in different scenarios, such as detecting anomalies in streaming data, time series, trajectory and image datasets.</p>

  <h3>Dr. Jie Ren</h3>
  <p><strong>Title:</strong> Uncertainty Estimations in LLMs</p>

  <h3>Prof. Pang Guansong</h3>
  <p><strong>Title:</strong> Anomalies Are Not a Class: Leveraging Labeled Anomalies in Deep and Generalist Anomaly Detection</p>
  <p><strong>Abstract:</strong> Most anomaly detection (AD) research focuses on unsupervised or semi-supervised settings, where models are trained using only normal data, or unlabeled data assumed to be predominantly normal. While this paradigm avoids reliance on anomaly labels, it inherently limits discriminability, as models lack explicit knowledge of what constitutes abnormality. In many real-world applications, however, labeled anomaly examples are available. These may include verified defect or tumor samples in a target system, as well as curated anomaly datasets released publicly. Such labeled anomalies encode valuable prior knowledge about abnormalities of interest and, when properly leveraged, can significantly enhance detection performance. A key challenge is that labeled anomalies rarely exhaust the space of abnormal behaviors encountered at inference time, raising fundamental questions about generalization beyond seen anomaly types. This talk reviews recent progress in "supervised anomaly detection", a paradigm that exploits labeled anomaly data while explicitly addressing unknowingness, open-set nature of anomalies. We discuss two research directions. The first focuses on open-set supervised anomaly detection, where models are trained with known anomaly classes yet are required to detect previously unseen anomalies during inference. The second explores generalist anomaly detectors, which are trained once on auxiliary labeled anomaly datasets and can generalize across domains/datasets without retraining. Together, these advances challenge the notion of anomalies as a fixed class (i.e., supervised anomaly detection ≠ binary classification) and point toward more discriminative, generalized anomaly detection systems.</p>
</div>

 