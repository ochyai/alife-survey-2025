# スポーン・再生産手法 / Spawning & Reproduction Methods

## 概要 / Overview

**JP:**
人工生命研究における「スポーン」とは、新たな個体・エージェント・パターンが生み出されるメカニズム全般を指す。本稿では、2024-2026年の研究動向を踏まえ、スポーン手法を5つのカテゴリに分類し、各手法の特徴・利点・代表的研究を整理する。

**EN:**
"Spawning" in ALife research refers broadly to mechanisms by which new individuals, agents, or patterns are generated. This document classifies spawning methods into five categories, organizing the characteristics, advantages, and representative studies of each approach based on research trends from 2024-2026.

---

## 分類体系 / Classification System

```
スポーン手法 / Spawning Methods
├── 1. 遺伝的継承 / Genetic Inheritance
│   ├── 交叉 / Crossover
│   ├── 突然変異 / Mutation
│   └── 選択 / Selection
├── 2. 自己複製 / Self-Replication
│   ├── テンプレートベース / Template-based
│   ├── 構成的 / Constructive
│   └── 情報的 / Informational
├── 3. LLM駆動生成 / LLM-Driven Generation
│   ├── コード生成 / Code Generation
│   ├── ルール生成 / Rule Generation
│   └── 構造生成 / Structure Generation
├── 4. セルオートマトン分裂 / CA Division
│   ├── パターン分裂 / Pattern Fission
│   ├── 成長分裂 / Growth Division
│   └── 自己組織化分裂 / Self-organized Division
└── 5. インタラクティブ進化 / Interactive Evolution
    ├── 人間フィードバック / Human Feedback
    ├── AIフィードバック / AI Feedback
    └── 混合フィードバック / Mixed Feedback
```

---

## 1. 遺伝的継承 / Genetic Inheritance

### 概要 / Description
**JP:** 親個体のパラメータ（遺伝子型）を交叉・突然変異によって子個体に伝達する手法。ダーウィン的進化の直接的な実装。

**EN:** Methods that transmit parental parameters (genotype) to offspring through crossover and mutation. A direct implementation of Darwinian evolution.

### 代表的手法 / Representative Methods

| 手法 / Method | 特徴 / Features | 適用例 / Applications |
|---|---|---|
| NEAT | トポロジー進化、歴史的マーカー | ネットワーク構造の進化 |
| HyperNEAT | 間接符号化、CPPN | 大規模パターン生成 |
| MAP-Elites | Quality-Diversity、アーカイブ | 多様な解の同時探索 |
| CMA-ES | 共分散行列適応 | 連続パラメータ最適化 |

### 最新動向 / Recent Developments
- ELMによるLLMベースの「知的変異」がこのカテゴリを拡張
- Quality-Diversity手法とLLMの統合（MAP-Elites + LLM mutation）
- 大規模並列進化計算によるスケーリング

---

## 2. 自己複製 / Self-Replication

### 概要 / Description
**JP:** 個体が自身のコピーまたは類似した構造を生成する能力。フォン・ノイマンの自己複製オートマトンに遡る、ALifeの中心的テーマ。

**EN:** The ability of an individual to generate copies or similar structures of itself. A central theme in ALife dating back to von Neumann's self-replicating automaton.

### 代表的手法 / Representative Methods

| 手法 / Method | メカニズム / Mechanism | 代表論文 / Key Paper |
|---|---|---|
| von Neumann型 | ユニバーサルコンストラクタ | von Neumann (1966) |
| Langtonループ | 最小自己複製構造 | Langton (1984) |
| Quine | 自己出力プログラム | 計算機科学全般 |
| SeRANNs | ニューラルネット自己複製 | Sudhakaran et al. (2024) |

### SeRANNs の革新性 / Innovation of SeRANNs
**JP:**
SeRANNs（Self-Replicating Neural Networks）は、ニューラルネットワーク自体が自己複製する手法を提案した。従来の自己複製はCA上のパターンやプログラムレベルであったが、SeRANNsは重み行列レベルでの自己複製を実現した。

**EN:**
SeRANNs proposed a method where neural networks themselves self-replicate. While conventional self-replication operated at the level of CA patterns or programs, SeRANNs achieved self-replication at the weight matrix level.

---

## 3. LLM駆動生成 / LLM-Driven Generation

### 概要 / Description
**JP:** 大規模言語モデルが直接的に新個体のコード、ルール、構造を生成する手法。2023年のELM以降、急速に発展。

**EN:** Methods where LLMs directly generate the code, rules, or structures of new individuals. Rapidly developed since ELM in 2023.

### 代表的手法 / Representative Methods

| 手法 / Method | 生成対象 / Target | 代表論文 / Key Paper |
|---|---|---|
| ELM | プログラムコード | Lehman et al. (2023) |
| Voyager | スキル関数 | Wang et al. (2023) |
| ShinkaEvolve | プログラム全体 | Isobe et al. (2025) |
| Digital Red Queen | 戦略コード | Isobe et al. (2025) |

### LLM駆動生成の特徴 / Features of LLM-Driven Generation
1. **セマンティック変異**: 意味を理解した上での変異が可能
2. **ゼロショット初期化**: 事前学習知識による高品質な初期個体生成
3. **自然言語インターフェース**: 進化の方向性をテキストで指示可能
4. **コンテキスト依存変異**: 個体の「文脈」を理解した変異

---

## 4. セルオートマトン分裂 / Cellular Automata Division

### 概要 / Description
**JP:** 連続的または離散的なセルオートマトン空間上で、パターンが分裂・成長することで新個体が生まれる手法。

**EN:** Methods where new individuals are born through pattern division and growth on continuous or discrete cellular automata spaces.

### 代表的手法 / Representative Methods

| 手法 / Method | 特徴 / Features | 代表論文 / Key Paper |
|---|---|---|
| Lenia | 連続CA、多様な生物的パターン | Chan (2020) |
| Flow-Lenia | 質量保存、局所パラメータ | Plantec et al. (2023) |
| Biomaker CA | 生態系シミュレーション | Randazzo & Mordvintsev (2023) |
| Growing NCA | 微分可能CA、自己修復 | Mordvintsev et al. (2020) |

### Flow-Leniaの革新性 / Innovation of Flow-Lenia
**JP:**
Flow-Leniaは、Leniaに質量保存則とパラメータの局所化を導入することで、より生物学的にリアルなダイナミクスを実現した。パターンの分裂が自然に発生し、オープンエンド進化への道を開いた。

**EN:**
Flow-Lenia introduced mass conservation and parameter localization to Lenia, achieving more biologically realistic dynamics. Pattern division occurs naturally, opening the path toward open-ended evolution.

---

## 5. インタラクティブ進化 / Interactive Evolution

### 概要 / Description
**JP:** 人間や他のエージェントのフィードバックを選択圧として用いる進化手法。美的評価など、定量化が困難な目的関数に対して有効。

**EN:** Evolutionary methods that use feedback from humans or other agents as selection pressure. Effective for objectives that are difficult to quantify, such as aesthetic evaluation.

### 代表的手法 / Representative Methods

| 手法 / Method | フィードバック源 / Feedback Source | 代表例 / Examples |
|---|---|---|
| Picbreeder | 人間の美的判断 | Stanley (2007) |
| EndlessForms | 人間の形態選好 | Clune et al. (2011) |
| ASAL | Foundation Model | Sudhakaran et al. (2024) |

### AIフィードバックへの移行 / Transition to AI Feedback
**JP:**
ASALのように、人間のフィードバックをFoundation Model（CLIP等）のフィードバックで代替する流れが加速している。これにより、インタラクティブ進化のスケーラビリティが大幅に向上した。

**EN:**
As seen in ASAL, the trend of replacing human feedback with foundation model (CLIP, etc.) feedback is accelerating. This has significantly improved the scalability of interactive evolution.

---

## 手法比較 / Method Comparison

| 項目 / Criteria | 遺伝的継承 | 自己複製 | LLM駆動 | CA分裂 | インタラクティブ |
|---|---|---|---|---|---|
| スケーラビリティ | 高 | 中 | 高 | 中 | 低→高(AI) |
| 新規性 | 中 | 低 | 高 | 中 | 高 |
| 計算コスト | 低 | 低 | 高 | 中 | 低 |
| 生物学的妥当性 | 中 | 高 | 低 | 高 | 低 |
| 制御可能性 | 高 | 低 | 高 | 低 | 高 |
