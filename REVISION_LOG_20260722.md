# 学位论文图表与章节整合记录（2026-07-22）

## 安全备份

- 修改前完整工程：`F:\wyj\毕业论文\backups\overleaf_thesis_current_20260722_210410`
- 备份包含修改前的正文、整页截图、英文原图和参考文献文件。

## 正文章节

- `chapters/03_zeroshot.tex`：方法框架切换为中文解释版，保留模型名、数据集名和提示词。
- `chapters/04_attrip.tex`：AttriPrompter 总体框架、提示排序及跨域图切换为中文解释版；研究对象中的英文 prompt 不翻译。
- `chapters/05_vistex.tex`：补入 MSCOCO FSOD、GFSOD、医学开放集迁移和组件消融的原生 LaTeX 表格；补入医学迁移、注意力与定性结果独立图；扩充实验分析。
- `chapters/06_lungai.tex`：按在投论文重写研究设计、预处理、多尺度分类、GLIP 渐进式细胞检测、AI-RVT 一致性、DFS/OS 与免疫细胞联合分层；补入队列表及八组独立科研图。
- `chapters/08_appendix.tex`：移除“整页论文截图扩页”的组织方式，改为独立补充图、原生表格、失败案例和复现约定。

## 中文图

- `paper2592_method_zh.png`：第三章零样本核检测框架。
- `xu1_zh.png`、`xu2_zh.png`、`xu5_zh.png`：第四章 AttriPrompter 关键图。
- `method_zh.png`：第五章 VisTex-OVLM 框架。
- `lung_image2_zh.png`：第六章 AI-RVT/VIS-RVT 一致性。
- `lung_image5_zh.png`：第六章免疫细胞空间密度分析。
- `lung_image6_zh.png`：第六章淋巴细胞/中性粒细胞联合分层。
- `lung_image7_zh.png`：第六章研究设计。
- `lung_image8_zh.png`：第六章多尺度模型和细胞检测流程。

英文原图均保留。复杂统计图中的实验变量缩写、队列名、细胞类别和数值保持原文，避免翻译过程改变曲线或统计事实。

## 删除的错误截图

删除 `figures/` 下 13 张包含小论文正文、页眉页脚或整页表格的截图，以及未使用的 `lung_contact_sheet.jpg`。它们仍可从完整工程备份中恢复。

## 参考文献

- 新增 `paper_refs.bib`，仅收录正文实际使用而原主文献库缺失的小论文引用。
- `main.tex` 改为加载 `ref,paper_refs`，避免原 `ref.bib` 与 `tmi_refs.bib` 的重复键导致 BibTeX 报错。

## 核对原则

- 表格数值直接取自小论文 LaTeX 源表，不从截图人工识别。
- 图像只使用独立源文件或中文解释版，不把含正文的论文页面当作插图。
- 作为算法输入的 prompt、数据集名、类别名和模型缩写原则上保留英文。
