# 大语言模型部署

本仓库收录本人在 **《大语言模型部署》HW4** 中的成果：

- **实验报告**（PDF）：`report/大语言模型横向对比分析.pdf`
- **实验截图**（PNG/JPG，共 18 张）：存放于 `screenshots/` 目录

## 目录结构
.
├── report/
│   └── 大语言模型横向对比分析.pdf
└── screenshots/
    ├── qianwen/
    ├── chatglm/
    └── baichuan/

      
## 报告摘要

- **实验目标**  
  在 GPU Notebook（8 vCPU · 32 GB · 24 GB VRAM）上依次部署 **Qwen‑7B‑Chat、ChatGLM3‑6B、Baichuan2‑7B‑Chat** 三款中文 LLM，使用 5 道歧义/套嵌问题进行横向测试。

- **关键发现**  
  1. *ChatGLM3‑6B* 回答最完整，但篇幅偏长；  
  2. *Qwen‑7B‑Chat* 语气自然，复杂指代略保守；  
  3. *Baichuan2‑7B‑Chat* 显存最省，准确度需精调；  
  4. 性能‑准确率折中场景优先选 GLM；资源敏感场景可用 Baichuan + Few‑Shot。

- **结论**  
  见报告第 5 节，涵盖三模型优缺点、适用场景与改进方向。

