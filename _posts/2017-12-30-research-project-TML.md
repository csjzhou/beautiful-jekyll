---
layout: post
title: Transparent Machine Learning
tags:
  - professional
  - research-project
date: 'Sat Dec 30 2017 11:00:00 GMT+1100 (AUS Eastern Standard Time)'
published: true
---

## Background

Machine Learning (ML) is currently facing prolonged challenges with the user acceptance of delivered solutions as well as 
seeing system misuse, disuse, or even failure. Significant barriers to the adoption of ML approaches exist in the areas 
of trust (of ML results), comprehension (of ML processes) and related workload, as well as confidence 
(in decision making based on ML results) by users. These fundamental challenges can be attributed to 
the nature of ``black-box'' of ML for domain users when offering ML-based solutions.

Therefore, besides the development of ML algorithms, research of introducing human into the ML loop (human-in-the-loop ML) 
and making ML transparent is emerging as one of active research fields recently. Other terms are also used to refer to such
researches, e.g. human interpretability in machine learning, or explainable artificial intelligence (XAI). 
We use Transparent Machine Learning (TML) in our context. TML aims to translate ML into impacts by allowing domain users 
understand data-driven inferences to make trustworthy decisions confidently based on ML results, and letting ML accessible 
by domain users without requiring training in complex ML algorithms and mathematical concepts. TML results in evolutionary 
improvements of the existing state of practice, for example,

- TML not only helps domain users proactively use ML outputs for informative and trustworthy decision making, but also allows users to see if an artificial intelligence system is working as desired;
- TML can help detect causes for an adverse decision and therefore can provide guidance on how to reverse it;
- TML allows effective interactions with ML algorithms, thus provides opportunities to improve impact of ML algorithms in real-world applications.

## Technologies

We propose the following approaches:
- ***2D Transparency Space***: a framework integrating both ML experts and domain users as active participants into the overall workflow of ML-based solutions.
- ***DecisionMind***: a pipeline revealing human cognition states ML-based decision making with multimodal interfaces.
