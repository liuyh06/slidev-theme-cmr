---
theme: ./
layout: cover
class: nvidia-demo
title: 英伟达 NVIDIA
info: 英伟达公司与技术平台介绍，CMR 模板 10 页示例
canvasWidth: 960
aspectRatio: 16/9
colorSchema: light
transition: fade
fonts:
  sans: Noto Sans CJK SC
  local: Noto Sans CJK SC
  provider: none
---

<div class="nv-eyebrow">NVIDIA</div>

# 英伟达

<div class="nv-cover-sub">GPU、软件生态与 AI 计算平台</div>

<span class="cmr-tag">公司与技术概览</span>

<div class="nv-cover-line">认识图形计算背后的平台能力</div>

<!--
本演示介绍英伟达的技术与产品平台，主要采用具有历史确定性的事实和具体产品案例，避免将某代产品称为当前最新产品。
来源：https://www.nvidia.com/en-us/about-nvidia/
-->

---
layout: contents
class: nvidia-demo
title: 内容导航
subtitle: Company & Technology
---

1. 公司与技术沿革 <small>GPU · CUDA · 深度学习</small>
2. 加速计算平台 <small>芯片 · 系统 · 开发工具</small>
3. 应用与工作负载 <small>AI 数据中心 · 机器人仿真</small>
4. 开发与部署 <small>训练 · 优化 · 推理服务</small>

<!--
这四部分构成一条理解路径：先看公司如何发展，再看平台的组成，然后用产品与场景理解能力，最后区分训练、推理和部署流程。本页是演示结构，不代表英伟达的财报业务分部划分。
-->

---
layout: section
class: nvidia-demo
title: 加速计算
subtitle: Accelerated Computing
number: '01.'
quote: 将并行计算用于真实问题
---

<!--
英伟达以 GPU 为基础推进加速计算，通过软件、系统与行业应用扩大其使用范围。
来源：https://www.nvidia.com/en-us/about-nvidia/
https://developer.nvidia.com/cuda
-->

---
layout: default
class: nvidia-demo
title: 四个技术里程碑
subtitle: A history of accelerated computing
---

<div class="nv-timeline">
  <div><div class="nv-year">1993</div><h2>公司成立</h2><p>黄仁勋、Chris Malachowsky<br/>与 Curtis Priem 联合创立。</p><small>起点：3D 图形与多媒体</small></div>
  <div><div class="nv-year">1999</div><h2>GeForce 256</h2><p>推出 GeForce 256，<br/>推动 GPU 产品发展。</p><small>图形处理器走向大众</small></div>
  <div><div class="nv-year">2006</div><h2>CUDA</h2><p>开放 GPU 并行计算能力，<br/>拓展科学与工程应用。</p><small>GPU 的用途超出图形</small></div>
  <div><div class="nv-year">2012</div><h2>深度学习</h2><p>GPU 为 AlexNet 的<br/>突破性成果提供计算支持。</p><small>加速计算进入 AI 研究</small></div>
</div>

<div class="nv-takeaway">持续演进的主线：<strong>扩大 GPU 能够解决的问题范围</strong></div>

<!--
1993 年 4 月 5 日，Jensen Huang、Chris Malachowsky、Curtis Priem 创立 NVIDIA。1999 年推出 GeForce 256。2006 年公布 CUDA 架构。2012 年 NVIDIA GPU 支持 AlexNet 的突破。
来源：https://www.nvidia.com/en-us/about-nvidia/corporate-timeline/
https://www.nvidia.com/content/timeline/time_99.html
-->

---
layout: two-cols
class: nvidia-demo
title: 硬件与软件共同组成平台
subtitle: Computing infrastructure and developer ecosystem
---

<div class="nv-col-label">HARDWARE</div>

## 计算基础设施

<div class="nv-stack-row"><b>GPU</b><span>承担大规模并行计算</span></div>
<div class="nv-stack-row"><b>互连</b><span>连接 GPU，支持多卡协同</span></div>
<div class="nv-stack-row"><b>系统</b><span>组织计算、存储与散热</span></div>

<div class="nv-col-note">单颗芯片的能力，需要系统配合才能发挥。</div>

::right::

<div class="cmr-panel nv-software">
<div class="nv-col-label">SOFTWARE</div>

## CUDA 开发生态

<div class="nv-stack-row"><b>编程</b><span>C++、Python 等开发入口</span></div>
<div class="nv-stack-row"><b>库</b><span>复用 GPU 加速计算能力</span></div>
<div class="nv-stack-row"><b>工具</b><span>编译、调试与性能分析</span></div>

<div class="nv-col-note">软件把硬件能力变为可调用的应用能力。</div>
</div>

<!--
CUDA 是 NVIDIA 的加速计算平台。CUDA Toolkit 包含编译器、GPU 加速库、运行时及开发工具。GB200 NVL72 展示 GPU、CPU、NVLink 和系统设计的结合。左右两栏是为解释平台而整理的教学结构，不是英伟达官方产品分类。
来源：https://developer.nvidia.com/cuda
https://www.nvidia.com/en-us/data-center/gb200-nvl72/
-->

---
layout: image-right
class: nvidia-demo
title: GB200 NVL72：机架级计算
subtitle: A concrete example of system-scale design
---

<div class="nv-product-label">GRACE BLACKWELL</div>

## 多颗芯片协同工作

<div class="nv-metrics"><div><b>72</b><span>Blackwell GPU</span></div><div><b>36</b><span>Grace CPU</span></div></div>

<p class="nv-product-copy">通过 <strong>NVLink</strong> 互连与液冷设计，<br/>构建面向大模型的机架级系统。</p>

<div class="nv-col-note">关键不只在算力，也在 GPU 之间的数据交换。</div>

::right::

<figure class="nv-rack"><img src="https://www.nvidia.com/content/dam/en-zz/Solutions/data-center/gb200-superchip/gb200-nvl72-og.jpg" alt="英伟达官方 GB200 NVL72 液冷机架产品图"/><figcaption>NVIDIA GB200 NVL72 · 官方产品图</figcaption></figure>

<!--
GB200 NVL72 在一个液冷机架中连接 36 颗 Grace CPU 与 72 颗 Blackwell GPU，使用 NVLink 进行 GPU 互连。本页不引用在特定测试条件下得出的性能倍数。
产品与图片来源：https://www.nvidia.com/en-us/data-center/gb200-nvl72/
图片：https://www.nvidia.com/content/dam/en-zz/Solutions/data-center/gb200-superchip/gb200-nvl72-og.jpg
-->

---
layout: image-left
class: nvidia-demo
title: 机器人先在虚拟环境中验证
subtitle: Omniverse libraries & Isaac Sim
---

<div class="nv-product-label">PHYSICAL AI</div>

## 仿真连接算法与场景

- 构建包含机器人和传感器的场景
- 模拟物理行为，测试算法表现
- 生成可控的合成数据

<div class="nv-callout">Isaac Sim 基于 Omniverse 库，<br/>用于机器人仿真、测试与数据生成。</div>

::right::

<figure class="nv-sim"><img src="https://developer.download.nvidia.com/images/isaac/nvidia-isaac-sim-og-1200x630.jpg" alt="英伟达 Isaac Sim 官方机器人仿真场景图"/><figcaption>Isaac Sim · 官方仿真场景图</figcaption></figure>

<!--
Isaac Sim 基于 NVIDIA Omniverse 库，提供机器人仿真、测试和合成数据生成能力。它支持设置物理、机器人和传感器模型。本页描述仿真的用途，不主张仿真结果能完全替代实机测试。
来源：https://developer.nvidia.com/isaac/sim/
图片：https://developer.download.nvidia.com/images/isaac/nvidia-isaac-sim-og-1200x630.jpg
-->

---
layout: compare
class: nvidia-demo
title: 训练与推理的目标不同
subtitle: Two workloads in the AI lifecycle
---

<div class="cmr-panel nv-compare-panel">
<div class="nv-col-label">TRAINING</div>

## 训练：更新模型参数

<p>模型从数据和反馈中学习，<br/>逐步调整内部参数。</p>

<dl><div><dt>核心过程</dt><dd>计算误差，更新权重</dd></div><div><dt>关注指标</dt><dd>模型质量、训练时间</dd></div><div><dt>典型任务</dt><dd>预训练、微调</dd></div></dl>
</div>

::right::

<div class="cmr-panel nv-compare-panel nv-inference">
<div class="nv-col-label">INFERENCE</div>

## 推理：使用已训练模型

<p>模型处理新的输入，<br/>输出预测或生成结果。</p>

<dl><div><dt>核心过程</dt><dd>执行模型，生成结果</dd></div><div><dt>关注指标</dt><dd>延迟、吞吐与成本</dd></div><div><dt>典型任务</dt><dd>问答、识别、内容生成</dd></div></dl>
</div>

<!--
训练通过数据与误差反馈改变模型权重。推理使用已训练模型处理新输入。关注指标是本演示为便于理解而归纳，并非排他性定义：两者都关心正确性、资源和成本。
来源：https://www.nvidia.com/en-eu/glossary/ai-training/
https://developer.nvidia.com/cuda
-->

---
layout: process
class: nvidia-demo
title: 一个 AI 应用的开发路径
subtitle: An illustrative development workflow
---

<CmrFlow :items="['准备数据', '训练与微调', '优化与评估', '部署与运行']" />

::right::

<div class="cmr-panel"><h2>工具连接各个环节</h2><p>CUDA 与计算库提供底层能力，应用工具把它们组织成开发工作流。</p><p>评估与部署之间需要反复迭代。</p></div>

<!--
本页是示意性开发路径，不是 NVIDIA 唯一或强制规定的流程。CUDA 平台支持训练和推理等工作负载，CUDA Toolkit 提供编译器、库与开发工具；实际项目会在评估与部署之间反复迭代。
来源：https://developer.nvidia.com/cuda
https://www.nvidia.com/en-eu/glossary/ai-training/
-->

---
layout: radial
class: nvidia-demo
title: GPU 加速覆盖不同工作负载
subtitle: One computing platform, multiple application domains
---

<CmrRadial center="GPU 加速" :items="[{title:'人工智能',text:'训练神经网络与执行推理'},{title:'科学计算',text:'并行计算与数值模拟'},{title:'数据分析',text:'数据处理与分析加速'},{title:'机器人',text:'仿真、感知与策略学习'}]" />

<!--
来源：https://developer.nvidia.com/cuda
本页按应用领域归纳，不代表排他的产品或财报分部划分。
-->

---
layout: modules
class: nvidia-demo
title: 一个机架系统的组成
subtitle: GB200 NVL72 as a system-design example
---

<CmrModules :items="[{title:'计算',lines:['Blackwell GPU','Grace CPU']},{title:'GPU 互连',lines:['NVLink','NVLink Switch']},{title:'网络',lines:['机架外通信','集群协同']},{title:'内存与数据',lines:['GPU 高带宽内存','CPU 内存']},{title:'基础设施',lines:['液冷设计','供电与运维']}]" />

<!--
来源：https://www.nvidia.com/en-us/data-center/gb200-nvl72/
本页是按系统功能整理的概念模块，不是硬件接线图。
-->

---
layout: gallery
class: nvidia-demo
title: 软件生态的不同入口
subtitle: Development tools, libraries and frameworks
---

<section><h2>开发环境</h2><p>CUDA Toolkit<br/>编译器与运行时</p></section>
<section><h2>开发工具</h2><p>Nsight<br/>调试与性能分析</p></section>
<section><h2>计算库</h2><p>CUDA-X<br/>复用领域计算能力</p></section>
<section><h2>框架入口</h2><p>PyTorch 等框架<br/>调用 GPU 加速能力</p></section>

::right::

CUDA
<small>加速计算平台</small>

<!--
来源：https://developer.nvidia.com/cuda
本页使用普通文字展示软件名称，并非官方标识或商标图形。
-->

---
layout: chart-notes
class: nvidia-demo
title: 两类市场的历史收入变化
subtitle: FY2024–FY2025 · historical data, not current results
---

<CmrBars title="数据中心" unit="十亿美元" :max="120" :rows="[{label:'FY24',value:47.525,display:'47.525'},{label:'FY25',value:115.186,display:'115.186'}]" />
<CmrBars title="游戏" unit="十亿美元" :max="12" :rows="[{label:'FY24',value:10.447,display:'10.447'},{label:'FY25',value:11.350,display:'11.350'}]" />

::right::

<section><h2>数据中心</h2><p>FY2025 收入较 FY2024 明显增长，是当期收入增长的主要来源。</p></section>
<section><h2>游戏</h2><p>保持收入增长，但业务规模与数据中心不同。</p></section>
<section><h2>读图口径</h2><p>两张图分别采用独立刻度；条长不能跨图比较。</p></section>

::caption::

FY2025 截至 2025-01-26；FY2024 截至 2024-01-28。数据源：NVIDIA FY2025 10-K。

<!--
来源：https://www.sec.gov/Archives/edgar/data/1045810/000104581025000023/R25.htm
原始单位为百万美元，本页换算为十亿美元。数据中心：47525、115186；游戏：10447、11350。均为历史收入，不是性能测试数据或最新财务数据。
-->

---
layout: flow-snake
class: nvidia-demo
title: 仿真与实机之间的开发路径
subtitle: An illustrative robotics workflow
---

<CmrFlow snake :items="['导入机器人资产','配置物理场景','配置传感器','训练或接入策略','仿真测试与评估','实机验证与迭代']" />

::right::

## 仿真帮助提前发现问题

在可控场景中测试机器人行为，降低每次实验的组织成本。

**实机验证仍然必要**，需要评估仿真与现实的差异。

<!--
来源：https://developer.nvidia.com/isaac/sim/
本页是整理后的示意流程，不是 NVIDIA 规定的唯一流程。训练可以通过 Isaac Lab 等配套工具完成，Isaac Sim 用于仿真和测试。
-->

---
layout: icon-steps
class: nvidia-demo
title: 用实验评估加速效果
subtitle: A controlled evaluation loop
---

<CmrIconSteps :items="[{icon:'01',title:'固定基线',text:'记录硬件、模型和输入条件'},{icon:'02',title:'修改变量',text:'每轮只改变需要研究的因素'},{icon:'03',title:'测量结果',text:'同时记录质量、延迟和资源'},{icon:'04',title:'复核结论',text:'重复实验并检查适用范围'}]" />

::right::

<p>性能结论需要<strong>可比条件</strong>。</p>
<p>速度提升应当与<strong>质量、资源和成本</strong>一起解释。</p>

<!--
本页为演示作者整理的通用实验方法，不宣称为 NVIDIA 官方流程，也没有虚构性能数据。
-->

---
layout: chart-grid
class: nvidia-demo
title: 四类市场的历史收入概览
subtitle: FY2024–FY2025 · revenue in US$ billions
---

<CmrBars title="数据中心" unit="十亿美元" :max="120" :rows="[{label:'FY24',value:47.525,display:'47.525'},{label:'FY25',value:115.186,display:'115.186'}]" />
<CmrBars title="游戏" unit="十亿美元" :max="12" :rows="[{label:'FY24',value:10.447,display:'10.447'},{label:'FY25',value:11.350,display:'11.350'}]" />
<CmrBars title="专业可视化" unit="十亿美元" :max="2" :rows="[{label:'FY24',value:1.553,display:'1.553'},{label:'FY25',value:1.878,display:'1.878'}]" />
<CmrBars title="汽车" unit="十亿美元" :max="2" :rows="[{label:'FY24',value:1.091,display:'1.091'},{label:'FY25',value:1.694,display:'1.694'}]" />

::caption::

各图使用独立刻度；四类市场不含 OEM 与其他，不能据此相加得到公司总收入。数据源：NVIDIA FY2025 10-K。

<!--
来源：https://www.sec.gov/Archives/edgar/data/1045810/000104581025000023/R25.htm
原始数据单位为百万美元；展示时除以 1000。FY2025 截至 2025-01-26；FY2024 截至 2024-01-28。保留三位小数，不引用最新业绩或投资结论。
-->

---
layout: summary
class: nvidia-demo
title: 公司能力的整体视图
subtitle: Hardware, software and applications
---

## 计算基础

GPU 与互连构成并行计算系统。

## 软件生态

编译器、计算库和工具连接开发者。

## 应用落地

AI、科学计算与机器人使用不同组合。

::right::

<p><strong>并行计算</strong></p>
<p>开发与优化工具</p>
<p>面向场景的系统平台</p>

<!--
来源：https://www.nvidia.com/en-us/about-nvidia/
https://developer.nvidia.com/cuda
https://www.nvidia.com/en-us/data-center/gb200-nvl72/
本页是前文归纳，不是财报口径或市场排名。
-->

---
layout: end
class: nvidia-demo
---

<div class="nv-eyebrow">NVIDIA</div>

# 理解英伟达的三个视角

<div class="nv-closing-points"><span><b>GPU</b>提供并行计算</span><span><b>软件</b>连接开发者</span><span><b>系统</b>承载实际应用</span></div>

<span class="cmr-tag">感谢观看　欢迎交流</span>

<!--
本页是对前文硬件、软件和应用平台的归纳。
来源：https://www.nvidia.com/en-us/about-nvidia/
https://developer.nvidia.com/cuda
https://www.nvidia.com/en-us/data-center/gb200-nvl72/
-->
