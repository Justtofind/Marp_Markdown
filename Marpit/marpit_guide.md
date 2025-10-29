# ✅ Marpit Markdown 从入门到精通 使用文档
> 支持 Marp CLI / Marpit API / VS Code Marp 插件

---

## 📌 目录

1. 什么是 Marpit？
2. 安装与环境准备
3. 基本用法
4. 分页与背景布局控制
5. 幻灯片主题与自定义样式
6. 高级功能（动画、背景、布局、脚注等）
7. 导出 PDF / PPTX / HTML
8. 最佳实践与常见错误
9. 示例模板（可直接复制使用）

---

## 1️⃣ 什么是 Marpit？

Marpit 是一个基于 Markdown 的 *幻灯片制作框架*，允许你通过 Markdown 写演示文稿，并导出：

✅ HTML  
✅ PDF  
✅ PPTX  

Marpit 核心理念：**让 Markdown 也能做出专业演示文稿**

---

## 2️⃣ 安装与环境准备

推荐使用 VS Code + Marp 扩展

### ✅ 安装步骤（任意方式）

| 方式 | 描述 |
|------|------|
| VS Code + Marp 插件 ✅推荐 | 实时预览 + 一键导出 |
| npm CLI | `npm install -g @marp-team/marp-cli` |
| Node API | 用于项目自动化集成 |

示例：安装 CLI
```bash
npm install -g @marp-team/marp-cli
```

---

## 3️⃣ 基本用法

### ✅ 分页基础语法

每张幻灯片使用 `---` 分隔：
```markdown
# 第 1 页标题
内容内容...

---

## 第 2 页
更多内容...
```

---

### ✅ 布局：垂直/水平居中
```markdown
<!-- _class: lead -->
# 居中标题
```

常用 class：

| class | 效果 |
|------|------|
| lead | 全屏大标题居中 |
| invert | 暗色主题 |
| two-column | 双栏布局 |

---

## 4️⃣ 背景与布局控制

### ✅ 背景图片
```markdown
<!-- _background: url('bg.jpg') -->
# 主标题
```

### ✅ 背景颜色
```markdown
<!-- _backgroundColor: #3498db -->
```

### ✅ 全局设置封面样式
```markdown
<!--
class: lead
backgroundColor: #222
color: white
-->
# 封面标题
副标题
```

---

## 5️⃣ 主题与自定义样式

### ✅ 使用内置主题
```markdown
---
marp: true
theme: default
---
```

官方主题：`default` / `gaia` / `uncover`

### ✅ 自定义 CSS
```markdown
<style>
section {
  font-size: 22px;
  background-image: linear-gradient(to right, #91eae4, #86a8e7, #7f7fd5);
}

h1 {
  color: #ffffff;
}
</style>
```

---

## 6️⃣ 高级功能

### ✅ 多栏布局
```markdown
<!-- _class: two-column -->
# 多栏示例
左侧内容

---

右侧内容
```

---

### ✅ 动画（Fragments）
```markdown
- 动画元素 { .fragment }
- 逐条显示 { .fragment }
```

---

### ✅ 引用脚注
```markdown
这是文本 [^1]

[^1]: 脚注内容
```

---

### ✅ 数学公式（支持 KaTeX）
```markdown
$$
F(x) = \int_a^b f(t) dt
$$
```

---

### ✅ 代码高亮
```markdown
```python
print("Hello Marpit")
```
```

---

## 7️⃣ 导出文档

### ✅ VS Code 导出
点击右上角 Marp 图标 → Export → 选择 PDF / PPTX

### ✅ CLI 导出
```bash
marp slides.md --pdf
marp slides.md --pptx
marp slides.md --html
```

---

## 8️⃣ 最佳实践与常见错误

| 错误 | 原因 | 解决办法 |
|------|------|------|
| 输出错位 | 未使用分隔符 | 检查 `---` |
| 样式不生效 | 未启用 marp | 顶部添加 `marp: true` |
| 中文换行混乱 | CSS 未设置字体 | 添加中文字体 family |
| PDF 输出背景丢失 | 未启用 print support | CLI 加 `--allow-local-files` |

---

## ✅ 9️⃣ 完整示例模板

```markdown
---
marp: true
theme: gaia
paginate: true
header: "Marpit 教程"
footer: "By ChatGPT"
---

<!-- class: lead -->
# Marpit 从入门到精通
副标题在这里

---

## 幻灯片示例

- 支持 Markdown
- 支持 PDF / PPTX 导出
- 支持主题和自定义样式

---

<!-- _backgroundColor: '#333' -->
# 深色页面示例
文本自动变亮

---

<!-- _class: two-column -->
## 左右分栏
左侧文字  
- A
- B

---

右侧内容  
图片 / 图表等

---

## 数学公式
$$
E = mc^2
$$

---

## 结束！
谢谢观看！
```

---

# 🎯 总结

| 级别 | 学习点 |
|------|------|
| 入门 | 分页、基本 Markdown、主题选择 |
| 进阶 | 背景、布局、分页控制、分页样式 |
| 高级 | CSS 定制、动画、PDF/PPTX 导出 |

---

如果你愿意，我还可以为你：

✅ 生成 Marp 幻灯片模板（公司/学校品牌）  
✅ 制作 PPTX 并直接导出可下载  
✅ 讲解 CSS 深层定制、主题打包  
✅ 教你如何用 Marpit 做学术汇报、课程演示
