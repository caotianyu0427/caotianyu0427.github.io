---
title: ''
summary: ''
date: 2024-01-01
type: landing

design:
  spacing: '5rem'

sections:
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |
        <div style="display:flex;gap:8px;justify-content:center;flex-wrap:wrap;margin:-2rem auto 0 auto;max-width:1200px;">
          <img src="/media/hero/AT8PASYNNERNTS0045-29-40cor_composite.jpg" alt="免疫荧光 — 多通道IF染色" style="height:280px;flex:1 1 200px;object-fit:cover;border-radius:8px;min-width:0;">
          <img src="/media/hero/AT8TS1021-21-40SNCOTHT.jpg" alt="免疫组化 — AT8/SNC/OTH" style="height:280px;flex:1 1 200px;object-fit:cover;border-radius:8px;min-width:0;">
          <img src="/media/hero/uncmtdpp61-29-40cor.jpg" alt="脑组织染色" style="height:280px;flex:1 1 200px;object-fit:cover;border-radius:8px;min-width:0;">
          <img src="/media/hero/hp61-20-10-1.jpg" alt="免疫组化 — 脑切片" style="height:280px;flex:1 1 150px;object-fit:cover;border-radius:8px;min-width:0;">
        </div>
    design:
      columns: '1'
      spacing:
        padding: ['1rem', 0, 0, 0]

  - block: resume-biography-3
    content:
      username: me
      text: |
        我的研究聚焦于开发基于剪接调控的 TDP-43 相关神经退行性疾病治疗策略。在约翰霍普金斯大学 Philip Wong 教授的实验室，我研究 TDP-43 功能缺失如何导致隐蔽外显子（cryptic exon）的异常包含，并最终引发神经退行性变。我的核心工作是开发一种嵌合治疗蛋白（CTR），该蛋白能够恢复 TDP-43 的剪接抑制功能，同时避免蛋白聚集的风险。通过 AAV 载体在小鼠模型中的递送，我已经证实了神经元拯救、行为恢复以及隐蔽外显子抑制的效果。目前，我正在推进基于转铁蛋白受体靶向 AAV 衣壳的人源化递送策略。

        我的长期目标是成为一名独立研究者，致力于开发针对 ALS（肌萎缩侧索硬化症）和 FTD（额颞叶痴呆）的剪接调控疗法，同时揭示 TDP-43 功能障碍与 tau 蛋白及 α-突触核蛋白病理之间的交互机制。

        **eRA Commons:** Tianyu &nbsp;|&nbsp; **实验室:** [Wong Lab](https://labs.pathology.jhu.edu/wong/) &nbsp;|&nbsp; **院系:** [病理学系，约翰霍普金斯大学医学院](https://www.hopkinsmedicine.org/pathology)
      button:
        text: 下载简历
        url: uploads/resume.pdf
      headings:
        about: ''
        education: 教育经历
        interests: 研究方向
    design:
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    id: research
    content:
      title: '🔬 研究方向'
      subtitle: ''
      text: |
        我的研究围绕理解和治疗 TDP-43 介导的神经退行性疾病展开，涵盖三个相互关联的主题：

        ---

        ### TDP-43 与隐蔽外显子生物学
        TDP-43 是一种关键的 RNA 结合蛋白，其功能缺失会导致隐蔽外显子的异常包含——这些通常被沉默的序列一旦表达，会导致 mRNA 降解或产生毒性蛋白。我研究 TDP-43 缺失如何驱动隐蔽外显子包含，以及这一过程如何在 ALS 和额颞叶痴呆等疾病中导致神经元脆弱性和死亡。

        ---

        ### 基于 AAV 的 ALS/FTD 基因治疗
        我的核心工作是开发嵌合 TDP-43 抑制因子（CTR）——一种工程化治疗蛋白，能够恢复 TDP-43 的剪接抑制功能而不会产生聚集风险。利用腺相关病毒（AAV）载体，我已在 FTD 小鼠模型中实现了广泛的脑内分布、神经元拯救、行为恢复和隐蔽外显子抑制。目前我正在推进基于转铁蛋白受体靶向 AAV 衣壳的人源化递送方案。

        ---

        ### 多蛋白病变与 Tau/α-突触核蛋白
        神经退行性疾病很少仅涉及单一病理蛋白。我研究 TDP-43 功能障碍如何与 tau 和 α-突触核蛋白病理相互作用——探索 TDP-43 功能缺失是否会使神经元对 tau 介导的毒性更加敏感，以及这些共病理如何导致阿尔茨海默病和路易体痴呆等疾病的临床异质性。
    design:
      columns: '1'

  - block: collection
    id: publications
    content:
      title: 📄 学术论文
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  - block: resume-awards
    id: awards
    content:
      title: 🏆 荣誉与奖项
      username: me

  - block: markdown
    id: memberships
    content:
      title: '🤝 学术组织'
      subtitle: ''
      text: |
        - **美国神经科学学会 (SfN)**，会员，2023 年至今
        - **美国基因与细胞治疗学会 (ASGCT)**，会员，2024 年至今
    design:
      columns: '1'

  - block: markdown
    id: cv
    content:
      title: '📋 个人简历'
      subtitle: ''
      text: |
        <a href="/uploads/resume.pdf" class="inline-flex items-center px-6 py-3 text-base font-medium text-white bg-primary-600 rounded-lg hover:bg-primary-700 transition-colors" download>
          📥 下载简历 (PDF)
        </a>
    design:
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: '📬 联系方式'
      subtitle: ''
      text: |
        **曹天雨，医学博士**
        博士后研究员
        Wong Lab
        病理学系
        约翰霍普金斯大学医学院

        **邮箱：** [tcao6@jh.edu](mailto:tcao6@jh.edu)

        **地址：** 720 Rutland Avenue, Baltimore, MD 21205, USA
    design:
      columns: '1'
---
