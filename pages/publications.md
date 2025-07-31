---
layout: default
---

## Publications

**[DIG-BUGS@ICML'25]**  
**In-Context Bias Propagation in LLM-Based Tabular Data Generation** [(arXiv)](https://arxiv.org/pdf/2506.09630)  
*Pol G. Recasens, Alberto Gutierrez, Jordi Torres, Josep Berral, Anisa Halimi, Kieran Fraser*

- <details>
  <summary><strong>Abstract</strong></summary>
  Large Language Models (LLMs) are increasingly used for synthetic tabular data generation through in-context learning (ICL), offering a practical solution for data augmentation in data-scarce scenarios. While prior work has shown their potential to improve downstream task performance by augmenting underrepresented groups, this often assumes access to an unbiased subset of in-context examples. In reality, data is frequently noisy and demographically skewed.  
  This paper systematically studies how statistical biases in in-context examples propagate to the synthetic data distribution, demonstrating that even mild biases cause global distortions. We also present an adversarial scenario where malicious actors can inject bias through selected in-context examples, compromising fairness for targeted subgroups. These findings expose a new vulnerability in LLM-based data generation pipelines used in sensitive domains.
  </details>

**[CLOUD'25]**  
**Mind the Memory Gap: Unveiling GPU Bottlenecks in Large-Batch LLM Inference** [(arXiv)](https://arxiv.org/pdf/2503.08311)  
*Pol G. Recasens, Ferran Agulló, Yue Zhu, Chen Wang, Eun Kyung Lee, Olivier Tardieu, Jordi Torres, Josep Ll. Berral*

- <details>
  <summary><strong>Abstract</strong></summary>
  While batching is commonly used to improve LLM inference throughput, performance gains tend to plateau with large batch sizes. Contrary to the prevailing belief that this is due to compute-bound behavior, our GPU-level analysis shows that inference remains memory-bound, with DRAM bandwidth saturation being the limiting factor.  
  We introduce a Batching Configuration Advisor (BCA) that optimizes memory allocation, reducing GPU usage without significantly harming throughput. Freed-up memory and compute capacity can then be utilized by concurrent workloads through model replication, improving GPU utilization. Our findings challenge established assumptions and offer actionable strategies for optimizing small LLM deployment.
  </details>

**[EuroMLSys'24]**  
**Towards Pareto Optimal Throughput in Small Language Model Serving** [(arXiv)](https://arxiv.org/pdf/2404.03353)  
*Pol G. Recasens, Yue Zhu, Chen Wang, Eun Kyung Lee, Olivier Tardieu, Alaa Youssef, Jordi Torres, Josep Ll. Berral*

- <details>
  <summary><strong>Abstract</strong></summary>
  The growing popularity of Small Language Models (SLMs) presents a promising alternative to large-scale LLMs in resource-constrained environments. In this paper, we benchmark SLM inference in terms of both performance and energy efficiency.  
  Our findings reveal that SLMs' smaller memory footprint enables serving them near the Pareto-optimal point on a single GPU. Furthermore, we show how model replication can be leveraged to boost serving throughput and resource utilization, providing practical strategies for efficient SLM deployment.
  </details>

**[FL-FM@NeurIPS'23]**  
**On Masked Pre-training and the Marginal Likelihood** [(OpenReview)](https://openreview.net/pdf?id=sPtEDSVD4K)  
*Pol G. Recasens, Jordi Torres, Josep Ll. Berral, Søren Hauberg, Pablo Moreno-Muñoz*

- <details>
  <summary><strong>Abstract</strong></summary>
  The high cost of training large foundation models has increased interest in federated learning and model reuse. This paper introduces *self-supervised Fisher merging*, a Bayesian approach that allows parameter-space model aggregation without data access.  
  Our method opens the door to collaborative model reuse while maintaining privacy. Experimental results demonstrate theoretical soundness on tractable models and potential for neural network aggregation, offering a practical route to data-free model composition.
  </details>

**[NeurIPS'23]**  
**On Masked Pre-training and the Marginal Likelihood** [(arXiv)](https://arxiv.org/pdf/2306.00520)  
*P. Moreno-Muñoz, P. G. Recasens, S. Hauberg*

- <details>
  <summary><strong>Abstract</strong></summary>
  Masked pre-training removes parts of the input and trains models to predict the missing content—a form of self-supervision that leads to strong generalization across domains.  
  This paper provides a theoretical framework showing that masked pre-training aligns with maximizing marginal likelihood—a Bayesian measure of generalization. We validate the theory empirically and provide insights into why and how masked pre-training works, especially for large-scale models.
  </details>