# 机器人运动与代数几何参考文献（2025–2026）

整理日期：2026-10-28。收录六篇文献，覆盖机器人逆运动学、轨迹认证、空间闭环机构、机构综合、高阶奇异性与自运动。

当前含 **4 篇全文 PDF** 和 **2 篇仅引用条目**。PDF 为 arXiv 或作者公开稿，已解析文件结构并核验首页题名、作者与页数；作者稿页数可能不同于正式出版排版。

统一引用文件：[references.bib](references.bib)；来源、版本、页数与 SHA-256：[references.json](references.json)。

| 编号 | 文献 | 作者 | 出版信息 | 本地全文 / 引用 |
|---|---|---|---|---|
| 1 | [Inverse Kinematics for a 7-Degree-of-Freedom Robot Manipulator Using Comprehensive Gröbner Systems](https://doi.org/10.1007/978-3-032-34586-8_11) | Rikita Komatsuzaki; Akira Terui; Masahiko Mikawa | Computer Algebra in Scientific Computing, CASC 2026, 2026；上线 2026-08-09 | [引用与 DOI](2026_Komatsuzaki_Terui_Mikawa_CGS_7DOF.reference.md)；全文未取得 |
| 2 | [Trajectory Planning and Certification for 3-DOF Robot Manipulators Using Real Quantifier Elimination Based on Comprehensive Gröbner Systems](https://arxiv.org/abs/2607.11657) | Yu Nakai; Akira Terui; Masahiko Mikawa | arXiv, 2026；上线 2026-07-13 | [PDF，9 页](2026_Nakai_Terui_Mikawa_Trajectory_Planning_Certification_3DOF.pdf) |
| 3 | [A study on design optimisation of a spatial, cable-actuated variable stiffness joint](https://doi.org/10.1016/j.mechmachtheory.2026.106394) | Isaac John; Santhakumar Mohan; Philippe Wenger | Mechanism and Machine Theory, 2026 | [引用与 DOI](2026_John_Mohan_Wenger_Cable_Actuated_Joint.reference.md)；全文未取得 |
| 4 | [Kinematic Synthesis over Curves Using Cellular Decompositions and Chebyshev Interpolants](https://doi.org/10.1007/978-3-032-10510-3_5) | Silviana Amethyst; Jonathan D. Hauenstein; Charles W. Wampler | Advances in the Mathematics of Robotics, IMA 2025, 2026；上线 2026-05-01 | [PDF，10 页](2026_Amethyst_Hauenstein_Wampler_Kinematic_Synthesis_over_Curves.pdf) |
| 5 | [Sixth-order Singularities of the 3RR Planar Pentad Mechanism](https://doi.org/10.1007/978-3-032-10510-3_17) | Charles W. Wampler; Manfred Husty; Jonathan D. Hauenstein | Advances in the Mathematics of Robotics, IMA 2025, 2026；上线 2026-05-01 | [PDF，8 页](2026_Wampler_Husty_Hauenstein_Sixth_order_Singularities_3RR.pdf) |
| 6 | [Finding mechanisms of exceptional mobility using numerical algebraic geometry](https://doi.org/10.1016/j.mechmachtheory.2025.106033) | Charles W. Wampler; Mark Plecnik | Mechanism and Machine Theory, 2025 | [PDF，38 页](2025_Wampler_Plecnik_Exceptional_Mobility.pdf) |

## 研究内容

1. **Komatsuzaki2026CGS7DOF**：预先指定一个关节角处理七自由度机械臂冗余，并利用预计算的综合 Gröbner 系统复用不同末端位姿下的逆运动学求解。
2. **Nakai2026TrajectoryCertification**：结合综合 Gröbner 系统与实量词消去，求解三自由度机械臂逆运动学，并认证线段与三次自然样条路径上每一点的逆解存在性。
3. **John2026CableJoint**：利用多项式同伦延拓求解空间缆驱机构的闭环约束，获得多组逆运动学解，并进一步开展工作空间、刚度与设计优化研究。
4. **Amethyst2026KinematicCurves**：对机构设计约束定义的实代数曲线进行数值胞腔分解，以同伦跟踪曲线分支，再用 Chebyshev 插值进行优化；包含四杆机构综合实例。
5. **Wampler2026SixthOrder**：研究与平面并联机器人正运动学相关的装配解如何合并成六重根，涉及高阶奇异位形、数值代数几何、Dixon 行列式与参数同伦。
6. **Wampler2025ExceptionalMobility**：利用纤维积与数值代数几何寻找异常自由度机构，涵盖超约束机构和机器人自运动，研究连续运动解集的出现。

## 版本与引用说明

- 第 1 篇出版社页面的首次上线日期为 2026-08-09，而推荐引用年份标为 2027。目录按上线年份标记 2026，BibTeX 保留出版社当前推荐的 2027 年，并在 note 字段记录差异。
- 第 2 篇为 arXiv v1 预印本；第 4、5、6 篇 PDF 为作者公开稿。正式出版物信息与所存 PDF 版本分别记录在 JSON 中。
- 第 1、3 篇保留官方 DOI 和引用记录；取得全文后可在此目录补充 PDF，并更新 JSON 中的状态与校验值。
