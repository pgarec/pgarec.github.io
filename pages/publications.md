---
layout: default
---

## Publications

**[DIG-BUGS@ICML'25]** In-Context Bias Propagation in LLM-Based Tabular Data Generation [(arXiv)](https://arxiv.org/pdf/2506.09630?)  
Pol G Recasens, Alberto Gutierrez, Jordi Torres, Josep Berral, Anisa Halimi, Kieran Fraser

<details>
<summary><strong>Abstract</strong></summary>
Large Language Models (LLMs) are increasingly used for synthetic tabular data generation through in-context learning (ICL), offering a practical solution for data augmentation in data scarce scenarios. While prior work has shown the potential of LLMs to improve downstream task performance through augmenting underrepresented groups, these benefits often assume access to a subset of unbiased in-context examples, representative of the real dataset. In real-world settings, however, data is frequently noisy and demographically skewed. In this paper, we systematically study how statistical biases within in-context examples propagate to the distribution of synthetic tabular data, showing that even mild in-context biases lead to global statistical distortions. We further introduce an adversarial scenario where a malicious contributor can inject bias into the synthetic dataset via a subset of in-context examples, ultimately compromising the fairness of downstream classifiers for a targeted and protected subgroup. Our findings demonstrate a new vulnerability associated with LLM-based data generation pipelines that rely on in-context prompts with in sensitive domains.
</details>

**[CLOUD'25]** Mind the Memory Gap: Unveiling GPU Bottlenecks in Large-Batch LLM Inference [(arXiv)](https://arxiv.org/pdf/2503.08311)  
Pol G Recasens, Ferran Agullo, Yue Zhu, Chen Wang, Eun Kyung Lee, Olivier Tardieu, Jordi Torres, Josep Ll Berral  

<details>
<summary><strong>Abstract</strong></summary>
Large language models have been widely adopted across different tasks, but their auto-regressive generation nature often leads to inefficient resource utilization during inference. While batching is commonly used to increase throughput, performance gains plateau beyond a certain batch size, especially with smaller models, a phenomenon that existing literature typically explains as a shift to the compute-bound regime. In this paper, through an in-depth GPU-level analysis, we reveal that large-batch inference remains memory-bound, with most GPU compute capabilities underutilized due to DRAM bandwidth saturation as the primary bottleneck. To address this, we propose a Batching Configuration Advisor (BCA) that optimizes memory allocation, reducing GPU memory requirements with minimal impact on throughput. The freed memory and underutilized GPU compute capabilities can then be leveraged by concurrent workloads. Specifically, we use model replication to improve serving throughput and GPU utilization. Our findings challenge conventional assumptions about LLM inference, offering new insights and practical strategies for improving resource utilization, particularly for smaller language models.
</details>

**[EuroMLSys'24]** Towards Pareto Optimal Throughput in Small Language Model Serving [(arXiv)](https://arxiv.org/pdf/2404.03353)  
Pol G Recasens, Yue Zhu, Chen Wang, Eun Kyung Lee, Olivier Tardieu, Alaa Youssef, Jordi Torres, Josep Ll Berral  

<details>
<summary><strong>Abstract</strong></summary>
Large language models (LLMs) have revolutionized the state-of-the-art of many different natural language processing tasks. Although serving LLMs is computationally and memory demanding, the rise of Small Language Models (SLMs) offers new opportunities for resource-constrained users, who now are able to serve small models with cutting-edge performance. In this paper, we present a set of experiments designed to benchmark SLM inference at performance and energy levels. Our analysis provides a new perspective in serving, highlighting that the small memory footprint of SLMs allows for reaching the Pareto-optimal throughput within the resource capacity of a single accelerator. In this regard, we present an initial set of findings demonstrating how model replication can effectively improve resource utilization for serving SLMs.
</details>

**[FL-FM@NeurIPS'23]** On masked pre-training and the marginal likelihood [(OpenReview)](https://openreview.net/pdf?id=sPtEDSVD4K)  
Pol G Recasens, Jordi Torres, Josep Lluis Berral, Søren Hauberg, Pablo Moreno-Muñoz

<details>
<summary><strong>Abstract</strong></summary>
The success of foundation models is strongly linked to scale, which has reinforced the interest in federated learning. With the prohibitive cost of training a large language model (LLM) in mind, little attention has been placed on reusing pre-trained models in collaborative training settings. Self-supervision has also played an important role in this success, but its emphasis has been primarily on data. This paper leverages Bayesian principles to bring self-supervision into the model aggregation toolbox. It introduces self-supervised Fisher merging, a framework that successfully merges models in parameter space without re-visiting data, opening a new door in model reusability. Experimental results build the foundation of our method on tractable linear models, and highlight its potential on aggregating neural networks.
</details>

**[NeurIPS'23]** On masked pre-training and the marginal likelihood [(arXiv)](https://arxiv.org/pdf/2306.00520)  
P Moreno-Muñoz, P Garcia Recasens, S Hauberg  

<details>
<summary><strong>Abstract</strong></summary>
Masked pre-training removes random input dimensions and learns a model that can predict the missing values. Empirical results indicate that this intuitive form of self-supervised learning yields models that generalize very well to new domains. A theoretical understanding is, however, lacking. This paper shows that masked pre-training with a suitable cumulative scoring function corresponds to maximizing the model's marginal likelihood, which is de facto the Bayesian model selection measure of generalization. Beyond shedding light on the success of masked pre-training, this insight also suggests that Bayesian models can be trained with appropriately designed self-supervision. Empirically, we confirm the developed theory and explore the main learning principles of masked pre-training in large language models.
</details>
