# DM0022 · K12 Question Samples (Primary School) / K12 学科科目样例（小学）

**Dataset card / 数据集卡片** · Zovda sample dataset. This repository is the GitHub mirror of the card; the data files are hosted on Hugging Face — **[download the dataset / 下载数据集](https://huggingface.co/datasets/Zovda/dm0022-k12-question-samples-primary)**.

本仓库是数据集卡片的 GitHub 镜像，数据文件托管在 Hugging Face，**[点击下载 / download](https://huggingface.co/datasets/Zovda/dm0022-k12-question-samples-primary)**。

| Item / 项目 | Value / 值 |
|---|---|
| Dataset ID / 数据集编号 | DM0022 |
| Files / 数据文件 | 6 |
| Size / 数据体积 | 7.78 KB |
| Language / 语言 | zh, en |
| Tasks / 任务类别 | question-answering, text-generation |
| Hugging Face / 数据地址 | [dm0022-k12-question-samples-primary](https://huggingface.co/datasets/Zovda/dm0022-k12-question-samples-primary) |
| Provided by / 提供方 | Zovda |
| Contact / 联系邮箱 | lucas@zovda.com |

## Overview / 简介

Primary-school samples: 6 files and 18 questions across math, Chinese and English, covering four formats — single-choice, true/false, problem solving and sentence rewriting.

小学学段数学、语文、英语 3 科共 6 个样例文件、18 题，覆盖单项选择、判断、解答与句子改写 4 种题型。

## What's inside / 数据内容

- 6 JSONL files: math 3 (single-choice, true/false, problem solving — 9 questions), Chinese 2 (true/false, sentence rewriting — 6), English 1 (single-choice — 3).
- 6 个 JSONL 文件：数学 3 个（单选、判断、解答，共 9 题）、语文 2 个（判断、句子改写，共 6 题）、英语 1 个（单选，3 题）。
- Every item carries prompt, answer, solution steps, knowledge point and source.
- 每题含题干、答案、解题步骤、知识点与题源。

## Specifications / 规格

- Format: UTF-8 JSONL
- 格式：UTF-8 JSONL
- Scale: 6 files / 18 questions / 7.78 KB
- 规模：6 文件 / 18 题 / 7.78 KB
- QC: 18/18 items carry source and item number; problem-solving items include full step-by-step solutions
- 质检：18/18 题含题源与来源题号；解答题含完整解题步骤

## Suitable tasks / 适用任务

- Primary-school subject QA and problem-solving training
- 小学学科问答与解题训练
- Lower-grade benchmark construction
- 低学段评测集构建
- Knowledge-point tagging
- 题目知识点打标

## Files / 文件清单

Paths below are relative to the Hugging Face repository root. 下表路径相对于 Hugging Face 仓库根目录。

| # | File | Size |
|---|---|---|
| 1 | `dm0022/小学/数学/判断题/样例.jsonl` | 1.17 KB |
| 2 | `dm0022/小学/数学/单项选择题/样例.jsonl` | 1.38 KB |
| 3 | `dm0022/小学/数学/解答题/样例.jsonl` | 1.68 KB |
| 4 | `dm0022/小学/英语/单项选择题/样例.jsonl` | 1.16 KB |
| 5 | `dm0022/小学/语文/判断题/样例.jsonl` | 1.12 KB |
| 6 | `dm0022/小学/语文/句子改写题/样例.jsonl` | 1.27 KB |

## Download / 下载

The files are not stored in this repository. 数据文件不在本仓库内，请从 Hugging Face 获取。

- Dataset page / 数据集页面: https://huggingface.co/datasets/Zovda/dm0022-k12-question-samples-primary
- Direct file URL / 单文件直链: `https://huggingface.co/datasets/Zovda/dm0022-k12-question-samples-primary/resolve/main/<path from MANIFEST.csv>`

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="Zovda/dm0022-k12-question-samples-primary",
    repo_type="dataset",
    local_dir="./dm0022-k12-question-samples-primary",
)
```

```python
from huggingface_hub import hf_hub_download

hf_hub_download(
    repo_id="Zovda/dm0022-k12-question-samples-primary",
    repo_type="dataset",
    filename="<path from MANIFEST.csv>",
    local_dir="./dm0022-k12-question-samples-primary",
)
```

## Rights and disclaimer / 授权与声明

Every item is attributed to its source paper and item number. Samples demonstrate schema and data conventions; contact us for licensing at scale.

题目来源标注到具体试卷与题号。样例用于展示字段结构与数据规范；规模化商用授权请联系我们。

This dataset is shared to demonstrate data organisation, technical specifications and delivery structure. For formal licensing, large-scale access or custom production, contact lucas@zovda.com.

本数据集仅用于展示数据组织方式、技术规格与交付结构。正式授权、规模化取数与定制生产请联系 lucas@zovda.com。

## About Zovda / 关于 Zovda

Zovda builds, cleans, annotates and packages training data across video, audio, images, e-commerce image-text pairs, exam question banks, embodied AI and coding-agent corpora.

Zovda 提供多模态与文本训练语料的数据采集、清洗、标注与结构化交付服务，覆盖视频、音频、图像、电商图文、K12 与职业题库、具身智能、代码智能体等方向。

**Contact / 联系方式:** lucas@zovda.com
