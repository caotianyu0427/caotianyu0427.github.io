---
title: "JuncForge"
summary: "用于小鼠基因组中隐秘外显子（CE）连接处检测的 qPCR 引物设计流程。"
date: 2025-06-01
tags:
  - 生物信息学
  - RNA 剪接
  - qPCR
links:
  - icon: brands/github
    url: https://github.com/caotianyu0427/JuncForge
    label: 代码
image:
  focal_point: Smart
---

## 简介

JuncForge 是一个计算流程，用于设计跨越隐秘外显子（CE）剪接连接处的 qPCR 引物对，适用于 RNA 剪接研究，包括 TDP-43 功能缺失与神经退行性疾病中隐秘外显子纳入等相关课题。

## 主要功能

给定标注了内含子中隐秘外显子的 GenBank 文件，流程将：

1. 定位 CE 特征及其左右连接处
2. 通过 Primer3 设计满足连接处跨越约束的引物对
3. 对基因组与 RefSeq mRNA 进行 pair-wise BLAST 筛选
4. 保留预期仅扩增含 CE 转录本的引物

## 技术栈

Python、Primer3、BLAST

## 链接

- GitHub: https://github.com/caotianyu0427/JuncForge
