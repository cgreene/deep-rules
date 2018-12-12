---
author-meta:
- Benjamin D. Lee
date-meta: '2018-12-12'
keywords:
- ten simple rules
- machine learning
- deep learning
- artificial intelligence
lang: en-US
title: Ten Simple Rules for Deep Learning in Biology
...






<small><em>
This manuscript
([permalink](https://Benjamin-Lee.github.io/deep-rules/v/b4a853c645372d9e49482f1342fcf274c0ccc173/))
was automatically generated
from [Benjamin-Lee/deep-rules@b4a853c](https://github.com/Benjamin-Lee/deep-rules/tree/b4a853c645372d9e49482f1342fcf274c0ccc173)
on December 12, 2018.
</em></small>

## Authors



+ **Benjamin D. Lee**<br>
    ![ORCID icon](images/orcid.svg){height="13px" width="13px"}
    [0000-0002-7133-8397](https://orcid.org/0000-0002-7133-8397)
    · ![GitHub icon](images/github.svg){height="13px" width="13px"}
    [Benjamin-Lee](https://github.com/Benjamin-Lee)<br>
  <small>
     School of Engineering and Applied Sciences, Harvard University; Department of Genetics, Harvard Medical School; Lab41, In-Q-Tel
  </small>



## Introduction

Deep learning (DL), a subfield of machine learning (ML) that focuses on deep artificial neural networks, is exploding in popularity and is increasingly being used for biological data analysis [@PZMP42Ak].
However, DL itself remains an active area of research, and the complexity of this field poses a large barrier of entry to those who would like to correctly utilize state-of-the-art DL technology in biological research applications.
While much has been written about the impressive results of DL in biology, there is a comparative dearth of literature articulating best practices for its use, with most instructional literature focusing on ML, rather than DL [@p4Nl5If0].

To fix this problem, we solicited input from a diverse community of researchers, who wrote this manuscript collaboratively using the GitHub version control platform [@6XC2t354] and Manubot [@1GGGHdsew].
In the course of our discussions, several themes became clear: the importance of understanding and applying ML fundamentals as a baseline for utilizing DL, the necessity for extensive model comparisons and careful evaluation, and the need for critical thought in interpreting results generated by means of DL, among others.
Ultmately, the rules we established range from high-level guidance to the implementation of best practices, and it is our hope that they will provide actionable, DL-specific advice for both new and experienced DL practitioners alike who would like to employ DL in biological research.
By increasing the accessibility of DL techniques to biology, we aim to improve the overall quality and reproducibility of DL in the literature, enabling these powerful methods to be properly utilized to generate new scientific insights.


## Rule 1: Concepts that apply to machine learning also apply to deep learning



## Rule 2: Use traditional methods to establish performance baselines


## Rule 3: Understand the complexities of training deep neural networks


## Rule 4: Know your data and your question


## Rule 5: Choose an appropriate neural network architecture and data representation


## Rule 6: Tune your hyperparameters extensively and systematically


## Rule 7: Address deep neural networks' increased tendency to overfit the dataset


## Rule 8: Do not necessarily consider a DL model as a black box


## Rule 9: Interpret predictions in the correct manner


## Rule 10: Don't share models trained on sensitive data

One of the greatest opportunities for deep learning in biology is the ability for deep learning techniques to incorporate representation learning to extract information that can not readily be captured by traditional methods [@UeE0s74F]. 
The abundance of features for each training example means that the representation learning of the deep learning models can capture information-rich abstractions of data during the training process. Therefore with deep learning, and even with some traditional machine learning models such as k-nearest neighbors which stores the full training data, it is important not to share models trained on sensitive data.
Applying deep learning to images of cats from the internet does not pose a significant privacy problems, but in the field of human health, this starts to approach privacy concerns. 
Adversarial training techniques, such as model inversion attacks, can be used to exploit model predictions to recover recognizable images of people's faces used for training [@zCqhgXvY]. 
These risks are higher in deep learning compared to traditional machine learning techniques because of the greater representational capacity of the models. 
This is achieved by the high volume of model weights, even in a relatively small project, that allow deep learning to model high-dimensional non-linear relationships among data. 
This enhanced modeling capacity allows the model to learn more robust and nuanced features of specific data, leading to the chance of revealing the underlying sensitive data. 
When you train deep learning models on sensitive data, be sure not to share the model weights directly, and use privacy preserving techniques [@1HuQe3Z8X] such as differential privacy [@LiCxcgZp, @eJgWbXRz] and homomorphic encryption [@me326jb9, @3326vtLW] to protect sensitive data.



## Conclusion


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>