# 营销方法导航 · Marketing Method Finder

输入业务情况，得到一份营销渠道决策与执行指南：KOL 要不要投、怎么选与合作；SEO 要不要做、先做哪些页面；Google Ads 是否适合、如何启动测试。默认交付简洁、图文并茂的网页，展开即可查看具体操作。

## 能做什么

- 根据阶段、客户、目标、预算与团队，逐项判断渠道“现在做 / 小额测试 / 暂缓 / 不适用 / 待核实”。
- 为推荐渠道提供筛选标准、执行步骤、素材与 brief、预算依据、责任角色、排期和停止条件。
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

默认包含优先级结论、渠道决策表、可展开的操作指南、预算分配、首轮排期、效果追踪与停止条件。缺少预算或数据时明确标注假设；不编造报价、关键词搜索量或广告资格。

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
    ├── channel-execution.md           # KOL、SEO、Google Ads 等执行要求
    └── stage-channel-framework.md     # 阶段判断与更多出海渠道
```

## 使用边界

决策采用“阶段证据 → 增长瓶颈 → 渠道选择 → 产品内目标动作”。除 KOL、SEO 和广告，还按需要比较产品发布/目录、垂直社区、Build in Public、视频、ASO、产品内传播、开源/集成与销售。不会只凭用户数量判断 PMF，也不会照搬固定佣金或历史案例收益。


不编造用户数据、转化率、评价或收益预测。不会因为选择了营销方法，就自动获得投放预算、发布内容、发送外联或修改账户的授权。已有明确的专项任务时，应直接使用相应 skill。

欢迎通过 Issues 反馈真实使用中的误判与改进建议，请避免提交客户隐私、素材或账户凭据。

## 联系作者 · Rika

- 推特 / X：[@Web3rika](https://x.com/Web3rika)
- 小红书：[Rika 的小红书](https://xhslink.cn/o/9dp4HKg0lqm)
- 微信：`wincrypto`

欢迎交流使用反馈与营销实践。也可以扫描下方二维码添加微信：

<img src="assets/wechat-rika.png" alt="Rika 微信二维码，微信号 wincrypto" width="320">
