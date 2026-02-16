# Neural Cellular Automata (NCA)

## 概要 / Overview

**JP:**
Neural Cellular Automata（NCA）は、従来のセルオートマトンの更新ルールをニューラルネットワークで置き換えた、微分可能なセルオートマトンモデルである。2020年のGrowing Neural Cellular Automata（Mordvintsev et al.）を皮切りに、自己修復、テクスチャ生成、3D形態形成など多岐にわたる応用が展開されている。

**EN:**
Neural Cellular Automata (NCA) are differentiable cellular automata models where the update rules of conventional CAs are replaced by neural networks. Starting with Growing Neural Cellular Automata (Mordvintsev et al., 2020), applications have expanded to self-repair, texture generation, 3D morphogenesis, and beyond.

---

## 基礎 / Foundations

### 従来のCAからNCAへ / From Conventional CA to NCA

| 特性 / Property | 従来のCA / Conventional CA | NCA |
|---|---|---|
| ルール / Rules | 手動設計 / Hand-designed | 学習可能 / Learnable |
| 微分可能性 | 不可 / No | 可能 / Yes |
| 状態空間 | 離散 / Discrete | 連続 / Continuous |
| 最適化 | 探索的 / Search-based | 勾配降下 / Gradient descent |

### NCAの基本アーキテクチャ / Basic NCA Architecture
1. **知覚 (Perception)**: Sobelフィルタ等で近傍情報を集約
2. **更新ルール (Update Rule)**: 小規模ニューラルネットワーク
3. **確率的更新 (Stochastic Update)**: ランダムに一部セルのみ更新
4. **残差接続 (Residual Connection)**: 安定性のための残差更新

---

## 主要研究 / Key Research

### Growing Neural Cellular Automata
- **著者**: Alexander Mordvintsev, Ettore Randazzo, Eyvind Niklasson, Michael Levin
- **年**: 2020
- **リンク**: [Distill.pub](https://distill.pub/2020/growing-ca/)

**JP:**
NCA研究の起点となった論文。単一セルから目標画像を成長させるNCAを学習し、部分的な破壊からの自己修復能力を持つことを示した。「局所的なルールからグローバルなパターンが創発する」というALifeの中心原理を微分可能な形で実装した。

**EN:**
The seminal paper of NCA research. It learned an NCA that grows a target image from a single cell and showed it possesses self-repair capabilities from partial destruction. It implemented the central ALife principle of "global patterns emerging from local rules" in a differentiable form.

### Self-Classifying MNIST Digits
- **著者**: Ettore Randazzo, Alexander Mordvintsev, Eyvind Niklasson, Michael Levin
- **年**: 2020

**JP:** NCAが画像分類タスクを分散的に実行できることを示した。各セルが局所的な計算のみで全体の分類結果に貢献する。

### Texture Generation with NCA
- **著者**: Alexander Mordvintsev, Eyvind Niklasson, Ettore Randazzo
- **年**: 2021

**JP:** NCAをテクスチャ生成に応用。単一のNCAルールから多様なテクスチャパターンを生成可能であることを示した。

---

## Lenia系列 / Lenia Family

### Lenia: Biology of Artificial Life
- **著者**: Bert Wang-Chak Chan
- **年**: 2020
- **リンク**: [arXiv:1911.07968](https://arxiv.org/abs/1911.07968)

**JP:**
Leniaは、Game of Lifeを連続空間・連続時間・連続状態に拡張したCAシステムである。数百種類の「生物的」パターン（glider、oscillator、自己複製子等）が発見されており、ALifeにおけるCA研究の新たな標準となっている。

**EN:**
Lenia is a CA system that extends the Game of Life to continuous space, continuous time, and continuous states. Hundreds of "biological" patterns (gliders, oscillators, self-replicators, etc.) have been discovered, establishing a new standard for CA research in ALife.

### Flow-Lenia
- **著者**: Erwan Plantec, Gautier Hamon, Mayalen Etcheverry, Pierre-Yves Oudeyer, Clément Moulin-Frier, Bert Wang-Chak Chan
- **年**: 2023
- **リンク**: [arXiv:2212.07906](https://arxiv.org/abs/2212.07906)

**JP:**
Flow-Leniaは、Leniaに質量保存則とパラメータの局所化を導入した拡張である。質量保存により、パターンの安定性が向上し、パラメータの局所化により、異なるルールを持つ領域が共存できる。これにより、パターンの自然な分裂やオープンエンドな進化の基盤が整えられた。

**EN:**
Flow-Lenia is an extension of Lenia that introduces mass conservation and parameter localization. Mass conservation improves pattern stability, and parameter localization allows regions with different rules to coexist. This lays the groundwork for natural pattern division and open-ended evolution.

---

## 自己複製NCA / Self-Replicating NCA

### SeRANNs: Self-Replicating Neural Networks
- **著者**: Shyam Sudhakaran, Djordje Grbic, Siyan Li, Adam Katona, Elias Najarro, Claire Glanois, Sebastian Risi
- **年**: 2024
- **リンク**: [arXiv:2404.03087](https://arxiv.org/abs/2404.03087)

**JP:**
SeRANNsは、ニューラルネットワークの重み自体が自己複製するシステムを実現した。NCAの枠組みを拡張し、ネットワークが自身のコピーを生成する能力を学習する。これは、フォン・ノイマンの自己複製オートマトンの現代的な神経科学的実装と見なすことができる。

**EN:**
SeRANNs achieved a system where neural network weights themselves self-replicate. Extending the NCA framework, networks learn the ability to generate copies of themselves. This can be viewed as a modern neuroscience implementation of von Neumann's self-replicating automaton.

**主要な知見 / Key Findings:**
- ニューラルネットワークは自己複製を学習可能
- 複製の忠実度と変異のトレードオフが進化を駆動
- 自己複製能力と他のタスク能力を同時に学習可能

---

## Biomaker CA
- **著者**: Ettore Randazzo, Alexander Mordvintsev
- **年**: 2023
- **リンク**: [arXiv:2307.09320](https://arxiv.org/abs/2307.09320)

**JP:**
Biomaker CAは、NCAベースの人工生態系シミュレーションである。各セルが異なる「遺伝子」（NCAの重み）を持ち、成長・分裂・死・栄養獲得といった生物学的プロセスをシミュレートする。複数の「種」が同一環境で競争・共存するダイナミクスが創発する。

**EN:**
Biomaker CA is an NCA-based artificial ecosystem simulation. Each cell has different "genes" (NCA weights) and simulates biological processes such as growth, division, death, and nutrient acquisition. Dynamics of multiple "species" competing and coexisting in the same environment emerge.

---

## 応用 / Applications

1. **自己修復材料 / Self-Healing Materials**: NCAの自己修復能力を材料科学に応用
2. **プロシージャル生成 / Procedural Generation**: ゲームやアートのコンテンツ生成
3. **形態形成 / Morphogenesis**: 3D形状の成長・発達シミュレーション
4. **ロボティクス / Robotics**: 分散制御のための局所ルール学習
5. **生命の起源 / Origin of Life**: 自己複製・自己組織化のメカニズム理解

---

## 今後の展望 / Future Directions

- 3D NCAの大規模シミュレーション
- NCAとLLMの統合（テキストからNCAルールを生成）
- 物理シミュレーションとの結合（粒子系、流体）
- NCAベースのロボットコントローラ
- メタ学習NCA（新しいタスクへの高速適応）
