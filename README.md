# Portfolio Site Workflow

把零散的项目资料，做成一个清楚、有个人特点、能持续更新的作品集网站。

这是一套给 AI 编程助手使用的 **Skill**，也可以当作人工制作网站的步骤指南。它整理自 KelanG 个人网站从初稿到多页面、双语、3D 互动与独立 HTML 分享版的迭代经验。它不是网站源码，也不是点一下就自动上线的托管服务。

## 能帮你做什么

- 把 PPT、图片、项目介绍和聊天记录整理成可信的个人与项目文案。
- 规划首页、项目列表、项目详情、关于和联系方式；根据内容规模调整结构。
- 选择适合个人特点的视觉方向，避免每个项目都长成同一个模板。
- 按需实现轻量转场、图片倾斜、3D 头像或模型互动。
- 检查手机布局、触屏、中英文、返回按钮、图片查看和最终分享文件。
- 说明以后怎么加项目、怎么更新、如何确认已经公开发布。

不要求所有网站采用黑白配色、3D、双语或多个页面。先满足真实的内容和使用场景。

## 安装与使用

需要一个支持文件夹 Skill 的编程助手，以及它执行具体任务所需的本地文件/浏览器工具。这个仓库本身没有必须安装的 npm 或 Python 依赖；构建网站时再按所选方案安装所需工具。

Codex 的用户级 Skill 目录可使用 `~/.agents/skills/`。在该目录下克隆本仓库：

```sh
git clone https://github.com/KelanG798/portfolio-site-workflow.git ~/.agents/skills/portfolio-site-workflow
```

Windows PowerShell：

```powershell
git clone https://github.com/KelanG798/portfolio-site-workflow.git "$env:USERPROFILE/.agents/skills/portfolio-site-workflow"
```

也可以下载 ZIP，解压后把包含 `SKILL.md` 的 `portfolio-site-workflow` 文件夹放入上述目录；避免出现重复嵌套目录。若 Skill 未出现，重新打开助手会话检查发现情况。其他助手的目录和调用方式请以其文档为准。

然后给助手发：

```text
使用 $portfolio-site-workflow 帮我制作个人作品集。
目标：让面试官看懂我做过什么。
已有资料：一份项目 PPT、两张产品图、一段个人介绍。
希望：手机和电脑都能看，后续容易添加项目。
先整理内容和页面结构，再把第一版做出来。
```

更新已有网站：

```text
使用 $portfolio-site-workflow 更新我的现有网站。
请先读取现有文件，保留我已经确认的风格。
根据新项目图片和说明新增一个独立项目页面，更新列表，
并验证手机布局和我最终分享出去的版本。
```

## 从哪里开始读

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](SKILL.md) | 助手入口与核心决策 |
| [完整流程](references/workflow.md) | 从定位、设计到交付的全流程 |
| [内容与页面](references/content-and-routes.md) | 文案提炼、项目结构、持续新增 |
| [视觉、动态与 3D](references/visuals-and-interaction.md) | 如何做出个人特点并控制交互质量 |
| [检查与发布](references/qa-and-release.md) | 手机、离线文件、公网发布的验收区别 |
| [KelanG 案例复盘](references/kelang-case.md) | 这套方法来自哪些真实迭代 |
| [需求记录](templates/site-brief.json) | 可选的机器可读输入 |
| [交接记录](templates/handoff.md) | 交付时留下可维护说明 |

最小输入是“你是谁、网站给谁看、一个项目做了什么”。不必为了填表编造结果，也不用一开始就做 3D。

## 一次完整任务应交付什么

1. 确认过的内容与页面结构。
2. 能浏览、能跳转的页面与可编辑源码。
3. 用户要求的分享文件或部署结果。
4. 实际检查记录、未验证项和新增项目的方法。

本仓库只公开流程、提示词和通用记录模板，不包含个人网站源文件、私人资料、头像模型或原始 PPT。MIT 许可覆盖本仓库中的方法文档与模板；不授予第三方素材的使用权。

## 依据与版本

- Codex Skills 官方说明：https://developers.openai.com/codex/skills/
- GitHub 仓库创建：https://cli.github.com/manual/gh_repo_create
- 无障碍与动效参考：https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion

整理日期：2026-10-24。欢迎通过 Issues 或 Pull Requests 提出可复现的问题、改进流程或补充案例。
