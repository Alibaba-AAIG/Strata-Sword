# Strata-Sword: A Hierarchical Safety Evaluation towards LLMs based on Reasoning Complexity of Jailbreak Instructions

**Strata-Sword** 是阿里巴巴 **AAIG** 团队提出的一种多级安全评测基准，旨在更全面地评估模型在面对不同思考复杂度下的安全能力，帮助模型开发者更好地理解不同模型的安全边界。


![Strata Logo](./assets/strata_sword_intro.png) 


---

## 🧩 我们的方案 — Strata-Sword


### 核心内容

1. **推理复杂度作为安全评估维度**  
   定义并量化“推理复杂度”作为可评估的安全维度，并根据推理复杂度的三个关键要素将不同的有害越狱指令划分为：基础指令、简单推理和复杂推理这三个不同的层级。

2. **分级越狱评测集构建**  
   将15种不同的越狱攻击方法按照推理复杂度划分成3个不同的等级，并总计包括700条越狱指令集。

3. **具有语言特色的越狱攻击方法**  
   Strata-Sword还考虑了语言特性，针对中文和英文分别定制了攻击方法，并首次引入了三种具有中文特色的越狱攻击方法，包括藏头诗攻击、猜灯谜攻击、和汉字拆解攻击。 


### 评测结果
   对当前23种主流的开源大语言模型和闭源商用模型进行系统性评估，从推理复杂度的角度对模型的安全能力边界进行刻画。 
![Strata Logo](./assets/strata_sword_result.jpg) 

   对Strata-Sword所采用的15种越狱攻击方法进行统计，评价每一种攻击方法的综合性能。 
![Strata Logo](./assets/strata_sword_attack_performance.jpg) 



## 🚀 快速上手

### 1. 环境安装：安装你所需要的环境

```bash
pip install -r requirements.txt
```

---

### 2. 测试：测试stata-sword三个等级的中英文越狱指令集
```bash
python strata_sword.py
```




## 📚 引用本工作
如果您在研究中使用了 Strata-Sword，请引用以下论文：
```bash
@article{Strata-Sword,
  title={Strata-Sword: A Hierarchical Safety Evaluation towards LLMs based on Reasoning Complexity of Jailbreak Instructions},
  author={Alibaba AI Group(AAIG)},
  year={2025},
  url={https://github.com/Alibaba-AAIG/Oyster}
}
```
---
## 🤝 参与贡献
我们欢迎安全评测和对齐方向的合作与讨论：
红队工作是一个持续不断的工作，strata-sword会在未来持续推出新的版本！
我们欢迎有更多大模型红队开发人员集思广益，不断地将提出的越狱攻击方法，并加入到我们的strata-sword的后续评测集中！
除此之外，也欢迎大家提交 Issue 报告问题，并在 Discussions 中交流想法！

---
## 📄 License
本项目遵循 Apache 2.0 License。

---
##  🙏 致谢
我们感谢开源社区和推动人工智能安全的研究人员。

Strata 是阿里巴巴 AAIG 对负责任的人工智能承诺的一部分。

“The LLM is my oyster, which I with sword will open.” 大模型是我的牡蛎，我将用剑打开它。
