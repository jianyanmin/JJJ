# 论文返修任务书（Revision Task Specification）

> 用途：交付给 codex 类 AI 编码/写作工具执行的**可操作任务说明书**。
> 目标：完成本次 Associate Editor 返修意见的逐条响应，产出**带修订痕迹的返修稿**与**中英文逐点回复信**。
> 版本：v1.0 ｜ 生成日期：2026-09-28

---

## 0. 任务背景与资产清单

### 0.1 稿件基本信息

| 项目 | 内容 |
|---|---|
| 题目 | Lactate Dynamics at the *Pseudomonas aeruginosa*–Host Interface: Bacterial Metabolism, Host Defense, and Emerging Links to Histone Lactylation |
| 类型 | 传统叙述性综述（traditional narrative review） |
| 轮次 | **第二轮返修**（AE 明确说明 "the revised manuscript"，"substantial revisions have made the manuscript more focused"） |
| 通讯作者 | Ke Wang；Fashuang Yang |
| 正文结构 | 7 个一级章节 + Author contributions / Funding / Conflict of interest / Data availability / References |
| 篇幅 | 正文约 10,900 词（含表格文字） |
| 参考文献 | 124 条 |
| 图表 | Table 1–3（证据分级表、测量解释边界表、治疗方向与权衡表）；Figure 1–4（图注在稿件内，图件为独立文件） |

### 0.2 章节地图（供定位修改用）

```
1  Introduction
2  Lactate availability at the P. aeruginosa–host interface
   2.1 Host sources and the bacterial sink
   2.2 Transport, clearance, and compartmentalization
3  How P. aeruginosa consumes and reshapes host lactate
   3.1 Stereospecific utilization and its conditional regulation
   3.2 Depletion of the host epithelial pool
   3.3 2-AA-driven reprogramming of host metabolism
4  What lactate does at the interface
   4.1 Bacterial fitness and adaptation
   4.2 Epithelial mucociliary defense
   4.3 Macrophage tolerance and persistence
5  Histone lactylation: an emerging extension
   5.1 Chemical identity, donors, and enzymes
   5.2 Lactate dependence is not lactylation dependence
   5.3 Matching measurement to claim
6  Therapeutic implications and open questions
7  Conclusion
```

### 0.3 输入资产（执行前必须全部就位）

| 编号 | 资产 | 格式 | 说明 |
|---|---|---|---|
| A1 | `Manuscript-clean.docx` | .docx | 上一轮返修后的清稿（无修订痕迹） |
| A2 | 审稿意见文件 | .doc | Associate Editor Krishnendu Mukherjee，2026-09-28 10:38，共 5 条 |
| A3 | 上一轮回复信 | 待补 | **若存在必须提供**，用于保证本轮口径与上一轮不矛盾 |
| A4 | 期刊作者须知 | 待补 | 用于确认标题层级、缩写规则、斜体规范、参考文献格式 |
| A5 | 参考文献库 | .bib / .ris / EndNote | 用于插入 AE 建议的 2 篇新文献并重排编号 |
| A6 | 图件源文件 | .ai/.pdf/.pptx/.py/.R | Figure 1–4，若需改图注中的术语则可能同步改图内标签 |

> **缺失处理规则**：A3–A6 任一缺失时，**不得臆造**。在产出中以 `【待作者确认：xxx】` 形式标记，并在最终交付说明中集中列出。

---

## 1. 审稿意见逐条拆解与回复策略

AE 结论为：**大修后可考虑最终接收**（"before the manuscript can be considered for final acceptance"），语气正面，无实质性科学质疑。核心诉求集中在**可读性、措辞审慎度、术语规范**三类，**不要求补做实验**。

> **重要定性**：本稿为综述，第 5 条"补充讨论近期文献"是唯一涉及内容增量的意见。任务书中所称"补充实验"在本稿语境下应理解为**补充证据与文献论证**，不涉及湿实验。

### 意见 1 — 整体清晰度与可读性

> "some sections remain difficult to read in terms of both context and language. In particular, information concerning the two major aspects namely, bacterial lactate utilization and lactate-associated changes in the infected host, is sometimes difficult to extract."

| 项目 | 内容 |
|---|---|
| 性质 | 结构/写作类，**工作量最大**，约占本轮 50% |
| 根因诊断 | AE 点名的两条主线（①细菌乳酸利用 ②感染宿主中乳酸相关改变）在现稿中**被章节切分打散**：细菌侧证据散落于 §2.1、§3.1、§4.1；宿主侧散落于 §2.1、§3.2、§3.3、§4.2、§4.3。读者需跨章节自行拼接。 |
| 回复策略 | **接受并实质性修改**。不做全文重排（会推翻上一轮已被认可的结构），而采用"**双主线显性化**"策略：在不改变一级章节编号的前提下，通过导航句、主题句、小结句，把两条线索在文中反复锚定。 |
| 具体动作 | ① §1 末尾新增一段**双主线路线图**，明确告诉读者两条线各在何处展开；② §3 与 §4 章首各加 2–3 句**过渡导航**，声明本章分别讲哪条线；③ 为 §2.1/§2.2/§3.1/§3.2/§3.3/§4.1/§4.2/§4.3 每节补**段首主题句 + 节末 1 句 take-home**；④ 逐段执行长句拆分（见 §3.3 自检阈值）；⑤ 考虑为两条主线各加一个**可选的小标题标签**（如 "Bacterial arm" / "Host arm"），若期刊格式允许。 |
| 不做什么 | 不重编章节号；不删除现有的证据分级（T1–T3）体系；不压缩 §5 的方法学告诫（这是本稿的学术贡献点）。 |

### 意见 2 — 巨噬细胞部分依赖摘要级研究

> "relies heavily on findings reported in an abstract-level study… the mechanistic interpretation should be presented more cautiously… reducing the mechanistic claims or explicitly presenting them as a research hypothesis rather than an established mechanism."

| 项目 | 内容 |
|---|---|
| 性质 | 措辞审慎度，**风险最高**（直接关系最终接收） |
| 对象 | 参考文献 **(20)**，2026 supplement abstract：2-AA → LDHA↑ → lactate↑ → GTPSCS/CBP-p300 → H3K18la↑ → 耐受性巨噬细胞与胞内持留 |
| 现状核查 | 现稿**已有**审慎处理：Abstract 写 "reported only in abstract form"；§1 写 "so far only in abstract form"；§3.3 写 "awaits full-length reporting and independent validation"；§4.3 写 "Necessity has not been tested"；Table 1 标为 T3；Figure 4C 用虚线框与虚线箭头表示。**现稿基础良好，但 AE 仍感到机制性过强** —— 说明问题出在**动词与句式**，而非缺少免责声明。 |
| 回复策略 | **完全接受**。采取"**假设化改写 + 篇幅收缩 + 视觉降权**"三管齐下，并在回复信中**列表展示逐处改动前后对照**，让 AE 一眼看到落实。 |
| 具体动作 | ① **动词降级**：将 `increases / drives / reprograms / links … to` 改为 `has been proposed to increase / would predict / is hypothesized to`；② **显式标注假设**：在 §3.3 与 §4.3 该分支的首句前加 "As a research hypothesis awaiting full-length validation, …"；③ **篇幅收缩**：该分支在 §3.3 与 §4.3 合计压缩 ≥30%，避免"heavily relies"的观感；④ **Figure 4 图注**加一句 "(C) is presented as a hypothesis, not an established mechanism."；⑤ **Abstract** 中相应句改为假设性表述；⑥ **§6** 中凡以 (20) 支撑的治疗推论，须明确标注其证据等级。 |
| 红线 | **不得删除**该分支（它是本稿"emerging extension"叙事的组成部分，且已在 Figure 4 与 Table 1 中成体系）。只降调、不删除。 |

### 意见 3 — "Therapeutic directions" 改为 "Potential therapeutic directions"

> "could be changed to 'Potential therapeutic directions', unless the authors can provide stronger preclinical evidence."

| 项目 | 内容 |
|---|---|
| 性质 | 措辞，**最易落实**，但**存在陷阱** |
| ⚠️ 陷阱 | AE 说的是"heading or terminology"，但现稿**一级标题实为 "6 Therapeutic implications and open questions"**，并不存在名为 "Therapeutic directions" 的标题。该措辞实际出现在 **3 处正文/图表**：<br>① **Abstract**："It then sets out the therapeutic directions that follow…"<br>② **§6 正文**："Therapeutic direction cannot be inferred from the sign of a lactate or H3K18la change alone…"<br>③ **Table 3 表题**："Candidate therapeutic directions at the lactate interface…" |
| 回复策略 | **完全接受，并主动扩大执行范围**。不只改一处，而是全文统一为 "potential therapeutic directions"，并在回复信中说明"我们核查了全文，发现该措辞出现于 3 处，已全部修改"——这是**低成本高印象分**的动作。 |
| 具体动作 | ① Abstract 改为 "…sets out the **potential** therapeutic directions that follow…"；② §6 正文句改为 "**Potential** therapeutic direction cannot be inferred…"（注意保持语法通顺，必要时改写为 "The choice among potential therapeutic directions cannot be inferred…"）；③ Table 3 表题保留 "Candidate"（其语义已等价于 potential），或统一改为 "Potential therapeutic directions…"——**二选一，全文一致**；④ 顺带核查 §6 与 §7 中所有治疗相关表述，确保均为条件式语气（`would`, `may`, `remains to be tested`），无一处暗示已有临床前验证。 |

### 意见 4 — 术语与命名规范化

> "'histone lactylation,' 'H3K18la,' 'Kla,' 'L-lactyllysine,' and 'lactylation' should be standardized… Abbreviations should be defined at first appearance and used consistently… scientific names should be italicized throughout."

| 项目 | 内容 |
|---|---|
| 性质 | 规范类，**可机械化核查**，**必须 100% 清零** |
| 现状实测 | 已对 A1 做逐 run 格式审计，结果如下（**这是硬伤，AE 完全正确**）： |

**斜体审计实测结果（A1 原稿）**

| 词条 | 斜体 | 非斜体 | 判定 |
|---|---:|---:|---|
| *Pseudomonas aeruginosa* | 8 | **36** | ❌ 严重不一致 |
| *P. aeruginosa* | 14 | **8** | ❌ 不一致 |
| *Staphylococcus aureus* | 0 | **3** | ❌ 全部未斜体 |
| *S. aureus* | 0 | **1** | ❌ 未斜体 |
| *Escherichia coli* | 0 | **1** | ❌ 未斜体 |
| *lldPDE* | 3 | **4** | ❌ 不一致 |
| *lldD* | 3 | **2** | ❌ 不一致 |
| *lldA* | 6 | **5** | ❌ 不一致 |
| *lldE* | 0 | **1** | ❌ 未斜体 |
| *lldP* | 3 | **5** | ❌ 不一致 |
| *Beclin1* | 1 | **4** | ❌ 不一致 |
| *Scd1* | 1 | 1 | ❌ 不一致 |
| *Ythdf1* | 2 | **1** | ❌ 不一致 |
| *in vivo* / *ex vivo* | 0 | 6 | ⚠️ 依期刊风格定（多数期刊现已不要求斜体） |

| 项目 | 内容 |
|---|---|
| 术语统计 | `lactylation` 56 次；`H3K18la` 35 次；`histone lactylation` 12 次；`Kla` 8 次；`L-lactyllysine` 1 次 |
| 回复策略 | **完全接受**。建立**术语总表（Terminology Table）**，一次性定义并全文替换；**斜体用脚本批量修正**（人工逐处改必漏）。回复信中附上术语表，显示系统性处理。 |
| 具体动作 | 见下方"**§1.4.1 术语标准化规则**"与"**§3.4 自动化核查脚本**"。 |

#### 1.4.1 术语标准化规则（执行时作为唯一真源）

| 概念 | 规范写法 | 首次定义位置与写法 | 后续用法 |
|---|---|---|---|
| 赖氨酸乳酰化（总称） | lysine lactylation (Kla) | §1 或 Abstract 首现处：`lysine lactylation (Kla)` | 此后一律 `Kla`；**不再混用** `lactylation` 作为缩写指代 |
| 组蛋白乳酰化 | histone lactylation | 首现处全拼，无需缩写 | 保留全称；仅在明确指组蛋白时使用 |
| H3 第 18 位赖氨酸乳酰化 | H3K18 lactylation (H3K18la) | 首现处：`histone H3 lysine 18 lactylation (H3K18la)` | 此后一律 `H3K18la` |
| L-型乳酰赖氨酸 | L-lactyllysine (K<sub>L</sub>-la) | §5.1 首现处全拼 + 缩写 | 此后 `K`<sub>`L`</sub>`-la`；与 `K`<sub>`D`</sub>`-la`、`Kce` 并列时保持同一体例 |
| D-型乳酰赖氨酸 | D-lactyllysine (K<sub>D</sub>-la) | 同上 | 同上 |
| Nε-羧乙基赖氨酸 | Nε-carboxyethyllysine (Kce) | 同上 | 同上 |
| H3K18 乙酰化 | H3K18 acetylation (H3K18ac) | 首现处全拼 | **务必与 H3K18la 视觉区分**，Figure 4B 图注已有提示，需保持 |

**执行要点**
1. **`lactylation` 与 `Kla` 的分工必须明确**：`lactylation` 仅作为普通名词（如 "protein lactylation", "histone lactylation"）；`Kla` 仅作为该化学修饰的缩写符号（如 "pan-Kla immunoblot", "a Kla signal"）。现稿 Table 2 已有 "Pan-Kla immunoblot"，与正文用法需对齐。
2. **缩写首现定义全文只做一次**，且必须出现在**正文**中；Abstract 中如使用缩写，需在 Abstract 内独立定义一次（摘要与正文的缩写定义相互独立，此为多数期刊通则）。
3. **建立全文缩写清单**并核对：2-AA, OMV, HHQ, MCT, LL-37, CF, EBC, m6A, LDHA, GTPSCS, CBP/p300, HDAC, ACSS2, AARS1/2, KAT2A, PGC-1α, ERRα, MPC1, SCD1, ULK1, YTHDF1, DNAH5, MvfR, c-di-GMP, NET, T1–T3 等 —— 逐一确认首现处已定义、后续无全拼/缩写混用。
4. **斜体规则**：属名+种名（*Pseudomonas aeruginosa*, *P. aeruginosa*, *Staphylococcus aureus*, *Escherichia coli*）**全文斜体**，包括标题、摘要、图题、表题、图注、参考文献标题中的种名。**基因名斜体**（*lldPDE*, *lldP*, *lldD*, *lldE*, *lldA*, *lldR*, *lldS*, *ldhA*, *mvfR*, *Scd1*, *Beclin1*, *Ythdf1*）；**蛋白名正体**（LldP, LldD, LldE, LldA, LldR, LldS, LdhA, MvfR, SCD1, Beclin1, YTHDF1）。Figure 2 图注已声明此规则（"Protein names are set in roman and gene names in italics"），**正文必须与图注自洽**。
5. **突变体写法**：`ΔlldDΔlldA`、`ΔmvfR` 中的基因部分斜体，Δ 正体。
6. **`in vivo`/`ex vivo`/`in vitro`**：按 A4 期刊须知执行；若无明确规定，**统一为正体**（现代主流风格）并在回复信中说明依据。

### 意见 5 — 补充讨论近期文献

> 建议（"if found suitable"）讨论 2 篇：
> **[Ref-N1]** Mariano F, et al. CytoSorb in burn patients with septic shock and AKI on CKRT efficiently reduces the levels of Gram-negative-derived quorum-sensing molecules associated with lactate increases. *Burns*. 2026 Sep;52(7):108105. doi:10.1016/j.burns.2026.108105
> **[Ref-N2]** Wang WR, Yan L, Zhao CY, He CC, Gao XH. Glycolytic reprogramming and immune responses in macrophages: a crosstalk driven by bacterial infection. *Front Immunol*. 2026 Apr 10;17:1783266. doi:10.3389/fimmu.2026.1783266

| 项目 | 内容 |
|---|---|
| 性质 | 内容增量，**措辞为"consider… if found suitable"，即软性建议** |
| 判定 | **两篇均高度契合，应当全部采纳**。理由：N1 直接连接"革兰阴性菌群体感应分子—乳酸升高—烧伤脓毒症"，与现稿 §4.1（HHQ/OMV/LL-37 轴）和 §2.1（人源烧伤创面渗出液，参考文献 12）形成呼应；N2 直接覆盖"细菌感染驱动的巨噬细胞糖酵解重编程"，正是 §3.3 与 §4.3 的上游框架。 |
| ⚠️ 强制核验 | **执行前必须用 PubMed/DOI 核验两条文献的著录信息**（作者、刊名、年卷期页、DOI 全部逐字段比对）。审稿意见中的著录可能有笔误。**禁止直接照抄未经核验的条目入库。** 若核验发现 DOI 或卷期不符，以数据库为准，并在回复信中不作声张地使用正确信息。 |
| 插入方案 | **N1 → §4.1**（在 HHQ/LL-37/酸化段落之后，1–2 句）：作为"群体感应分子与乳酸升高在临床脓毒症中共变"的临床侧佐证，并可在 §6 中作为"体外清除群体感应分子"这一潜在治疗方向的现实锚点（注意仍需条件式语气，CytoSorb 数据不足以支持疗效主张）。<br>**N2 → §3.3 章首或 §4.3 引入处**（1–2 句）：作为巨噬细胞糖酵解重编程的综述性背景，为 2-AA 相关讨论提供更宽的语境，同时**有助于缓解意见 2**——用已发表全文文献承托巨噬细胞部分，降低对摘要级文献 (20) 的依赖观感。 |
| 战术价值 | **N2 的插入同时回应意见 2 和意见 5**，务必在回复信的**意见 2 回复中交叉引用**这一点。 |
| 副作用管理 | 插入 2 条新文献将导致**参考文献编号整体后移**。必须全文重排编号并核对所有正文引用位、表格引用位、图注引用位（现稿引用密集，如 "(13, 14, 55, 56)"、"(18, 19, 77–79)" 等区间引用尤易出错）。 |

---

## 2. 阶段拆解（P0–P6）

> 每阶段格式：**输入 → 动作 → 产出 → 通过条件（Gate）**。
> 未达 Gate 不得进入下一阶段。

### P0 · 资产校验与基线建立

| 项 | 内容 |
|---|---|
| **输入** | A1–A6 |
| **动作** | ① 校验 A1 可解析、章节完整、表 1–3 与图注 1–4 齐全；② 抽取纯文本基线 `baseline.txt` 与格式审计基线 `baseline_format.json`（记录每个 run 的斜体/加粗状态）；③ 清点参考文献 124 条并建立 `refs_map.csv`（旧编号 → 作者年份 → 新编号预留列）；④ 建立全文缩写清单 `abbrev_inventory.csv`；⑤ 核验 A4 期刊须知中的标题层级/斜体/缩写/参考文献格式要求；⑥ 列出缺失资产。 |
| **产出** | `baseline.txt`、`baseline_format.json`、`refs_map.csv`、`abbrev_inventory.csv`、`P0_资产校验报告.md` |
| **Gate** | 章节数、表数、图注数、参考文献数与 §0.1 一致；缺失资产已显式登记；**若 A4 缺失，必须先向作者索取或明确声明采用的默认规范** |

### P1 · 意见拆解与回复策略确认

| 项 | 内容 |
|---|---|
| **输入** | A2、A3、`P0_资产校验报告.md` |
| **动作** | ① 将 5 条意见拆为**可执行子项**（预计 5 条 → 约 18–22 个子项）；② 为每个子项标注：定位（章节/段落/表/图）、动作类型（改写/降调/替换/新增/格式）、预估改动量、风险等级；③ 与 A3 比对，确保本轮口径不与上一轮回复自相矛盾；④ 生成 `response_matrix.csv`（列：意见号、子项号、原文摘录、定位、动作、优先级、风险、状态）。 |
| **产出** | `response_matrix.csv`、`P1_意见拆解与策略.md` |
| **Gate** | 5 条意见 100% 覆盖，无"待定"；每个子项可独立验收；风险等级 ≥ 高的子项已写明兜底方案 |

### P2 · 内容实质性修改（意见 2、5 优先）

> **先做内容、后做语言**——顺序不可颠倒，否则润色成果会被内容改动推翻。

| 项 | 内容 |
|---|---|
| **输入** | A1、`response_matrix.csv`、A5、两篇新文献全文/摘要（经 PubMed 核验） |
| **动作** | **P2-a 意见 2（降调）**：逐处执行动词降级、假设化标注、篇幅收缩 ≥30%、Figure 4 图注加注、Abstract 同步；建立 `claim_downgrade_log.csv`（原句 / 改后句 / 所在位置 / 降调理由）。<br>**P2-b 意见 5（补文献）**：DOI 核验 → 写入 A5 → 按插入方案撰写 §4.1 与 §3.3/§4.3 的插入文字 → **全文参考文献重编号** → 逐条核对所有正文/表/图注引用位。<br>**P2-c 意见 3（措辞）**：3 处 "therapeutic direction(s)" 统一处理 + §6/§7 治疗语气全面条件式化。 |
| **产出** | `manuscript_P2.docx`（内容改定稿，尚未润色）、`claim_downgrade_log.csv`、`refs_map.csv`（新编号已填）、`P2_内容修改说明.md` |
| **Gate** | ① 摘要级文献 (20) 相关表述**无一处**使用无条件机制性动词（用 §3.4 脚本 D 扫描）；② 该分支篇幅较基线下降 ≥30%；③ 新增 2 条文献著录经 DOI 核验通过；④ 参考文献重编号后**引用位 100% 对齐**（脚本 C 零告警）；⑤ "therapeutic direction" 措辞全文统一 |

### P3 · 结构与可读性重构（意见 1）

| 项 | 内容 |
|---|---|
| **输入** | `manuscript_P2.docx` |
| **动作** | ① §1 末新增**双主线路线图**段落（细菌侧 / 宿主侧各在何处展开）；② §3、§4 章首加过渡导航；③ 为 8 个二级小节补段首主题句与节末 take-home；④ 逐段长句拆分（阈值见 §3.3）；⑤ 被动语态与名词化压缩；⑥ 检查段落长度（>200 词的段落需评估拆分）；⑦ 核对两条主线在全文的**锚定密度**——确保读者每 1–2 页都能定位当前处于哪条线。 |
| **产出** | `manuscript_P3.docx`、`P3_可读性重构说明.md`（含双主线锚点分布表） |
| **Gate** | ① 两条主线在 §1 有显式路线图；② 8 个二级小节均有主题句与 take-home；③ 长句指标达标（脚本 A）；④ **反向验收**：仅读每段首句能否复原全文论证链——不能则重做 |

### P4 · 术语与格式规范化（意见 4）

> **必须放在 P3 之后**：P3 会产生新文字，新文字同样需要术语与斜体规范。

| 项 | 内容 |
|---|---|
| **输入** | `manuscript_P3.docx`、§1.4.1 术语总表、A4 |
| **动作** | ① 生成术语总表并落盘为 `terminology.csv`（唯一真源）；② **脚本化**执行斜体修正（种名、基因名），蛋白名强制正体；③ 缩写首现定义核查与补齐（正文与摘要各一次）；④ 全文缩写一致性扫描（有无全拼/缩写混用）；⑤ 表 1–3 与图注 1–4 同步规范（**易漏项，必须单独走一遍**）；⑥ 参考文献标题中的种名斜体核查；⑦ 若图件内含种名/基因名标签，登记为 `【需改图】` 清单交作者。 |
| **产出** | `manuscript_P4.docx`、`terminology.csv`、`format_audit_after.json`、`P4_术语格式核查报告.md`、`需改图清单.md` |
| **Gate** | 脚本 B 输出**零不一致**：种名斜体 100%、基因名斜体 100%、蛋白名正体 100%、缩写首现定义 100%、后续用法 100% 一致 |

### P5 · 整体润色与学术规范复核

| 项 | 内容 |
|---|---|
| **输入** | `manuscript_P4.docx` |
| **动作** | ① 全文通读润色（语法、时态、冠词、搭配、过渡词）；② **时态规范**：描述既往研究结果用过去时，陈述公认事实/本文观点用现在时——现稿混用较多，需统一；③ 逻辑连接词检查（避免 however/therefore 滥用）；④ **证据分级（T1–T3）标注一致性**复核——这是本稿特色，不可在润色中被削弱；⑤ 摘要与正文一致性复核（摘要中每个论断在正文均有对应且强度一致）；⑥ 标题/关键词/running title 与正文一致性；⑦ 数字、单位、符号规范（mmol/L、%、℃、α/β 等）；⑧ **最终反向自检**：以审稿人视角重读，逐条确认 5 条意见已落实。 |
| **产出** | `manuscript_final_clean.docx`（清稿）、`P5_润色说明.md` |
| **Gate** | ① 脚本 A/B/C/D 全部零告警；② 摘要—正文—结论三处论断强度一致；③ 无新增未定义缩写；④ 全文无 `【待作者确认】` 以外的占位符 |

### P6 · 交付物生成

| 项 | 内容 |
|---|---|
| **输入** | A1（基线）、`manuscript_final_clean.docx`、`response_matrix.csv`、`claim_downgrade_log.csv` |
| **动作** | ① 生成**带修订痕迹稿** `manuscript_final_tracked.docx`（见 §4.1 三选一方案）；② 生成**修改说明表** `修改对照表.xlsx/csv`（意见号 / 子项 / 原文 / 改后文 / 位置 / 页行号）；③ 生成**英文回复信** `Response_to_Reviewers_EN.docx`；④ 生成**中文回复信** `审稿意见回复_CN.docx`；⑤ 生成 `提交清单.md` 与 `遗留问题与待确认事项.md`。 |
| **产出** | 见 §4 交付物清单 |
| **Gate** | 交付物齐全；修订痕迹稿可在 Word 中正常显示"接受/拒绝修订"；回复信中每条意见均标注**具体页码与行号** |

---

## 3. 质量自检标准

### 3.1 通用红线（任一触发即判定不合格）

| # | 红线 |
|---|---|
| R1 | **臆造文献**：任何未经 DOI/PubMed 核验的参考文献条目 |
| R2 | **臆造数据**：为回应意见而编造任何数值、效应量、样本量、实验结果 |
| R3 | **过度承诺**：在回复信中承诺稿件中并未实际做出的修改 |
| R4 | **删除实质内容**：以"简化"为名删除证据分级体系、方法学告诫（§5）、或摘要级分支本身 |
| R5 | **引用错位**：参考文献重编号后出现任一引用位与文献不对应 |
| R6 | **改变科学结论**：润色过程中改变任何论断的方向或强度 |
| R7 | **格式回退**：P3/P5 新增的文字未经 P4 术语与斜体规范 |
| R8 | **与上一轮矛盾**：本轮回复口径与 A3 中的承诺冲突 |

### 3.2 逐意见验收标准

| 意见 | 验收标准 | 验收方法 |
|---|---|---|
| 1 可读性 | §1 有显式双主线路线图；8 个二级小节均有主题句+take-home；仅读段首句可复原论证链；长句指标达标 | 人工反向验收 + 脚本 A |
| 2 巨噬细胞降调 | 摘要级分支相关句 **0 处**无条件机制性动词；篇幅降 ≥30%；Abstract/§3.3/§4.3/§6/Figure 4 图注/Table 1 **六处**均已同步；`claim_downgrade_log.csv` 逐处可追溯 | 脚本 D + 六处清单逐项打勾 |
| 3 措辞 | "therapeutic direction(s)" 全文统一；§6/§7 治疗表述 100% 条件式 | 脚本 E（grep + 情态动词检查） |
| 4 术语格式 | 种名/基因名斜体 100%；蛋白名正体 100%；缩写首现定义 100%；表与图注同步 | 脚本 B（零告警） |
| 5 新文献 | 2 条著录经 DOI 核验；各有 ≥1 处实质性正文讨论（非仅堆砌引用）；重编号后引用位全对 | DOI 核验记录 + 脚本 C |

### 3.3 可读性量化阈值（意见 1 专用）

| 指标 | 阈值 | 说明 |
|---|---|---|
| 单句词数 | 平均 ≤ 25 词；**>40 词的句子占比 ≤ 5%** | 现稿存在多个 50+ 词长句，是 AE "difficult to read" 的直接来源 |
| 段落词数 | >200 词的段落需逐个评估是否拆分 | |
| 每段主题句 | 100% 覆盖 | 段首第一句须能独立表达该段主旨 |
| 被动语态占比 | ≤ 30% | 综述可适度使用，但不应主导 |
| 连续从句嵌套 | ≤ 2 层 | |
| 主线锚定密度 | 每 500 词至少 1 处显式主线标识 | 直接回应 AE "difficult to extract" |

### 3.4 自动化核查脚本（P0 阶段一并建立）

| 脚本 | 名称 | 功能 | 输出 |
|---|---|---|---|
| A | `check_readability.py` | 句长分布、段长、被动语态、主题句缺失定位 | `readability_report.csv` |
| B | `check_format.py` | 逐 run 扫描种名/基因名斜体、蛋白名正体、缩写首现与一致性（**须覆盖正文+表格+图注+参考文献**） | `format_report.csv` |
| C | `check_citations.py` | 引用位与 `refs_map.csv` 交叉比对，检测断号、重号、区间引用越界、孤儿文献 | `citation_report.csv` |
| D | `check_hedging.py` | 扫描 (20) 相关段落中的强机制性动词（`increases`,`drives`,`reprograms`,`mediates`,`causes`,`establishes`,`demonstrates`,`shows that`）并标红 | `hedging_report.csv` |
| E | `check_terms.py` | 依 `terminology.csv` 做术语一致性替换核查 + "therapeutic direction" 措辞统一核查 | `terms_report.csv` |

> **技术要求**：脚本基于 `python-docx` 逐 `run` 处理以保留格式信息；`.doc` 旧格式需先转换。**禁止以纯文本方式处理后回写**，否则丢失全部格式与修订痕迹。

---

## 4. 交付物清单

| # | 交付物 | 格式 | 要求 |
|---|---|---|---|
| D1 | 返修稿（带修订痕迹） | .docx | Word 修订模式可见，可逐条接受/拒绝 |
| D2 | 返修稿（清稿） | .docx | 已接受全部修订 |
| D3 | 修改对照表 | .xlsx / .csv | 列：意见号、子项号、原文、改后文、章节、页、行 |
| D4 | 英文回复信 | .docx | 逐条回复，含页行号，模板见 §5.1 |
| D5 | 中文回复信 | .docx | 与 D4 内容对应，供作者内部核对 |
| D6 | 参考文献增补说明 | .md | 2 条新文献的核验记录与插入位置 |
| D7 | 术语总表 | .csv | `terminology.csv` |
| D8 | 自检报告 | .md | 脚本 A–E 输出汇总 + 逐意见验收打勾表 |
| D9 | 需改图清单 | .md | 图件内需同步修改的标签（若有） |
| D10 | 遗留问题与待确认事项 | .md | 所有 `【待作者确认】` 汇总 |

### 4.1 修订痕迹生成方案（三选一，按可得性降级）

| 方案 | 做法 | 优点 | 缺点 |
|---|---|---|---|
| **优选** | 在 A1 基础上**开启 Word 修订模式直接编辑**（或用 `python-docx` 写入 `w:ins`/`w:del` 标记） | 最符合期刊要求 | 程序化写入 track changes 较复杂，需严格验证 |
| **次选** | 用 Word/LibreOffice 的"比较文档"功能，对 A1 与 `manuscript_final_clean.docx` 生成差异稿 | 可靠、易实现 | 差异粒度可能过细，格式改动会大量显示 |
| **兜底** | 提交清稿 + **高亮标注版**（改动处黄色高亮）+ 详细修改对照表（D3） | 实现简单 | 部分期刊不接受，**需先确认 A4 要求** |

> **执行前必须确认 A4 中期刊对返修稿形式的要求**（tracked changes / highlighted / point-by-point only），不同期刊要求差异很大。

---

## 5. 回复信模板

### 5.1 英文回复信（Response to Reviewers）

```
Response to the Associate Editor

Manuscript ID: [    ]
Title: Lactate Dynamics at the Pseudomonas aeruginosa–Host Interface:
       Bacterial Metabolism, Host Defense, and Emerging Links to Histone Lactylation

Dear Dr. Mukherjee,

We thank you for the constructive assessment of our revised manuscript and for
the encouraging comment that the revisions have made the manuscript more focused
and better aligned with the topic. We have now addressed each of the remaining
points, and we believe the manuscript has been further improved as a result.

Below we respond point by point. Editor comments are in italics; our responses
follow in plain text. All page and line numbers refer to the tracked-changes
version of the revised manuscript.

────────────────────────────────────────────────────────────────────────
Comment 1. Overall clarity and readability
────────────────────────────────────────────────────────────────────────
[Verbatim comment]

Response:
We agree, and we thank the Editor for identifying the specific difficulty —
that the two major strands (bacterial lactate utilization and lactate-associated
changes in the infected host) were hard to extract. We have addressed this
without altering the section structure that was endorsed in the previous round.

Specifically, we have:
  (i)   added an explicit roadmap at the end of the Introduction that names the
        two strands and states where each is developed (p. X, lines X–X);
  (ii)  added navigational openings to Sections 3 and 4 (p. X, lines X–X; p. X,
        lines X–X);
  (iii) given each subsection a topic sentence and a closing take-home statement;
  (iv)  shortened long sentences throughout and reduced nominalization, lowering
        the proportion of sentences exceeding 40 words from X% to X%.

────────────────────────────────────────────────────────────────────────
Comment 2. Macrophage section
────────────────────────────────────────────────────────────────────────
[Verbatim comment]

Response:
We fully accept this point and have revised the macrophage section to present
the abstract-level findings explicitly as a research hypothesis rather than an
established mechanism.

  (i)   All mechanistic verbs applied to this branch have been changed to
        hypothesis-framing language (e.g., "increases" → "has been proposed to
        increase").
  (ii)  The branch is now introduced explicitly as a hypothesis awaiting
        full-length validation (p. X, lines X–X; p. X, lines X–X).
  (iii) Its length has been reduced by approximately X%, so that it no longer
        carries disproportionate weight.
  (iv)  The legend of Figure 4 now states that panel C is a hypothesis, not an
        established mechanism.
  (v)   The Abstract has been revised accordingly (p. X, lines X–X).
  (vi)  In addition, and as suggested in Comment 5, we have incorporated a
        recently published full-length review of macrophage glycolytic
        reprogramming in bacterial infection (Wang et al., Front Immunol 2026),
        which provides peer-reviewed support for this section and further
        reduces reliance on the abstract-level report.

A complete list of the individual wording changes is provided in the
accompanying table of revisions.

────────────────────────────────────────────────────────────────────────
Comment 3. Therapeutic directions
────────────────────────────────────────────────────────────────────────
[Verbatim comment]

Response:
We have adopted the suggested terminology. On reviewing the manuscript, we found
that this wording appeared in three places, and all have been revised:
  (i)   the Abstract (p. X, line X);
  (ii)  Section 6 (p. X, line X);
  (iii) the caption of Table 3 (p. X, line X).
We have also checked all therapeutic statements in Sections 6 and 7 to ensure
that each is expressed conditionally and that none implies established
preclinical support.

────────────────────────────────────────────────────────────────────────
Comment 4. Terminology and nomenclature
────────────────────────────────────────────────────────────────────────
[Verbatim comment]

Response:
We thank the Editor for this important point. We have standardized the
terminology throughout using the convention below, defined each abbreviation at
first appearance, and used it consistently thereafter:

  • lysine lactylation (Kla) — general chemical modification
  • histone lactylation — used only where histones are specifically meant
  • histone H3 lysine 18 lactylation (H3K18la)
  • L-lactyllysine (KL-la), D-lactyllysine (KD-la), Nε-carboxyethyllysine (Kce)
  • H3K18 acetylation (H3K18ac) — kept visually distinct from H3K18la

We have also italicized all scientific names throughout the manuscript,
including the title, Abstract, main text, tables, figure legends, and reference
list. Gene names are now italicized and protein names set in roman consistently,
in line with the convention already stated in the legend of Figure 2.

────────────────────────────────────────────────────────────────────────
Comment 5. Recently published research
────────────────────────────────────────────────────────────────────────
[Verbatim comment]

Response:
We thank the Editor for these suggestions. Both are relevant and have been
incorporated:

  • Mariano et al. (Burns 2026) has been added to Section 4.1 (p. X, lines X–X),
    where it provides clinical support for the association between
    Gram-negative quorum-sensing molecules and rising lactate, complementing the
    ex vivo burn-wound exudate data already discussed.
  • Wang et al. (Front Immunol 2026) has been added to Section [3.3/4.3]
    (p. X, lines X–X), where it frames macrophage glycolytic reprogramming in
    bacterial infection and, as noted under Comment 2, strengthens the
    peer-reviewed basis of the macrophage section.

────────────────────────────────────────────────────────────────────────

We hope these revisions address the remaining concerns and thank you again for
the careful and constructive handling of our manuscript.

Sincerely,
[Corresponding author] on behalf of all authors
```

### 5.2 中文回复信（作者内部核对用）

```
致副主编回复函

稿件编号：[    ]
题目：Lactate Dynamics at the Pseudomonas aeruginosa–Host Interface…

尊敬的 Mukherjee 副主编：

感谢您对返修稿的建设性评审，以及"修改后稿件更聚焦、更切题"的肯定。我们已逐条
处理剩余问题，认为稿件质量得到进一步提升。以下逐条回复，页码行号均对应带修订
痕迹版本。

【意见 1｜整体清晰度与可读性】
原文：……
回复：我们认同该意见，并特别感谢您指出了具体症结——细菌乳酸利用与感染宿主中
乳酸相关改变这两条主线不易提取。我们在不改动上一轮已获认可的章节结构的前提下
作了如下处理：
  (1) 在引言末新增双主线路线图，明确两条线各自展开的位置（第 X 页第 X–X 行）；
  (2) 在第 3、4 章章首新增导航性过渡段；
  (3) 为各二级小节补充段首主题句与节末要点句；
  (4) 全文拆分长句、压缩名词化结构，40 词以上句子占比由 X% 降至 X%。

【意见 2｜巨噬细胞部分】
原文：……
回复：完全接受。已将摘要级研究的相关内容明确改写为研究假设而非既定机制：
  (1) 该分支所有机制性动词改为假设性表述；
  (2) 明确标注为"有待全文发表验证的研究假设"（第 X 页第 X–X 行）；
  (3) 该分支篇幅压缩约 X%，避免权重失衡；
  (4) Figure 4 图注新增说明，panel C 为假设而非既定机制；
  (5) 摘要相应修改；
  (6) 并按意见 5 补充了已正式发表的巨噬细胞糖酵解重编程综述（Wang 等，
      Front Immunol 2026），为本节提供同行评议文献支撑，降低对摘要级报道的依赖。
逐处措辞改动详见随附修改对照表。

【意见 3｜治疗方向措辞】
原文：……
回复：已采纳。核查全文后发现该措辞出现于三处，均已修改：摘要（第 X 页第 X 行）、
第 6 章（第 X 页第 X 行）、表 3 表题（第 X 页第 X 行）。同时复核第 6、7 章全部
治疗相关表述，确保均为条件式语气，无任何暗示已有临床前证据支持之处。

【意见 4｜术语与命名规范】
原文：……
回复：感谢指正。已按统一规范标准化全文术语，并在首次出现处定义、其后一致使用：
  • lysine lactylation (Kla)｜histone lactylation｜H3K18la
  • L-lactyllysine (KL-la)、D-lactyllysine (KD-la)、Nε-carboxyethyllysine (Kce)
  • H3K18 acetylation (H3K18ac)——与 H3K18la 保持视觉区分
并已将全文（含题目、摘要、正文、表格、图注、参考文献）的物种拉丁名统一斜体，
基因名斜体、蛋白名正体，与 Figure 2 图注已声明的体例保持自洽。

【意见 5｜补充近期文献】
原文：……
回复：两篇均与本文高度相关，已全部采纳：
  • Mariano 等（Burns 2026）补入 4.1 节（第 X 页第 X–X 行），为革兰阴性菌群体
    感应分子与乳酸升高的关联提供临床侧证据，与已讨论的人源烧伤创面渗出液数据呼应；
  • Wang 等（Front Immunol 2026）补入 [3.3/4.3] 节（第 X 页第 X–X 行），为细菌
    感染驱动的巨噬细胞糖酵解重编程提供框架，并如意见 2 所述强化该节的文献基础。

再次感谢您对本稿的认真处理。

此致
敬礼

通讯作者（代表全体作者）
```

### 5.3 回复信撰写规范

| # | 规范 |
|---|---|
| 1 | **先致谢、再接受、后说明**——不辩解、不对抗；AE 本轮语气正面，务必保持配合姿态 |
| 2 | **每条回复必须给出具体页码与行号**，让 AE 无需搜索即可定位 |
| 3 | **原意见逐字引用**（英文信中用斜体区分），不得转述或简化 |
| 4 | **能做的全做，做了的说清**；对确实不做的（如本稿无）须给出科学理由，不得回避 |
| 5 | **不承诺稿件未实际完成的修改**（红线 R3） |
| 6 | **意见 2 与意见 5 的交叉引用**必须写出——这是本轮回复的最大加分点 |
| 7 | **意见 3 主动扩大执行范围**要写明（"我们核查全文发现出现于三处，均已修改"），显示系统性态度 |
| 8 | 中英文两版**内容严格对应**，避免中文版承诺多于英文版 |

---

## 6. 执行顺序与依赖关系

```
P0 资产校验
   ↓
P1 意见拆解（5 条 → 约 18–22 子项）
   ↓
P2 内容修改  ← 先做，否则润色成果被推翻
   ├─ P2-a 意见 2 降调（风险最高，优先）
   ├─ P2-b 意见 5 补文献 + 全文重编号
   └─ P2-c 意见 3 措辞统一
   ↓
P3 可读性重构（意见 1，工作量最大）
   ↓
P4 术语与格式规范（意见 4）  ← 必须在 P3 之后，覆盖新增文字
   ↓
P5 整体润色与复核
   ↓
P6 交付物生成（修订痕迹稿 + 中英文回复信）
```

**关键依赖**
- P2-b 的参考文献重编号**必须在 P3/P5 新增文字之前完成**，否则新文字中的引用会再次错位。
- P4 **必须在 P3 之后**：P3 产生的新句子同样含有种名、基因名、缩写。
- P6 的修订痕迹稿以 **A1 原稿**为比较基准，不是以中间版本。

---

## 7. 风险登记

| # | 风险 | 影响 | 缓解措施 |
|---|---|---|---|
| K1 | 参考文献重编号导致引用错位 | **高**（红线 R5） | 脚本 C 强制零告警；区间引用（如 "(18, 19, 77–79)"）逐条人工复核 |
| K2 | 意见 2 降调不足，AE 再次退回 | **高** | 六处同步清单逐项打勾；脚本 D 扫描强机制性动词；篇幅压缩量化到 ≥30% |
| K3 | P3 新增文字未经 P4 规范 | 中（红线 R7） | 强制执行顺序；P5 再跑一次脚本 B |
| K4 | 图件内标签需改但无源文件 | 中 | P4 输出"需改图清单"交作者，不自行处理 |
| K5 | 期刊返修稿形式要求不明（A4 缺失） | 中 | P0 Gate 强制确认；未确认时按 §4.1 三方案全部产出 |
| K6 | 新文献著录信息有误 | 中（红线 R1） | DOI/PubMed 逐字段核验并留存记录（D6） |
| K7 | 可读性改写削弱了证据分级的审慎表述 | 中（红线 R4、R6） | P5 专设"证据分级标注一致性"复核项 |
| K8 | 本轮口径与上一轮回复矛盾 | 中（红线 R8） | P1 强制与 A3 比对；A3 缺失时向作者索取 |

---

## 8. 附：执行者须知

1. **本稿的学术特色是"审慎"**——证据分级 T1–T3、"lactate-associated" 与 "lactylation-dependent" 的严格区分、§5 的方法学告诫，都是作者刻意构建的。所有修改**只能增强而不能削弱**这一特色。AE 的意见 2 正是要求把这份审慎进一步贯彻到巨噬细胞部分。
2. **AE 已明确表示稿件大有改善**，本轮属"最后一公里"。策略应为**全面接受、超额落实**，而非辩论。
3. **不要重写全文**。上一轮的结构与论证已获认可，大规模重排会引入新风险并可能触发第三轮评审。
4. 遇到任何需要作者判断的科学问题（如某处降调是否过度、某文献是否确实适合插入），**标记 `【待作者确认】` 并汇总至 D10**，不要自行决定。
