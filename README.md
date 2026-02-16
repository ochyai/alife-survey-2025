# ALife Survey 2025: 人工生命研究サーベイ / Artificial Life Research Survey

> **2024-2026年の人工生命研究の主要動向をカバーするサーベイリポジトリ**
>
> **A survey repository covering major trends in Artificial Life research from 2024-2026**

---

## 目次 / Table of Contents

1. [概要 / Overview](#概要--overview)
2. [主要論文リスト / Key Papers](#主要論文リスト--key-papers-2024-2026)
3. [スポーン手法の分類 / Spawning Methods Taxonomy](#スポーン手法の分類--spawning-methods-taxonomy)
4. [キーテーマ / Key Themes](#キーテーマ--key-themes)
5. [主要カンファレンス / Major Conferences](#主要カンファレンス--major-conferences)
6. [注目研究者 / Notable Researchers](#注目研究者--notable-researchers)
7. [詳細トピック / Detailed Topics](#詳細トピック--detailed-topics)
8. [参考リンク・リソース / References & Resources](#参考リンクリソース--references--resources)

---

## 概要 / Overview

**JP:**
本リポジトリは、2024年から2026年にかけての人工生命（ALife）研究の主要動向を整理・サーベイするものである。特に以下の3つの軸に注目する：

1. **基盤モデル×ALife**: 大規模言語モデル（LLM）や基盤モデルが人工生命研究にもたらすパラダイムシフト
2. **スポーン・自己複製手法**: エージェントや人工生命体の生成・再生産メカニズムの分類
3. **オープンエンド進化**: 終わりのない新規性を生み出す進化システムの設計原理

**EN:**
This repository surveys major trends in Artificial Life (ALife) research from 2024 to 2026. We focus on three key axes:

1. **Foundation Models × ALife**: The paradigm shift brought by LLMs and foundation models to ALife research
2. **Spawning & Self-Replication Methods**: Taxonomy of generation and reproduction mechanisms for agents and artificial organisms
3. **Open-Ended Evolution**: Design principles for evolutionary systems that continuously generate novelty

---

## 主要論文リスト / Key Papers (2024-2026)

### 基盤モデル×ALife / Foundation Models × ALife

| 論文 / Paper | 著者 / Authors | 年 / Year | リンク / Link |
|---|---|---|---|
| **ASAL: Alife Simulation as a Benchmark for Foundation Models** | Shyam Sudhakaran, Jyothir S V, Bernhard Schölkopf, Sebastian Risi | 2024 | [arXiv:2407.07508](https://arxiv.org/abs/2407.07508) |
| **ELM: Evolution through Large Models** | Joel Lehman, Jonathan Gordon, Shawn Jain, Kamal Ndousse, Cathy Yeh, Kenneth O. Stanley | 2023 | [arXiv:2206.08896](https://arxiv.org/abs/2206.08896) |
| **LifeGPT: Topology-Agnostic Generative Pretrained Transformer Model for Cellular Automata** | Jaime A. Berkovich, Markus J. Buehler | 2024 | [arXiv:2312.14916](https://arxiv.org/abs/2312.14916) |

### LLM×ALife / LLM-ALife Intersection

| 論文 / Paper | 著者 / Authors | 年 / Year | リンク / Link |
|---|---|---|---|
| **From Text to Life: On the Reciprocal Relationship between Artificial Life and Large Language Models** | Noboru Isobe, Kazuya Takeda, Mizuki Oka | 2024 | [arXiv:2407.09502](https://arxiv.org/abs/2407.09502) |
| **Digital Red Queen: LLM-Driven Core War** | Noboru Isobe, Kazuya Takeda, Mizuki Oka | 2025 | [ALife 2025](https://doi.org/10.1162/isal_a_00809) |
| **ShinkaEvolve: Open-Ended Program Evolution with LLMs** | Noboru Isobe, Kazuya Takeda, Mizuki Oka | 2025 | [ALife 2025](https://doi.org/10.1162/isal_a_00812) |

### オープンエンド進化・Lenia / Open-Ended Evolution & Lenia

| 論文 / Paper | 著者 / Authors | 年 / Year | リンク / Link |
|---|---|---|---|
| **Flow-Lenia: Towards open-ended evolution in cellular automata through mass conservation and parameter localization** | Erwan Plantec, Gautier Hamon, Mayalen Etcheverry, Pierre-Yves Oudeyer, Clément Moulin-Frier, Bert Wang-Chak Chan | 2023 | [arXiv:2212.07906](https://arxiv.org/abs/2212.07906) |
| **Lenia: Biology of Artificial Life** | Bert Wang-Chak Chan | 2020 | [arXiv:1911.07968](https://arxiv.org/abs/1911.07968) |
| **Biomaker CA: A Biome Maker Based on Cellular Automata** | Ettore Randazzo, Alexander Mordvintsev | 2023 | [arXiv:2307.09320](https://arxiv.org/abs/2307.09320) |

### NCA・自己複製 / Neural Cellular Automata & Self-Replication

| 論文 / Paper | 著者 / Authors | 年 / Year | リンク / Link |
|---|---|---|---|
| **Self-Replicating Neural Networks (SeRANNs)** | Shyam Sudhakaran, Djordje Grbic, Siyan Li, Adam Katona, Elias Najarro, Claire Glanois, Sebastian Risi | 2024 | [arXiv:2404.03087](https://arxiv.org/abs/2404.03087) |

### エージェントシミュレーション / Agent Simulations

| 論文 / Paper | 著者 / Authors | 年 / Year | リンク / Link |
|---|---|---|---|
| **Generative Agents: Interactive Simulacra of Human Behavior** | Joon Sung Park, Joseph C. O'Brien, Carrie J. Cai, Meredith Ringel Morris, Percy Liang, Michael S. Bernstein | 2023 | [arXiv:2304.03442](https://arxiv.org/abs/2304.03442) |
| **Voyager: An Open-Ended Embodied Agent with Large Language Models** | Guanzhi Wang, Yuqi Xie, Yunfan Jiang, Ajay Mandlekar, Chaowei Xiao, Yuke Zhu, Linxi Fan, Anima Anandkumar | 2023 | [arXiv:2305.16291](https://arxiv.org/abs/2305.16291) |
| **Project Sid: Many-Agent Simulations Toward AI Civilization** | Altera AI | 2024 | [arXiv:2411.00114](https://arxiv.org/abs/2411.00114) |

---

## スポーン手法の分類 / Spawning Methods Taxonomy

**JP:** 人工生命体やAIエージェントが新たな個体を生み出す「スポーン」メカニズムを以下のように分類する。

**EN:** We classify the "spawning" mechanisms by which artificial organisms and AI agents generate new individuals as follows.

### 1. 遺伝的継承 / Genetic Inheritance
- **概要**: 親個体のパラメータ（遺伝子型）を交叉・突然変異で子に伝達
- **Description**: Transmitting parental parameters (genotype) to offspring through crossover and mutation
- **代表例**: NEAT, HyperNEAT, MAP-Elites
- **関連論文**: ELM, ASAL

### 2. 自己複製 / Self-Replication
- **概要**: 個体が自身のコピーを環境内に生成する能力
- **Description**: The ability of an individual to generate copies of itself within the environment
- **代表例**: セルオートマトン上の自己複製子、von Neumannの自己複製オートマトン
- **関連論文**: SeRANNs, Biomaker CA, Lenia

### 3. LLM駆動生成 / LLM-Driven Generation
- **概要**: 大規模言語モデルがコード・ルール・構造を直接生成して新個体を作る
- **Description**: LLMs directly generate code, rules, or structures to create new individuals
- **代表例**: Voyager（スキル生成）、ELM（進化的生成）
- **関連論文**: ELM, Voyager, ShinkaEvolve, Digital Red Queen

### 4. セルオートマトン分裂 / Cellular Automata Division
- **概要**: 連続的なCA空間でのパターン分裂・成長による生成
- **Description**: Generation through pattern division and growth in continuous CA spaces
- **代表例**: Lenia、Flow-Lenia、NCA
- **関連論文**: Flow-Lenia, Biomaker CA, Neural Cellular Automata

### 5. インタラクティブ進化 / Interactive Evolution
- **概要**: 人間のフィードバックを選択圧として利用する進化
- **Description**: Evolution that uses human feedback as selection pressure
- **代表例**: Picbreeder、EndlessForms
- **関連論文**: ASAL (foundation model feedback as proxy)

詳細は [`papers/spawning-methods.md`](papers/spawning-methods.md) を参照。

---

## キーテーマ / Key Themes

### 1. LLM × 進化計算 / LLM × Evolutionary Computation

**JP:**
LLMの登場により、進化計算の変異オペレータとしてLLMを活用する研究が急速に進展している。ELMでは、LLMが直接コードを変異・生成することで、従来の遺伝的プログラミングの表現力制約を突破した。ShinkaEvolveは、LLMによるプログラム進化をオープンエンドに拡張し、Digital Red Queenは共進化的なLLM対戦環境を構築した。

**EN:**
The advent of LLMs has rapidly advanced research using LLMs as mutation operators in evolutionary computation. ELM broke through the expressiveness constraints of traditional genetic programming by having LLMs directly mutate and generate code. ShinkaEvolve extends LLM-driven program evolution to open-ended settings, while Digital Red Queen constructs coevolutionary LLM battle environments.

### 2. NCAルネサンス / Neural Cellular Automata Renaissance

**JP:**
Neural Cellular Automata（NCA）は、微分可能なセルオートマトンとして2020年代に復活を遂げた。Growing Neural Cellular Automata（Mordvintsev et al.）を皮切りに、自己修復、テクスチャ生成、3D形態形成などへ応用が拡大している。SeRANNsは、ニューラルネットワーク自体が自己複製するという革新的な概念を提示した。

**EN:**
Neural Cellular Automata (NCA) experienced a renaissance in the 2020s as differentiable cellular automata. Starting with Growing Neural Cellular Automata (Mordvintsev et al.), applications have expanded to self-repair, texture generation, and 3D morphogenesis. SeRANNs introduced the groundbreaking concept of neural networks that self-replicate.

### 3. オープンエンド進化 / Open-Ended Evolution

**JP:**
人工生命研究の聖杯とも言えるオープンエンド進化は、無限に新規性を生み出し続ける系の構築を目指す。Quality-Diversity（MAP-Elites）、Novelty Search、Minimal Criterion Coevolution などのアルゴリズムが基盤となり、LLMの活用によって新たな局面を迎えている。

**EN:**
Open-ended evolution, often considered the holy grail of ALife research, aims to build systems that continuously generate novelty indefinitely. Algorithms such as Quality-Diversity (MAP-Elites), Novelty Search, and Minimal Criterion Coevolution form the foundation, and the utilization of LLMs has brought this field to a new phase.

### 4. 身体化AI / Embodied AI

**JP:**
仮想環境でのエージェントシミュレーション（Generative Agents, Project Sid）から、物理ロボットへの進化的設計転移まで、身体性を持つAIの研究が加速している。Voyagerのように、マインクラフト世界で自律的にスキルを獲得するLLMエージェントは、身体化AIとALifeの交差点に位置する。

**EN:**
Research on embodied AI is accelerating, from agent simulations in virtual environments (Generative Agents, Project Sid) to evolutionary design transfer to physical robots. LLM agents like Voyager, which autonomously acquire skills in Minecraft worlds, sit at the intersection of embodied AI and ALife.

---

## 主要カンファレンス / Major Conferences

| カンファレンス / Conference | 頻度 / Frequency | 次回開催 / Next Edition | 備考 / Notes |
|---|---|---|---|
| **ALIFE** (International Conference on Artificial Life) | 毎年 / Annual | ALIFE 2026 | 人工生命分野の最重要会議 / Premier ALife venue |
| **GECCO** (Genetic and Evolutionary Computation Conference) | 毎年 / Annual | GECCO 2026 | 進化計算の最大会議 / Largest EC conference |
| **NeurIPS** | 毎年 / Annual | NeurIPS 2026 | ALife関連ワークショップ多数 / Multiple ALife-related workshops |
| **ICML** | 毎年 / Annual | ICML 2026 | 自己組織化・創発関連 / Self-organization & emergence |
| **ICLR** | 毎年 / Annual | ICLR 2026 | NCA・生成モデル関連 / NCA & generative models |
| **IEEE SSCI** | 毎年 / Annual | IEEE SSCI 2026 | Swarm Intelligence関連 / Swarm intelligence |

### 関連ワークショップ / Related Workshops
- NeurIPS Workshop on Agent Learning in Open-Endedness (ALOE)
- GECCO Workshop on Open-Ended Evolution
- ALIFE Workshop on LLMs and Artificial Life

---

## 注目研究者 / Notable Researchers

| 研究者 / Researcher | 所属 / Affiliation | 主要テーマ / Key Topics |
|---|---|---|
| **Kenneth O. Stanley** | Maven / OpenAI Alumni | Open-endedness, Novelty Search, NEAT, ELM |
| **Karl Friston** | UCL | Free Energy Principle, Active Inference, Self-organization |
| **David Ha** | Sakana AI | World Models, NCA, Creative AI |
| **Sebastian Risi** | IT University of Copenhagen | NCA, Self-replication, ASAL, Quality-Diversity |
| **Bert Wang-Chak Chan** | Google DeepMind | Lenia, Flow-Lenia, Continuous CA |
| **Alexander Mordvintsev** | Google | Growing NCA, Self-organizing systems |
| **Joel Lehman** | Stochastic Labs | Quality-Diversity, ELM, Open-endedness |
| **池上高志 (Takashi Ikegami)** | 東京大学 / University of Tokyo | 複雑系、ALife理論、意識と生命 / Complex systems, ALife theory |
| **岡瑞起 (Mizuki Oka)** | 筑波大学 / University of Tsukuba | LLM×ALife、Digital Red Queen、ShinkaEvolve |
| **磯辺昇 (Noboru Isobe)** | 筑波大学 / University of Tsukuba | LLM-driven ALife, Core War, Program Evolution |
| **Pierre-Yves Oudeyer** | INRIA | Intrinsic Motivation, Curiosity-driven Learning |
| **Jeff Clune** | University of British Columbia | AI-Generating Algorithm, Open-endedness |

---

## 詳細トピック / Detailed Topics

各トピックの詳細は以下のファイルを参照：

| トピック / Topic | ファイル / File |
|---|---|
| 基盤モデル×ALife | [`papers/foundation-models.md`](papers/foundation-models.md) |
| スポーン・再生産手法 | [`papers/spawning-methods.md`](papers/spawning-methods.md) |
| オープンエンド進化 | [`papers/open-ended-evolution.md`](papers/open-ended-evolution.md) |
| Neural Cellular Automata | [`papers/neural-cellular-automata.md`](papers/neural-cellular-automata.md) |
| LLM×ALife | [`papers/llm-alife.md`](papers/llm-alife.md) |
| 日本の人工生命研究 | [`papers/japanese-alife.md`](papers/japanese-alife.md) |

---

## 参考リンク・リソース / References & Resources

### オンラインリソース / Online Resources
- [ISAL (International Society for Artificial Life)](https://alife.org/)
- [ALife Journal (MIT Press)](https://direct.mit.edu/artl)
- [Lenia Portal](https://chakazul.github.io/lenia.html)
- [Distill.pub - Growing Neural Cellular Automata](https://distill.pub/2020/growing-ca/)
- [OpenAI - Evolution through Large Models Blog](https://openai.com/research/evolution-through-large-models)
- [Sakana AI](https://sakana.ai/)

### 教科書・書籍 / Textbooks & Books
- Christoph Adami, *Introduction to Artificial Life* (Springer, 1998)
- Mark A. Bedau & Norman H. Packard (eds.), *Artificial Life VII* (MIT Press, 2000)
- 池上高志, 『動きが生命をつくる』（青土社, 2007）
- 池上高志, 『生命のサンドウィッチ理論』（講談社, 2012）
- 岡瑞起 他, 『作って動かすALife』（オライリー・ジャパン, 2018）

### BibTeX
参考文献の詳細は [`references.bib`](references.bib) を参照。

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Last updated: 2026-02-16*
