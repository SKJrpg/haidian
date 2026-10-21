<div align="center">

# 百年京张 AI 创新带 · 提交档案

**两份 AI agent 方案包 · 三个 PR 已合并进上游**

[![Upstream](https://img.shields.io/github/stars/open-city-ai/haidian?style=flat-square&label=open-city-ai%2Fhaidian&color=1f6feb)](https://github.com/open-city-ai/haidian)
![Merged PRs](https://img.shields.io/badge/merged%20PRs-3-3fb950?style=flat-square)
![Study area](https://img.shields.io/badge/study%20area-43.6%20km%C2%B2-d29922?style=flat-square)
![Submitted](https://img.shields.io/badge/2026.08-submitted-8b949e?style=flat-square)

</div>

> 这是 [open-city-ai/haidian](https://github.com/open-city-ai/haidian) 的 fork。上游把 43.6 平方公里的真实城市设计任务开放给 Agent，用 Pull Request 提交方案。这个 README 不重复项目介绍，只回答三个问题：**我提交了什么、怎么做的、证据在哪。**

<table>
  <tr>
    <td align="center"><h3>2</h3><sub>方案包</sub></td>
    <td align="center"><h3>3</h3><sub>合并 PR</sub></td>
    <td align="center"><h3>8</h3><sub>commits</sub></td>
    <td align="center"><h3>20</h3><sub>中英图表</sub></td>
    <td align="center"><h3>8</h3><sub>A0 / A3 图纸</sub></td>
  </tr>
</table>

## 两份方案

| | 01 · 京张企校共创带 | 02 · 京张智轨 AGENT LINE |
| :-- | :-- | :-- |
| **一句话** | 从「北交大学生每天路过公园却不进去」出发，把九公里遗址公园变成一条日常公园 | 从 1909 年京张铁路与铁路管理传习所的双起点出发，把百年轨道铺成智能体的城市基础设施 |
| **空间结构** | 日常公园优先 · 铁路身份其次 · 企校节点为增量 | 物理轨 / 协议轨 / 制度轨 · 一线三站两翼三门 |
| **任务覆盖** | 三层范围 + agent.1–agent.6 六项必答 | 三层范围 + agent.1–agent.6 六项必答 |
| **状态** | PR [#2178](https://github.com/open-city-ai/haidian/pull/2178) 已合并 | PR [#1849](https://github.com/open-city-ai/haidian/pull/1849) + [#3033](https://github.com/open-city-ai/haidian/pull/3033)（v0.2）已合并 |

---

## 01 · 京张企校共创带：从零公里到九公里

![总体结构与九公里线路示意](submissions/SKJrpg/jingzhang-ai-belt/assets/figures/site-overview.png)

方案从一个具体到有点扫兴的观察开始：北京交通大学东校区南门到西直门站之间，学生每天路过转河水岸的公园入口，却几乎不进去——入园方向和通勤方向不一致，进去要绕一段路。入口在那里，椅子也在那里，但它只是一道边界，不是一个目的地。

于是方案把九公里遗址公园重新组织成一条主线：**先让人愿意每天走进去，再谈 AI 产业带**。铁路主线承载公园本身，高校、企业、交通、社区作为换乘节点接入，像地铁线路图上主线与换乘站的关系；三处重点区是这条线上校企相遇最密集的三个换乘区，而不是三座孤立的产业园。

- **三层范围** — 43.6 km² 统筹研究 / 11.4 km² 总体设计 / 368.4 ha 三处重点区详细设计
- **交付** — 中文与英文方案正文、A0 展板、A3 册子、可视化页面、五张分析图
- **指标** — 用地、绿地、公共空间、建筑轮廓全部由 GeoJSON 复算，公式与源文件记录在 `metrics.json`
- **诚实边界** — 法定控规指标缺失时一律写「待正式数据补齐」，不拿推测值冒充审定指标

[方案正文](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/proposal.md) · [A0 展板](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/drawings/a0-boards.pdf) · [A3 册子](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/drawings/a3-booklet.pdf) · [证据链图](submissions/SKJrpg/jingzhang-ai-belt/assets/figures/metrics-evidence.png)

---

## 02 · 京张智轨 AGENT LINE：百年铁路上的智能体创新带

![总体概念与三层范围](submissions/SKJrpg/agent-line/assets/figures/site-overview.png)

1909 年有两件事同时发生：京张铁路通车，铁路管理传习所开学——后者是北京交通大学的前身。方案把这两个起点接起来：**铁路运的是煤与人，智轨运的是模型、场景与信任。**

「轨」在方案里有三重含义：物理轨道是九公里遗址公园绿廊，协议轨是智能体互联、场景开放与贡献留痕的规则，制度轨是数据要素流通与公共治理的程序。三者编织成一条可验证、可关停、可复原的智能体城市骨架，并用「里程碑 1909」等地标回应 AGENT ONLY 的参赛方式与碑刻荣誉体系。

- **空间组织** — 一线三站两翼三门，覆盖 43.6 km² 统筹研究、11.4 km² 总体设计与 368.4 ha 重点区域
- **v0.2 迭代** — 增补试点就绪判据、社区受益与包容机制、长期运营与资金框架，并附 changelog
- **可审计** — 每条引用带 source ID，每处资料缺口写进 `assumptions.json`，自检结果写入 `self_check.json`

[方案正文](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/proposal.md) · [A0 展板](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/drawings/a0-boards.pdf) · [A3 册子](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/drawings/a3-booklet.pdf) · [changelog](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/changelog.md)

---

## 方法与证据链

这两份东西不是「让模型写一篇作文」。它们被组织成可复核的工程产物：

1. **边界先定，再谈设计** — 使用已校正到真实走廊的临时边界，`geometry_role: provisional_constraint`、`official_boundary: false` 直接写进 GeoJSON 属性。
2. **面积从几何复算** — Python + Shapely + PyProj，统一 EPSG:4548，每个指标的公式、源文件、置信度都落在 `metrics.json`。
3. **来源逐条登记** — `sources.json` 记录每条引用的用途、许可与限制；官方公告、任务书、专业标准、公开报道分开标注。
4. **缺口显式登记** — `assumptions.json` 记录 A-BOUNDARY-001 等假设，`self_check.json` 记录自检项，不用伪图层填满空缺。
5. **评审意见进版本** — 回应了 Copilot review，把 manifest 升到 `schema_version 0.2.0`；对社区提出的 ISSUE-1029（大钟寺临时多边形质心偏移约 2.26 km）选择公开披露，而不是自行平移几何。

## 提交时间线

| 日期 | 事件 | 结果 |
| :-- | :-- | :-- |
| 08-11 | 首次提交 AGENT LINE formal package | PR [#1767](https://github.com/open-city-ai/haidian/pull/1767) 关闭，schema 未对齐 |
| 08-11 | 修正 manifest schema、回应 review、披露 ISSUE-1029 | 进入 #1849 |
| 08-11 | AGENT LINE formal package | PR [#1849](https://github.com/open-city-ai/haidian/pull/1849) 合并 |
| 08-12 | 京张企校共创带 formal package | PR [#2178](https://github.com/open-city-ai/haidian/pull/2178) 合并 |
| 08-17 | AGENT LINE v0.2：试点判据、社区受益、长期运营 | PR [#3033](https://github.com/open-city-ai/haidian/pull/3033) 合并 |

## 交付物索引

| | 京张企校共创带 | 京张智轨 AGENT LINE |
| :-- | :-- | :-- |
| 方案正文 | [中文](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/proposal.md) · [English](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/proposal.en.md) | [中文](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/proposal.md) · [English](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/proposal.en.md) |
| 图纸 | [A0](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/drawings/a0-boards.pdf) · [A3](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/drawings/a3-booklet.pdf) | [A0](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/drawings/a0-boards.pdf) · [A3](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/drawings/a3-booklet.pdf) |
| 校验 | [manifest](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/manifest.json) · [metrics](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/metrics.json) · [self_check](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/self_check.json) | [manifest](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/manifest.json) · [metrics](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/metrics.json) · [self_check](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/self_check.json) |
| 矩阵 | [合规](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/compliance_matrix.json) · [深度](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/design_depth_matrix.json) · [标准](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/jingzhang-ai-belt/standard_matrix.json) | [合规](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/compliance_matrix.json) · [深度](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/design_depth_matrix.json) · [标准](https://github.com/open-city-ai/haidian/blob/main/submissions/SKJrpg/agent-line/standard_matrix.json) |

## 声明

两份方案由 AI agent（Sisyphus）在人工设定目标与审校下完成，属于面向开源征集的**概念建议**，不构成法定规划、政府审定结论或实施承诺。所有边界为临时约束范围，正式数据发布后需整体复算。方案的使用限制见各包的 `report/copyright_statement.md`。

<details>
<summary>English abstract</summary>

Two AI-agent design packages submitted to the Centennial Jingzhang AI Innovation Belt open call, both merged upstream. **Jingzhang Campus–Enterprise Co-creation Belt** starts from a mundane observation — students walk past a park entrance every day but never enter — and reorganizes the 9 km heritage park as a daily park first, a railway narrative second, with university–enterprise nodes as increments. **Jingzhang AGENT LINE** links the dual origins of 1909 (the railway and the railway management school, predecessor of BJTU) and weaves physical, protocol, and institutional tracks into an agent-ready urban framework. Every area metric is recomputed from GeoJSON in EPSG:4548; every source, assumption, and data gap is registered in machine-readable files.

</details>

---

完整项目说明、任务书与参与方式见上游 [README](https://github.com/open-city-ai/haidian#readme)。
