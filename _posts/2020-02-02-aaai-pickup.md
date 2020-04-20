---
layout: post
title: Personal Pickup of AAAI 2020 Accepted Papers
description: This pickup mainly focuses on learning from weak supervision and pairwise comparison.
visible: True
---

As [AAAI 2020](https://aaai.org/Conferences/AAAI-20/)
[accepted list](https://aaai.org/Conferences/AAAI-20/wp-content/uploads/2020/01/AAAI-20-Accepted-Paper-List.pdf) is released and I have to prepare contents for a [seminar](https://twitter.com/breadhouse_semi),
I pick up some papers with (potentially) interesting problem settings.
My main focus is learning from weak supervision and pairwise comparison.

The collection is totally biased.
Papers are ordered by their paper ids.
As my emphasis is on the problem setting,
detailed experiment results are not shown in my slides,
since they should appear good anyway.

### [Comparing Election Methods Where Each Voter Ranks Only Few Candidates](https://arxiv.org/abs/1901.10848)
TL; DR: A new weakly-supervised election voting problem setting is proposed with theoretically guaranteed algorithms.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vR7xMsjLiyPr-rfAXShn8LGRbxnIX74mvSoqL6FGpbKv5NDF_CTZYrm5tt9oEtGV2rQNPcaXMjjAgG1/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* This papers studies a general problem setting of election voting,
which is not covered by standard machine learning textbooks.
* This seems to be a primary weakly-supervised extension for the traditional problem setting,
much space left to be explore.

### [Pruning from Scratch](https://arxiv.org/abs/1909.12579)
TL; DR: An efficient pruning algorithm without pre-training.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vQYCtvIroLu2fQL35NSeb0DXaTX1WfwCXHPwIZkesstcdendBN2FI0-yERVK1dtd4pLRYu-BbMZI00a/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* [Weight Agnostic Neural Networks](https://nips.cc/Conferences/2019/ScheduleMultitrack?event=14530)
by Gaier et al. on NeurIPS 2019 already recognized the unnecessariness of weights.
* It may inspire other problems where people still think training is inevitable.

### [Exploiting Motion Information from Unlabeled Videos for Static Image Action Recognition](https://arxiv.org/abs/1912.00308)
TL; DR: A framework for image action recognition that also uses unlabeled video data.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vRQqj445JHy2On8O1MHbPa-QsWqhM0DOv_dZgNenxa9GQ6LnQNVGt9l9aTqjnlC92DTNY2lASk1ta73/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* Some parts of the proposed framework are still heuristic and not end-to-end,
etc., feature vectors for clustering.
* Learning image tasks from videos seems interesting,
as there are other accepted papers on weakly-supervised temporal action localization.
* It would be interesting to abstract the problem setting to a more general problem.

### [Weakly Supervised Disentanglement by Pairwise Similarities](https://arxiv.org/abs/1906.01044)
TL; DR: Disentanglement representation learning with similarity information.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vSGkn0wwqk6Prv4UXw-mfJD6Bj845J8aQHSPMavIwBiyAbR07Q87b_dF0aRJG5eTMqdVjkcMkRw_vRR/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* The arxiv version is in NeurIPS format, so there might be significant improvement for AAAI version.
* Giving originally unsupervised task weak supervision needs more motivation than giving originally fully supervised task only weak supervision.
* I am not sure how constraining the information into $z^{(u)}$ is connected to disentanglement.
* In practice, it might not be so easy to compare in the sense of a vector $z^{(u)}$,
which has more than one dimension.
And it is considered to be hard to give a real value rather than yes or no for comparison.

### [Online Active Learning of Reject Option Classifiers](https://arxiv.org/abs/1906.06166)
TL; DR: Streaming based active learning with abstention.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vRYVxqe9tYjc7qOmHXUaB7IoenWAIOKeT7RUo2sXn2NXAwSL4TKVrBO60FwwSkgVAlzj_Zo2IAQj0ce/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* The arxiv version is in NeurIPS format, so there might be significant improvement for AAAI version.
* The use of the two loss functions may need stronger motivation.
* Upper bounds on label complexity may be helpful.

### [Can We Predict the Election Outcome from Sampled Votes?](http://www.cs.toronto.edu/~nisarg/papers/samples.pdf)
TL; DR: Election problem when preference from only part of the voters are observed.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vShnjhTeeqaOOsnEwzN8QCaFusL74YrovJnsdufyua4jteRzVQ4kzDpesWUiz59S4kBRhINIHRGXTLI/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* This is a quite difficult problem since there are a part of voters whose preference is totally hidden.

### [Rank Aggregation via Heterogeneous Thurstone Preference Models](https://arxiv.org/abs/1912.01211)
TL; DR: Introducing a new parameter into the Thurstone model to deal with different noise level of labelers.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vSQCvXohR35TA0zH8yLlh-HigSQ3iSEtNSgCoduWvXKdZUy0q9b5g17SKG9-Dyjh0ko_Uq7hZAi0MTT/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* A simple and efficient improvement for the famous Thurstone model.

<style>
.responsive-wrap { width: 80%; margin: 0 auto; }
.responsive-wrap iframe{ max-width: 100%; }
</style>
