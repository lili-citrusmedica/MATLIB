# 代数几何与机器人：三篇论文阅读清单

核验日期：2026-10-27。以下按“符号计算与认证 → 逆运动学实现 → 实时避障”排列。每条区分论文元数据、阅读建议与获取方式。配套引用见 [robotics-algebraic-geometry.bib](robotics-algebraic-geometry.bib)。

## 1. 参数化 Gröbner 系统与轨迹认证

**Trajectory Planning and Certification for 3-DOF Robot Manipulators Using Real Quantifier Elimination Based on Comprehensive Gröbner Systems**

- 作者：Yu Nakai；Akira Terui；Masahiko Mikawa。
- 日期与版本：2026-07-13，arXiv v1；此处按预印本引用，不推定已被期刊接收。
- 标识：[arXiv:2607.11657v1](https://arxiv.org/abs/2607.11657v1)；[DOI: 10.48550/arXiv.2607.11657](https://doi.org/10.48550/arXiv.2607.11657)。
- 开放获取：[arXiv PDF](https://arxiv.org/pdf/2607.11657)（已确认可访问，9 页）。
- 内容与关联：以末端位置为参数建立逆运动学方程，通过 comprehensive Gröbner systems（CGS）复用参数化计算，并结合实量词消去认证轨迹上各点存在逆运动学解。论文处理折线和三次自然样条，实现在 Risa/Asir 中。
- 阅读建议：先检查参数空间如何分层、特殊参数下解集如何改变，再区分“逐点存在解”与“存在连续关节轨迹”这两个命题；不能把前者直接当作后者。可将这些问题与特殊纤维、临界条件及消去计算联系起来，但这里的联系是学习建议，并非论文声称研究了临界理想或重数理想。
- 权利核验：arXiv 页面链接至 [arXiv non-exclusive license](https://arxiv.org/licenses/nonexclusive-distrib/1.0/license.html)。本次未确认授权在 GitHub 重新分发全文，因此仅提供官方链接，不收录 PDF 或 TeX 副本。

## 2. IK-Geo：从几何分解到多项式逆运动学

**IK-Geo: Unified Robot Inverse Kinematics Using Subproblem Decomposition**

- 作者：Alexander J. Elias；John T. Wen。
- 期刊：*Mechanism and Machine Theory*，209，105971，2025 年 7 月。
- 正式版：[DOI: 10.1016/j.mechmachtheory.2025.105971](https://doi.org/10.1016/j.mechmachtheory.2025.105971)；[出版社页面](https://www.sciencedirect.com/science/article/pii/S0094114X25000606)。
- 预印本：[arXiv:2211.05737](https://arxiv.org/abs/2211.05737)，初稿 2022-11-10，所核验版本 v3 为 2024-02-19；该版本早于 2025 期刊版，不视为逐字相同。
- 开放获取：[arXiv PDF](https://arxiv.org/pdf/2211.05737)（已确认可访问，19 页）；[作者项目代码](https://github.com/rpiRobotics/ik-geo)（论文内给出的仓库）。
- 内容与关联：把 6R 机械臂逆运动学分解为六类几何子问题；根据轴线关系使用闭式解或低维搜索。半角正切代换把相关子问题转成多项式系统，为比较几何求解、消去法与数值求根提供实际例子。
- 阅读建议：先复现一个子问题，再选一种机器人几何检查全部实解、奇异情况和数值误差；可与第 1 篇的符号认证思路对照。
- 权利核验：所核验 arXiv 页面链接至 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)，允许在满足署名等条件时再分发。此清单保留官方 PDF 链接，不复制全文；该许可核验针对 arXiv 版本，不自动套用于期刊排版版或项目代码。

## 3. 机器人距离场与任务优先级实时避障

**Real-time collision avoidance with robot distance fields in a task-priority framework**

- 作者：Andrea Govoni；Michela Cavuoto；Yiming Li；Sylvain Calinon；Gianluca Palli。
- 期刊：*Robotics and Autonomous Systems*，200，105394，2026 年 6 月。
- 标识：[DOI: 10.1016/j.robot.2026.105394](https://doi.org/10.1016/j.robot.2026.105394)。
- 开放获取：[出版社全文页面及 PDF 入口](https://www.sciencedirect.com/science/article/pii/S0921889026000679)。出版社检索记录标为 Open access / Creative Commons；本次未成功独立打开 PDF，也未核实具体 CC 子类型，因此不提供未经验证的直接下载地址、不收录全文。
- 内容与关联：使用 Bernstein 多项式距离场表示机器人连杆几何，以解析梯度构造环境与自碰撞避障任务，并放入任务优先级控制框架；论文报告 GPU 实现及多种机械臂平台实验。
- 阅读建议：关注距离场近似误差、定义域外延拓及其梯度对控制的影响。它能把多项式表示与实时控制连接起来，但不应把实验避障效果理解为全局代数安全认证。
- 预印本与代码：本次未核实与此 DOI 对应的独立开放预印本或作者代码仓库；不以其他距离场项目替代本论文实现。

## 使用与版本说明

- 本次归档为书目、原创阅读笔记与官方获取链接，没有提交出版社 PDF、预印本 PDF、TeX 源码或第三方代码。
- “可以免费阅读”与“允许在 GitHub 重新分发”分别核验；链接目标的版权与许可仍由原作者或出版方保留。
- BibTeX 将 IK-Geo 的期刊版和早期预印本分别记录，避免混淆年份与版本。
