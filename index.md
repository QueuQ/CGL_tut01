---
layout: default
---

## Abstract
Over the past years, deep learning on graphs has made significant progress in various areas. However, most graph learning tasks assume graphs are static, while real-world graphs may constantly grow or evolve. Therefore, it is crucial to study how to constantly adapt a graph learning model to new patterns/tasks over graphs without forgetting the previously learned knowledge. To this end, in this tutorial, we will introduce the newly emerging area of continual graph learning (CGL). Specifically, we will (1) introduce different continual graph learning settings, (2) present the key challenges in CGL, (3) highlight the existing CGL techniques, and (4) discuss future directions.
The length of this tutorial will be 3 hours, including a 150 minutes presentation and 30 minutes Q&A.

## Introduction
Real-world graphs are often continuously growing or evolving. For example, new types of papers may be constantly added to a citation network, and a document classifier is expected to continuously adapt and be capable of classifying the new types of papers. In drug design research, molecules with new types of properties may be continuously encountered, and a molecule property predictor has to keep learning the new molecule properties. Existing graph learning models are good at learning new patterns/tasks. However, the high plasticity also brings the catastrophic forgetting problem, which refers to the drastic performance drop on previously learned tasks after the model has learned new tasks. To this end, CGL is attracting increasingly more attention recently, and therefore will be thoroughly discussed in this tutorial. 

Due to the complex forms of graph data from different areas, we will first introduce the formal setting of CGL. Specifically, we will explain the node-level tasks and graph-level tasks under both task-incremental (task-IL) and class-incremental (class-IL) scenarios. Then, based on these settings, we will introduce the key challenges of the CGL, as well as the difference compared to traditional continual learning on independent data (e.g. images). Next, we will introduce the existing methods, including both the methods specially developed for CGL, and the traditional continual learning methods that are applicable to CGL. Finally, after analyzing the advantages and disadvantages of the existing methods, we will point out the unresolved challenges, as well as future research directions.

## Tutorial Outline
* Introduction

Real-world graphs are often continuously growing or evolving. For example, new types of papers may be constantly added to a citation network, and a document classifier is expected to continuously adapt and be capable of classifying the new types of papers. In social networks, new communities of people may be constantly emerging. In drug design research, molecules with new types of properties may be continuously encountered, and a molecule property predictor has to keep learning the new molecule properties. Existing graph learning models are good at learning new patterns/tasks. However, the high plasticity also brings the catastrophic forgetting problem, which refers to the drastic performance drop on previously learned tasks after the model has learned new tasks. To this end, CGL is attracting increasingly more attention recently, and therefore will be thoroughly discussed in this tutorial. 

Due to the complex forms of graph data from different areas, we will first introduce the formal setting of CGL. Specifically, we will explain the node-level tasks and graph-level tasks under both task-incremental (task-IL) and class-incremental (class-IL) scenarios. Then, based on these settings, we will introduce the key challenges of the CGL, as well as the difference compared to traditional continual learning on independent data (e.g. images). Next, we will introduce the existing methods, including both the methods specially developed for CGL, and the traditional continual learning methods that are applicable to CGL. Finally, after analyzing the advantages and disadvantages of the existing methods, we will point out the unresolved challenges, as well as future research directions.

* Formulation of the CGL Tasks & Challenges

To introduce the problem setting of CGL, we will start from the setting of the traditional continual learning. Then, based on the difference between graph data and the independent data in traditional continual learning, we introduce the different CGL settings including both node-level tasks and graph-level tasks under both task-IL and class-IL scenarios. The problem formulation directly comes from our recent work on benchmarking the CGL methods. With the specific settings, we will compare CGL and traditional continual learning to highlight the unique challenges and difference in CGL.


* Reviews on Existing Methods

The introduction on the existing methods contains two parts. First, we will introduce the techniques that are not developed for CGL but can be adapted for CGL, like Elastic Weight Consolidation (EWC), Learning without Forgetting~(LwF), Gradient Episodic Memory~(GEM), Memory Aware Synapses~(MAS), etc.. Next, we will introduce methods that are specially developed for CGL, including Experience Replay based GNN~(ERGNN), Topology-aware Weight Preserving~(TWP), Hierarchical Prototype Networks~(HPNs), and Sparsified Subgraph Memory (SSM). We will also demonstrate the performance of these methods under different CGL settings. Among the methods, Hierarchical Prototype Networks~(HPNs) is our recent work, and the performance of these methods are obtained from our benchmark work (CGLB).

* Future Directions

With the performance comparisons, we will analyze the advantages and disadvantages of the existing models. Besides, the experimental results also reveal the unresolved challenges. Accordingly, we will further point out the directions for future investigation on the CGL problem, and the development of new models. 

## What will the participants learn from the tutorial?

Since graphs that are continuously growing or evolving are common in various real-world applications, e.g.,  social networks, drug discovery, recommender systems, etc., this tutorial about CGL will attract audiences from broad areas and trigger their interest in applying related methods or developing more advanced techniques in this direction. Participants may also extend CGL to more practical or complex scenarios. Besides, CGL may interest a number of researchers on network science, because the grwoing graph (network) setting is very realistic in network science researches and the accompanying techniques are highly valuable.


## Tutors

* Xikun Zhang is Ph.D. student at the School of Computer Science in The University of Sydney. His research interests mainly include applying deep learning to tackle graph related problems, which is closely related to the topic of this tutorial. His works have been published in top conferences and journals, such as NeurIPS, TPAMI, ICDM, CVPR, ECCV, and TNNLS. 
Email: xzha0505@uni.sydney.edu.au



* Dongjin Song is an assistant professor in the Department of Computer Science and Engineering at the University of Connecticut (UConn). His research interests include machine learning, deep learning, data mining, and related applications for time series data and graph representation learning. Papers describing his research have been published at top-tier data science and artificial intelligence conferences, such as NeurIPS, ICML, ICLR, KDD, ICDM, SDM,  AAAI, IJCAI, CVPR, ICCV, etc. He has served as PC chairs for AI for Time Series (AI4TS) workshop at IJCAI 2022 and the Mining and Learning from Time Series workshop at KDD 2022. He has also served as senior PC members for AAAI, IJCAI, and CIKM. He won the UConn Research Excellence Research (REP) Award in 2021.
Email: dongjin.song@uconn.edu


* Dacheng Tao (Fellow, IEEE) is currently a Professor of Computer Science and an ARC Laureate Fellow in the School of Computer Science and the Faculty of Engineering at The University of Sydney. He mainly applies statistics and mathematics to artificial intelligence and data science. His research is detailed in one monograph and over 200 publications in prestigious journals and proceedings at prominent conferences such as IEEE TPAMI, IJCV, JMLR, NeurIPS, ICML, ICLR, CVPR, ICCV, ECCV, AAAI, IJCAI, ICDM and ACM SIGKDD, with several best paper awards, such as the Best Theory/Algorithm Paper Runner Up Award at IEEE ICDM’07, the Distinguished Paper Award at 2018 IJCAI, the 2014 ICDM 10-year Highest-Impact Paper Award, and the 2017 IEEE Signal Processing Society Best Paper Award. He received the 2015 and 2020 Australian Eureka Prize and the 2018 IEEE ICDM Research Contributions Award. He is a fellow of the Australian Academy of Science, TWAS, AAAS, ACM and IEEE.
Email: dacheng.tao@gmail.com
