---
layout: post
title: My first research publication.
date: 2019-07-20 15:00
inline: false
tag:
- Generative Adversarial Networks
- Deep Learning
- Android Malware Analysis

---

I finally succeeded to publish my first article in a journal. 

***

### Abstract
Mobile and cell devices have empowered end users to tweak their cell phones more than ever and introduce applications just as we used to with personal computers. Android likewise portrays an uprise in mobile devices and personal digital assistants. It is an open‐source versatile platform fueling incalculable hardware units, tablets, televisions, auto amusement frameworks, digital boxes, and so forth. In a generally shorter life cycle, Android also has additionally experienced a mammoth development in application malware. In this context, a toweringly large measure of strategies has been proposed in theory for the examination and detection of these harmful applications for the Android platform. These strategies attempt to both statically reverse engineer the application and elicit meaningful information as features manually or dynamically endeavor to quantify the runtime behavior of the application to identify malevolence. The overgrowing nature of Android malware has enormously debilitated the support of protective measures, which leaves the platforms such as Android feeble for novel and mysterious malware. Machine learning is being utilized for malware diagnosis in mobile phones as a common practice and in Android distinctively. It is important to specify here that these systems, however, utilize and adapt the learning‐based techniques, yet the overhead of hand‐created features limits ease of use of such methods in reality by an end user. As a solution to this issue, we mean to make utilization of deep learning–based algorithms as the fundamental arrangement for malware examination on Android. Deep learning turns up as another way of research that has bid the scientific community in the fields of vision, speech, and natural language processing. Of late, models set up on deep convolution networks outmatched techniques utilizing handmade descriptive features at various undertakings. Likewise, our proposed technique to cater malware detection is by design a deep learning model making use of generative adversarial networks, which is responsible to detect the Android malware via famous two‐player game theory for a rock‐paper‐scissor problem. We have used three state‐of‐the‐art datasets and augmented a large‐scale dataset of opcodes extracted from the Android Package Kit bytecode and used in our experiments. Our technique achieves F1 score of 99% with a receiver operating characteristic of 99% on the bytecode dataset. This proves the usefulness of our technique and that it can generally be adopted in real life.

<center>
<div>
    <img class="col three" src="{{site.baseurl}}/assets/images/GANNN.jpg">
	<figcaption class="caption">Block diagram of LSTM-GAN Architecture used in our expermients</figcaption>
</div>
</center>

***

### Links for the paper 
- Wiley Link : [Here](https://onlinelibrary.wiley.com/doi/abs/10.1002/ett.3675)
- ResearchGate Link : [Here](https://www.researchgate.net/publication/334479318_Android_malware_detection_through_generative_adversarial_networks?_sg=8rWKXZt9omxHXYyn_4CDh8j5bRgwX_Aap3KFeJTBMP09oeqpNWpsq5vl_5PcSnHMaIFD4zM3PYcrAw._PBE9vktyY4n5aXYzjAuGVW7m3wb9RIiewWtZmwiJmhpAldE0rJ_w5JjSus-HiVwfh2_z3aJNeNnb9zwJgIbqA&_sgd%5Bnc%5D=1&_sgd%5Bncwor%5D=0)
- Download the paper : <a href="../../16506963.pdf" download>Here</a>

***

### Bibtex 

{% highlight markdown %}
@article{ruby,
  title={Android malware detection through generative adversarial networks},
  author={Amin, Muhammad and Shah, Babar and Sharif, Aizaz and Ali, Tamleek and Kim, Ki‐lL and Anwar, Sajid},
  month={Jul},
  year={2019},
  journal={Transactions on Emerging Telecommunications Technologies}, 
  publisher={John Wiley & Sons, Ltd},
}
{% endhighlight %}

