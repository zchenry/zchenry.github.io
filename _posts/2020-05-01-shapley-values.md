---
layout: post
title: A Series of Work on Data Shapley Value
description: This article introduces three papers that apply a concept from game theory to machine learning.
visible: True
---

Determining data values in a principled way is an interesting research topic
and has profound influence on applications.
As I prepared presentation content for a [seminar](https://twitter.com/breadhouse_semi),
I pick up three papers on applying Shapley value,
a concept from cooperative game theory,
into the field of machine learning.
They are first-authored by a same researcher.

### [Data Shapley: Equitable Valuation of Data for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html)
TL; DR: This paper introduces a new way to define data values.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vQfNoUPloBqekUUcqokQ20VgjpGWXEzHzwPL95ZNhZXz2TTbnSU77AwESXgM5mE8HRnTmZvJDbv5fNL/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* The third property seems not essential and only serves to simplify the proof.
* Theories on convergence of the approximation methods would make the paper more persuasive.
* It would be interesting to explore its application on other fields like active learning and coresets.

### [Neuron Shapley: Discovering the Responsible Neurons](https://arxiv.org/abs/2002.09815)
TL; DR: Applying the above introduced data Shapley value into the task of evaluating neuron importance in a neural network.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vRM_qk9nUCXPTPUC5GA_vJNjPbmxmZxmkK0b_CLsUDjZOYguGRRzWn_SOUx7FbLiMpSt5hONDSquIaE/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* This paper differs the above paper only on the approximation method and the application.
* It would be interesting to apply this method on validating lottery ticket hypothesis.

### [A Distributional Framework for Data Valuation](https://arxiv.org/abs/2002.12334)
TL; DR: This paper extends the definition of the data Shapley value.
<div class='responsive-wrap'>
<iframe src='https://docs.google.com/presentation/d/e/2PACX-1vTjX6TxPCUwG-Z-eP9OJ2lES2M149hMgkKVTcHsygVbvDvCC7Sey9dF8OCMyd0AXuKzP2lAu6i8nfdY/embed?start=false&loop=false&delayms=6000000' frameborder='0' width='640' height='510' allowfullscreen='true' mozallowfullscreen='true' webkitallowfullscreen='true'></iframe>
</div>
#### My Thoughts
* The idea is simple, just taking an expectation.
* The theories are introduced in an intuitive and clear way.
* I wonder what is the next step for authors.

<style>
.responsive-wrap { width: 80%; margin: 0 auto; }
.responsive-wrap iframe{ max-width: 100%; }
</style>
