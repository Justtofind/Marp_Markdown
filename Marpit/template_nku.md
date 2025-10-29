---
marp: true
theme: default
paginate: true
headingDivider: 2
footer: "南开大学 · 学术汇报"
style: |
  section {
    font-family: 'Helvetica', 'Microsoft YaHei', sans-serif;
    background-color: #ffffff;
  }
  h1, h2, h3 {
    color: #4B116F; /* 南开大学主题紫 */
  }
  header {
    content: "南开大学";
    position: absolute;
    top: 10px;
    left: 20px;
    font-size: 16px;
    color: #4B116F;
  }
  footer {
    position: absolute;
    bottom: 10px;
    right: 20px;
    font-size: 14px;
    color: #6c6c6c;
  }
  img.nku-logo {
    width: 80px;
    position: absolute;
    right: 30px;
    top: 20px;
  }
---

<!-- class: lead -->
<img class="nku-logo" src="https://upload.wikimedia.org/wikipedia/commons/5/5c/Nankai_University_Logo.svg" />

# 🎓 学术报告标题
## 副标题 / 课题名称
**姓名**  
南开大学 · 学院名称  
指导教师：XXX  
报告日期：2025.xx.xx

---

## 内容提要 Outline
- 研究背景
- 文献综述
- 方法与模型
- 实验与结果
- 结论与展望

---

## 研究背景与意义
- 研究问题简介
- 现有方案不足
- 学术与应用价值

> 可加入图示辅助说明

---

## 文献综述
引用方式示例：

- Zhang et al. (2022)：图像分类，数据集较小
- Li et al. (2023)：Transformer 优势明显但成本高

| 作者 | 年份 | 方法 | 局限性 |
|------|------|------|------|
| Zhang | 2022 | CNN | 数据集单一 |
| Li | 2023 | Transformer | 计算开销大 |

---

## 方法与模型
### 模型框架
![width:500px](images/model.png)

数学公式示例：

$$
\mathop{\arg\min}_{\theta} \sum_{i=1}^{n}\|y_i - f(x_i;\theta)\|^2 + \lambda\|\theta\|_2^2
$$

---

## 实验设计
- 数据集说明
- 实验变量设置
- 评价指标选择

---

## 实验结果
<!-- _class: two-column -->

### 左侧结论总结
- 指标全面提升
- 模型稳健表现
- 可解释性更强

---

![width:300px](images/accuracy.png)

---

## 消融实验
逐步展示：

- 只用特征 A（Acc: 80%） {.fragment}
- 特征 A+B（Acc: 87%） {.fragment}
- 本方法全部加入（Acc: 92%） {.fragment}

---

## 结论与未来工作
✅ 已实现创新贡献  
✅ 提升性能  
✅ 推动应用落地

🔮 后续研究方向：
- 扩大数据规模
- 改善实时性能
- 结合大模型

---

<!-- class: lead -->
# 🙏 致谢
感谢导师、团队与评审老师

---

<!--
class: hidden
paginate: false
-->
# 备份页 / Q&A
可在答辩问答时使用