---
layout: page
title: Projects
subtitle: The projects I worked on.
meta-title: Mert Kosan - Projects
---

## Global Counterfactual Explainer for Graph Neural Networks
Period: September 2021 - September 2022<br>
Location: [UC Santa Barbara - Dynamo](https://dynamo.cs.ucsb.edu/)

> Global Counterfactual Explainer for Graph Neural Networks.<br>
> Mert Kosan*, Zexi Huang*, Sourav Medya, Sayan Ranu, Ambuj Singh.<br>
> ACM International Conference on Web Search and Data Mining, 2023 (WSDM'23).

Published at: [WSDM'23](https://www.wsdm-conference.org/2023/) <br>
Paper: [https://dl.acm.org/doi/10.1145/3539597.3570376](https://dl.acm.org/doi/10.1145/3539597.3570376) <br>
Code and Data: [https://github.com/mertkosan/GCFExplainer](https://github.com/mertkosan/GCFExplainer)

One way to address the explainability problem in graph neural networks (GNNs) is counterfactual reasoning, where the objective is to change the GNN prediction by minimal changes in the input graph. Existing methods for the counterfactual explanation of GNNs are limited to
instance-specific local reasoning. In this work, we study a novel problem; the global explainability of GNNs through global counterfactual reasoning. Specifically, we want to find a small set of representative counterfactual graphs that explains all
input graphs. Drug discovery is one of the main applications of this work.

<!--
![](/img/gcfexplainer_case_study.png)
-->

<p align="center" width="100%">
    <img width="75%" src="/img/gcfexplainer_case_study.png">
</p>

Figure: Illustration of global and local counterfactual explanations for the AIDS dataset. The global counterfactual graph (c) presents a high-level recourse rule—changing ketones and ethers into aldehydes (shown in blue)—to combat HIV,
while the edge removals (shown in red) recommended by local counterfactual examples (b) are hard to generalize.

## AI Decision Systems with Feedback Loop Active Learner
Period: June 2022 - August 2022
Location [Visa Research - Austin](https://usa.visa.com/)

> AI Decision Systems with Feedback Loop Active Learner.<br>
> Mert Kosan, Linyun He, Shubham Agrawal, Hongyi Liu, Chiranjeet Chetia.<br>
> CANDLE: Collaboration of Humans and Learning Algorithms for Data Labeling. WSDM 2023 Crowd Science Workshop.

Published at: [WSDM'23](https://www.wsdm-conference.org/2023/) <br>
Paper: [https://ceur-ws.org/Vol-3357/paper2.pdf](https://ceur-ws.org/Vol-3357/paper2.pdf) <br>

The paper addresses the limitation of the collaboration of AI decision systems and human labelers in human-in-the-loop systems. Our framework aims for better ground-truth labeling by learning the interests/expertise
of human labelers using active-learning.

![](/img/flal_framework.png)

Figure: Feedback Loop Active Learner steps. (1) It starts with embedding stream data using pre-trained embedders. (2) User embedding mapper maps the embedding space into a more personalized space. (3) Feature extractor generates learned
or expert-designed features to tackle the cold-start problem for recommenders. (4) Generates relevance scores based on AI decision system and extracted features. It sends queries to users for ground truth generation. (5) User generates
ground truths and relevancy of the query. They send them back to the framework. Later, FLAL updates its components using an active learning mechanism and keeps ground truth information for future updates on the AI decision system. Notice
that the user’s interest (relevancy) in queries can also be inferred using interaction detectors.

## Event Detection on Dynamic Networks
Period: September 2018 - September 2020<br>
Location: [UC Santa Barbara - Dynamo](https://dynamo.cs.ucsb.edu/)

> Event Detection on Dynamic Graphs.<br>
> Mert Kosan, Arlei Silva, Sourav Medya, Brian Uzzi, Ambuj Singh.<br>
> Deep Learning on Graphs: Method and Applications, Association for the Advancement of Artificial Intelligence 2023 (DLG-AAAI’23).

Published at: [DLG-AAAI'23](https://deep-learning-graphs.bitbucket.io/dlg-aaai23/) <br>
Paper: [https://arxiv.org/abs/2110.12148](https://arxiv.org/abs/2110.12148) <br>
Code and Data: [https://github.com/mertkosan/DyGED](https://github.com/mertkosan/DyGED)

We propose DyGED, a simple yet novel deep learning model for event detection on dynamic graphs. DyGED learns correlations between the graph macro dynamics—i.e. a sequence of graph-level representations and labeled events. Our framework consists of
dynamic graph neural networks further enhanced by structural and temporal self-attention.  We tested our method on multiple datasets comparing multiple competing baselines, and outperformed them by up to 8.5% while being more scalable than the top alternatives.

<!--
A figure below illustrates (a) event detection on dynamic graphs based on a generic deep learning architecture. (b) At the micro scale, the dynamics is captured at node level using a temporal GNN architecture and then pooled for graph-level classification.
(c) At the macro scale, the dynamics is captured at the graph level using an RNN over pooled (static) GNN node embeddings. Our work investigates how the dynamics at different scales affects event detection performance.
![Event Detection Summary Figure](/img/ed_figure_new.png)
-->

![](/img/DLG-AAAI23%20Poster.png)
[Poster's PDF version](/docs/DLG-AAAI23%20Poster.pdf)
