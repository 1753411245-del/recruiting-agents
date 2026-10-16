# 招聘智能体系列（Recruiting Agents）

一套 **纯前端、零依赖、零网络请求** 的招聘智能体工具。每个工具都是单个 HTML 文件，浏览器打开即用，无需安装任何环境；全部数据仅保存在本机浏览器的 `localStorage` 中，不上传任何服务器。

## ✨ 特性

- **单文件 · 免安装**：每个智能体一个 HTML，双击即用，也可部署到任意静态托管
- **本地存储**：数据不出本机，清浏览器数据即重置
- **合规红线内建**：歧视性标签自动检测、候选人隐私不出本机、AI 输出须人工复核留痕
- **可演练**：内置示例数据一键载入，快速体验全流程

## 📦 包含工具

| # | 工具 | 文件 | 说明 |
|---|------|------|------|
| 01 | JD 生成智能体 | [agents/jd-generator.html](agents/jd-generator.html) | 输出对外版 + 内部版双 JD，内置合规风险检测与人才画像打分表 |
| 02 | 简历筛选智能体 | [agents/resume-screener.html](agents/resume-screener.html) | 硬门槛→一票否决→加分加权三层过滤，A/B/C 分级 + 风险预审（空档期/跳槽/薪资矛盾）+ 面试邀约方案 + 台账归档 |
| 03 | 人才寻访智能体 | [agents/talent-sourcing.html](agents/talent-sourcing.html) | 目标公司清单、人才地图、寻访话术与渠道盘点 |
| 04 | 结构化面试评估报告 | [agents/interview-eval.html](agents/interview-eval.html) | 维度评分、STAR 追问记录、录用建议自动汇总 |
| 05 | AI 面试题生成 | [agents/interview-questions.html](agents/interview-questions.html) | 按岗位/层级/考察维度生成结构化面试题与追问链 |
| 06 | 招聘流程自动化看板 | [agents/recruiting-automation.html](agents/recruiting-automation.html) | 招聘漏斗、关键指标、阶段流转数据看板 |
| 07 | 业务解码画布 | [agents/business-canvas.html](agents/business-canvas.html) | 四层业务解码 + 九格画布 + 招聘漏斗瓶颈分析 + 行动清单 |

## 🚀 快速开始

**在线版**：开启 GitHub Pages 后直接访问仓库首页（Settings → Pages）。

**离线版**：下载本仓库，双击任意 `agents/*.html` 即可使用。

> 提示：部分浏览器对 `file://` 协议下的 localStorage 有限制，推荐通过 GitHub Pages 在线使用，或本地起一个静态服务（如 `python -m http.server`）。

## 🔒 隐私与合规

- 全部工具本地运行，无第三方接口、无统计埋点、无网络请求
- 内置歧视性标签检测（性别/年龄/婚育/地域等），在配置筛选标准时实时警示
- 候选人简历与评估数据仅存本机，不向第三方传输
- AI 能力为预留接口（默认关闭）；如自行接入云端模型，请自行评估数据合规
- 本工具仅辅助 HR 决策，**不替代人工判断，不用于歧视性筛选**

## 📁 目录结构

```
recruiting-agents/
├── index.html                  # 门户页（GitHub Pages 首页）
├── agents/
│   ├── jd-generator.html
│   ├── resume-screener.html
│   ├── talent-sourcing.html
│   ├── interview-eval.html
│   ├── interview-questions.html
│   ├── recruiting-automation.html
│   └── business-canvas.html
├── README.md
└── LICENSE
```

## 🤝 贡献

欢迎提 Issue 与 PR。新增智能体请保持「单 HTML 文件、无外部依赖、localStorage 存储」的约定。

## 📄 License

[MIT](LICENSE)
