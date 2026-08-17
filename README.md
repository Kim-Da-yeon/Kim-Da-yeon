## 김다연 · Dayeon Kim

Graduate student in Big Data Science at Korea University. I work on **Bayesian
computation** and **applied text modelling** — samplers that can actually reach
the modes of a hard posterior, and models whose structure matches how the data was
generated.

[Blog](https://kim-da-yeon.github.io/) · [dayun0405@gmail.com](mailto:dayun0405@gmail.com)

---

### Research

**[bntm-topic-model](https://github.com/Kim-Da-yeon/bntm-topic-model)** · *paper in preparation*
A sentence-level topic model that treats a document as a network of topic
transitions rather than an exchangeable mixture — which matters when documents are
genuinely sequential, like adverse-event reports or accident narratives. Logistic-normal
transition matrix and topic–word distributions, sparse Dirichlet on the global
weights so `K` is only an upper bound. Fitted with **AWSGHMC**, an adaptively
weighted stochastic-gradient HMC that flattens the energy landscape to cross
barriers between modes. Model and sampler are evaluated as separate claims, on
separate axes.

**[llmrec-metadata-standard](https://github.com/Kim-Da-yeon/llmrec-metadata-standard)**
LLMs emit free text, not controlled vocabulary, so the same country arrives as
`USA` / `United States` / `America`. Normalizing LLM-generated recommendation
metadata to ISO 3166-1 and BCP 47 took interoperability from **0 → 80.3%** and
collapsed 1,166 surface forms for a single country down to 57 canonical codes —
and, as a side effect, caught 724 column-shift errors the model had made. It did
*not* significantly improve recommendation accuracy across 10 seeds, and the
write-up says so.

**[GCIoU-SGMCMC-3D-Detection](https://github.com/Kim-Da-yeon/GCIoU-SGMCMC-3D-Detection)**
Do Bayesian samplers work as optimizers on a real 3D detector? SGLD / SGHMC /
SGNHT against Adam on PointPillars/KITTI under an identical GCIoU energy. Adam
wins by +31.4% BEV AP — and the sampler with the *lowest training loss* is not the
one that detects best, which is the part worth keeping.

### Systems and packages

**[SONY_Chatbot](https://github.com/Kim-Da-yeon/SONY_Chatbot)**
Korean retrieval-augmented QA over product manuals. `bge-m3` + Chroma retrieval
with page-level source attribution, KoAlpaca-7b generation, and a web-search
fallback when nothing survives product filtering.

**[mcmc-r-packages](https://github.com/Kim-Da-yeon/mcmc-r-packages)**
The same stochastic-approximation Monte Carlo sampler as an R package three times
over — pure R, C via Rcpp, Python via reticulate — plus a minimal NIMBLE example.
Useful mostly for what the side-by-side comparison exposed about the three
implementations.

**[Pykachu-Volleyball](https://github.com/Kim-Da-yeon/Pykachu-Volleyball)**
Tabular Q-learning on a reverse-engineered Pikachu Volleyball `gymnasium`
environment, with a dense reward reshaped for table-based learning. A good lesson
in what belongs in a state representation.

---

### Interests

Stochastic-gradient MCMC · multimodal posteriors · sequential and sentence-level
topic models · honest evaluation of LLM-generated data

<sub>Most repositories carry a Limitations section. They are not decoration — if a
result did not replicate, it says so there.</sub>
