---
layout: page
title: Finished Projects
subtitle: The projects I worked on.
meta-title: Mert Kosan - Finished Projects
---

## Event Detection on Dynamic Networks
Period: September 2018 - September 2020  
Location: [UC Santa Barbara - Dynamo](https://dynamo.cs.ucsb.edu/)
Project Type: Research

We propose DyGED, a simple yet novel deep learning model for event detection on dynamic graphs. DyGED learns correlations between the graph macro dynamics—i.e. a sequence of graph-level representations and labeled events. Our framework consists of 
dynamic graph neural networks further enhanced by structural and temporal self-attention.  We tested our method on multiple datasets comparing multiple competing baselines, and outperformed them by up to 8.5% while being more scalable than the top alternatives.

A figure below illustrates (a) event detection on dynamic graphs based on a generic deep learning architecture. (b) At the micro scale, the dynamics is captured at node level using a temporal GNN architecture and then pooled for graph-level classification. 
(c) At the macro scale, the dynamics is captured at the graph level using an RNN over pooled (static) GNN node embeddings. Our work investigates how the dynamics at different scales affects event detection performance.

![Event Detection Summary Figure](/img/ed_figure_new.png)