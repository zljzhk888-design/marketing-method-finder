# 营销方法导航 · Marketing Method Finder

把「不知道该怎么营销」变成一个有理由、可验证的行动选择，并直接生成简洁、图文并茂的分析网页。

## 能做什么

- 根据业务阶段、客户购买路径、增长卡点和资源约束，推荐一个优先营销方法。
- 用路径图、场景示意和实验时间线解释：先做什么、为什么、如何验证。
- 给出投入上限、观察窗口、业务指标和继续或调整的条件。
- 匹配当前环境中可用的专项营销 skills，衔接后续执行。
- 资料不全时，明确标注假设，先生成有用的初版。

## 安装到 Codex

需要 Git，以及支持本地 skills 的 Codex 环境。在终端执行：

```bash
git clone https://github.com/zljzhk888-design/marketing-method-finder.git ~/.codex/skills/marketing-method-finder
```

如果该目录已经存在，请先确认内容，避免覆盖自己的修改。安装后新开聊天，在可用 skills 中确认 `marketing-method-finder` 已被识别。自定义 skills 目录的环境请调整安装路径。

更新已通过上述方式安装的版本：

```bash
git -C ~/.codex/skills/marketing-method-finder pull --ff-only
```

## 使用

在 Codex 聊天中输入：

```text
使用 $marketing-method-finder，分析一个全新的 AI 剪辑软件应该怎么做 marketing，直接生成简洁、图文并茂的分析网页。
```

更具体的信息可以让结果更准确：

```text
使用 $marketing-method-finder 分析我的 AI 剪辑软件：
- 客户：每周发布多条口播的独立创作者
- 能力：删停顿、字幕、口播粗剪
- 阶段：刚上线，有 10 位试用用户，尚未付费
- 目标：一个月验证首批付费
- 资源：一人运营，每周 10 小时，预算 2000 元
请给出优先打法、验证实验，并生成简洁图文网页。
```

以上数字仅为输入示例，不是推荐门槛或效果承诺。

## 网页交付

默认包含一句话结论、增长路径图、推荐打法、第一轮实验、执行 skill，以及可展开的假设和资料依据。

有可用的 Sites 插件时，按其流程生成并交付托管网页；发布和访问权限由该环境的工具与用户授权决定。没有网站工具时，生成可本地打开的 HTML 文件。核心分析不强制依赖某个付费服务；托管、联网检索和专项 skills 需要相应工具可用。安装本 skill 本身不会自动安装这些工具。

[查看 AI 剪辑软件分析示例](https://ai-edit-marketing-nov02.sturdy-cake-4726.chatgpt.site/)

示例使用假设业务背景，不代表对某一真实产品的实测结论。生成报告的视觉效果与交付能力取决于运行环境。

## 文件结构

```text
marketing-method-finder/
├── SKILL.md                           # 判断与执行流程
├── agents/openai.yaml                 # Codex 展示信息
└── references/
    ├── method-map.md                  # 方法与专项 skill 匹配
    ├── web-report.md                  # 图文网页交付规范
    └── behavioral-marketing.md        # 行为科学书单与应用导航
```

## 行为科学资料

参考资料收藏包括 Thinking, Fast and Slow、Predictably Irrational、Nudge、How to Change、Noise、The Power of Experiments 等书，以及 Choiceology、Freakonomics Radio 等播客。完整清单见 [行为科学资料与应用](references/behavioral-marketing.md)。

这些资料用于提出「行为障碍 → 可能机制 → 干预 → 指标」的待验证假设。收藏不代表已读取全文；具体研究、数据与引文需要核实。仓库不包含书籍全文或播客音频，也不把心理学概念当作营销效果保证。

## 使用边界

不编造用户数据、转化率、评价或收益预测。不会因为选择了营销方法，就自动获得投放预算、发布内容、发送外联或修改账户的授权。已有明确的专项任务时，应直接使用相应 skill。

欢迎通过 Issues 反馈真实使用中的误判与改进建议，请避免提交客户隐私、素材或账户凭据。
