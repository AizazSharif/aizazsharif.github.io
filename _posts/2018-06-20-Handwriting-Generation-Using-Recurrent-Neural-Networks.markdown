---
title:  "Handwriting Generation Using Recurrent Neural Networks"
layout: post
date:   2018-06-20 
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Long_Short Term Memory
- Sequence Generation
- PyTorch
category: blog
author: aizazsharif
# jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f35c.png" height="20" width="20" align="absmiddle">'
---

As many of us have used WordArt extensively back in school life and other tools similar to it for generating stylish text. Since then there is a lack of cursive font that can look similar to the human handwriting and also available to be used inside books and articles. Now, with the power of Deep Learning we are able to generate human-like handwriting (including some cursive) inside a computer.

I was recently introduced with the work of [Alex Graves](https://arxiv.org/abs/1308.0850) in which he proposed the basic architecture. The paper is hard to understand at first but I will try to break down the main points to get the overall picture.

## Architecture
The main architecture used behind handwriting generation is Long-Short Term Memory. The dataset needed for the task is [IAM Handwriting Database](http://www.fki.inf.unibe.ch/databases/iam-handwriting-database). The framework used for creating the whole model is Pytorch is a Deep Learning framework extensively used for research purposes and it is written in python. 


## Types of Handwriting Generation
There are two types of handwriting generation.
- Unconditional Handwriting
- Conditional Handwriting

### Unconditional Handwriting
Here the model is trained with the sequnces provided in the dataset and is asked to pick any handwriting style for generating some text at random to see the performance of the model. 

<img src="https://greydanus.github.io/assets/scribe/stroke_to_ascii.png">
<figcaption class="caption">Handwriting Generation</figcaption>


### Conditional Handwriting
It is more complex since the prediction is involved now. You will be training your model not just on the handwriting sequences but on the ascii text sentences in parallel as well. This way when the model is ready, it will generate handwriting based on text you have provided to generate.

<img src="https://greydanus.github.io/assets/scribe/ascii_to_stroke.png">
<figcaption class="caption">Handwriting generation from ascii characters</figcaption>



## Results
After training the model for 50 epochs I generated both Unconditional Handwriting and Conditional Handwriting images. The quality and accuracy of the handwriting can be increased if there is GPU accesible so that the model can be trained further for improvement.

---
<img src="{{site.baseurl}}/assets/images/conditional_sample_4.png">
<figcaption class="caption">Conditional Handwriting</figcaption>

---

---
<img src="{{site.baseurl}}/assets/images/unconditional_sample_2.png">
<figcaption class="caption">Unconditional Handwriting</figcaption>

---

There are a lot of minute technical details regarding the architecture but I am skipping that so that one can get the basic concept first before exploring more. The two sources that helped me in this were the proposed paper itself and the lecture of the author himself at the Oxford University on this topic.

---
<iframe width="560" height="315" src="https://www.youtube.com/embed/-yX1SYeDHbg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

---
You can find the source code [here](https://github.com/AizazSharif/Handwriting-Generation-Using-Recurrent-Neural-Networks).