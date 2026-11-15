---
theme: ./
layout: cover
title: 我的答辩
canvasWidth: 960
fonts:
  sans: Noto Sans CJK SC
  local: Noto Sans CJK SC
  provider: none
---

<div class="subtitle">项目答辩 · 2026</div>

# 在这里填写项目名称

<span class="cmr-tag">汇报人姓名　指导教师姓名</span>

---
layout: contents
title: 目录
subtitle: Contents
---

1. 研究背景 <small>Background</small>
2. 方案设计 <small>Design</small>
3. 实验结果 <small>Results</small>
4. 总结展望 <small>Summary</small>

---
layout: section
title: 方案设计
subtitle: Architecture Design
number: '01.'
quote: 工欲善其事，必先利其器
---

---
layout: default
title: 研究背景
---

## 当前问题

介绍研究对象、使用场景，以及需要解决的具体问题。

- 用一段文字说明现状
- 用证据解释问题的影响
- 标出本次工作的**核心目标**

---
layout: two-cols
title: 总体方案
---

## 设计目标

介绍方案的关键约束与设计原则。

- 性能要求
- 资源限制

::right::

<div class="cmr-panel">

## 方案组成

填写模块划分、接口关系与实现边界。

</div>

---
layout: image-right
title: 总体架构
---

## 系统组成

左侧解释主要模块与数据流，右侧替换自己的架构图。

**保留图例与接口名称。**

::right::

![替换为自己的图片](https://www.nvidia.com/content/dam/en-zz/Solutions/data-center/gb200-superchip/gb200-nvl72-og.jpg)

---
layout: image-left
title: 实验结果
---

## 结果分析

填写实验条件、比较对象和指标单位。

**结论需要与图表对应。**

::right::

![替换为自己的图片](https://developer.download.nvidia.com/images/isaac/nvidia-isaac-sim-og-1200x630.jpg)

---
layout: compare
title: 方案对比
---

<div class="cmr-panel">

## 基线方案

- 原始实现
- 主要限制
- 测试条件

</div>

::right::

<div class="cmr-panel">

## 改进方案

- 修改内容
- 测量结果
- 适用范围

</div>

---
layout: process
title: 研究方法
---

<CmrSteps :items="[{title:'建立基线',text:'固定测试环境并记录初始指标。'},{title:'控制变量',text:'每轮修改一个因素，运行相同测试。'},{title:'分析结果',text:'比较性能与资源开销，形成可验证的结论。'}]" />

---
layout: end
---

<div class="subtitle">THANK YOU FOR WATCHING</div>

# 感谢观看

<span class="cmr-tag">欢迎提问</span>
