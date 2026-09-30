# Termini

**English** | [中文](#termini-中文)

AI ops workspace for SSH, Telnet, RDP and SFTP.

Connect protocols in one place. The agent runs on real devices; risky actions require approval first; everything is logged; reports can be generated.

## Highlights

- **Approval boundary** — read-only actions pass automatically; similar commands are approved once by prefix; steps that change a system still wait for confirmation
- **Deliverables** — inspection and troubleshooting results as Word, PDF or Excel
- **Host inventory** — hosts, identities and permissions in one place
- **In-session file transfer** — local and remote side by side in the current workspace
- **RDP in the same workspace** — alongside SSH, Telnet and SFTP
- **Session-aware command hints** — suggestions from the current session and device dialect
- **Inspection to routine** — you decide whether new observation points join the routine

## What the AI can do

In Deck chat, the agent uses built-in tools. Risky steps still wait for your confirmation.

### Devices and remote work

- Look up registered devices and groups, and keep a long-lived device profile (role, key paths, known pitfalls) for later chats.
- Run the same non-interactive command on one or many devices over SSH, or over Telnet when SSH is unavailable (typical for some switches and routers).
- Read and edit remote files over SFTP, and upload or download files or directories between this machine and registered devices.

### This machine

- Run commands and multi-line scripts on the host where Termini runs, including interactive TTY sessions when needed; list, read, write into, or stop processes started in the current chat.
- Run approved read-only lookups without a separate approval (directory listings, git history, dependency trees, and similar).
- Run one-shot scripts (JavaScript / TypeScript / Python, or the built-in engine on mobile) to produce richer Word / Excel / PPT / PDF or to transform data.

### Code and local files

- Map a repo’s structure, search by text or regex, find symbols, or ask in natural language where something lives.
- Read and precisely edit local text files in batches.
- Reuse earlier parse or OCR results for the same files or URLs, and page through long tool outputs that were truncated.

### Documents and images

- Read PDF, Word, and Excel; turn scanned or image-heavy PDFs into text with vision when needed.
- Export Markdown to Word or PDF; write Excel sheets for tabular deliverables.
- Transcribe local images with a vision model, or generate images from a text prompt when an image model is configured.

### Desktop UI (this machine)

- Inspect on-screen windows and controls, then click, type, and send shortcuts so the agent can drive desktop apps on this computer (not remote desktops).

### Web

- Search the web for timely information, and fetch the text of public pages when you ask for a specific URL.

### Monitoring and discovery

- Probe a device with SNMP (get / walk / suggest candidate OIDs).
- Draft, create, list, and update formal monitoring indicators on devices so values can be collected on a schedule.

### How the agent organizes work

- Maintain a todo list for multi-step jobs; ask you clarifying questions with choices when only you can decide.
- Spin up background sub-agents for parallel investigation, watch their progress, wait for them, or cancel them.
- Save reusable skills, look them up later, and update them; search for additional tools when needed.
- Start or stop background loops that re-run a tool on an interval and wake the chat on a match.
- Read earlier chat history when context was truncated; send HTML email when you ask for a report or alert mail.
- List and change app data tables when that is part of the task.

## Screenshots

### Android

<table>
<tr>
<td align="center">
<img src="docs/screenshots/android/deck.png" width="280" alt="AI Deck"><br>
AI Deck chat
</td>
<td align="center">
<img src="docs/screenshots/android/sftp.png" width="280" alt="SFTP"><br>
In-session SFTP file browser
</td>
</tr>
<tr>
<td align="center">
<img src="docs/screenshots/android/rdp.png" width="280" alt="RDP"><br>
RDP desktop in the same workspace
</td>
<td align="center">
<img src="docs/screenshots/android/snippets.png" width="280" alt="Snippets"><br>
Reusable command snippets
</td>
</tr>
</table>

### Windows

<table>
<tr>
<td align="center">
<img src="docs/screenshots/windows/hosts.png" width="520" alt="Hosts"><br>
Host inventory dashboard
</td>
<td align="center">
<img src="docs/screenshots/windows/terminal-ssh.png" width="520" alt="SSH terminal"><br>
SSH session terminal
</td>
</tr>
<tr>
<td align="center">
<img src="docs/screenshots/windows/terminal-network.png" width="520" alt="Network CLI"><br>
Network device CLI session
</td>
<td align="center">
<img src="docs/screenshots/windows/rdp.png" width="520" alt="RDP"><br>
Windows RDP tab
</td>
</tr>
<tr>
<td align="center" colspan="2">
<img src="docs/screenshots/windows/ai-deck.png" width="520" alt="AI Deck"><br>
AI troubleshooting on real devices
</td>
</tr>
</table>

## Download / Docs / Pricing / Sign in

All product pages: [https://terminiapp.com/](https://terminiapp.com/)

## Platforms

| Platform | Status |
| --- | --- |
| iOS | Available |
| macOS | Available |
| Windows | Available |
| Linux | Coming soon — packages will be published on this repository's Releases |

## This repository

This repository does **not** include source code. It is for product introduction and feedback only.

- Open an [Issue](https://github.com/chengpengvb/termini-app/issues) for bugs or feature requests
- Pull requests that treat this as an open-source codebase are not accepted

## Privacy / Terms

- [Privacy Policy](https://terminiapp.com/en/privacy)
- [Terms of Service](https://terminiapp.com/en/terms)

---

# Termini（中文）

[English](#termini) | **中文**

面向 SSH、Telnet、RDP、SFTP 的 AI 运维工作区。

在一处连接上述协议；agent 在真实设备上执行；风险操作先批准；有日志；能出报告。

## 要点

- **批准边界** — 只读自动过；相似命令按前缀批一次；改系统仍要确认
- **交付物** — 巡检与排障结果可输出为 Word / PDF / Excel
- **主机清单** — 主机、身份与权限集中管理
- **会话内传文件** — 本地与远端同在当前工作区
- **RDP 同一工作区** — 与 SSH、Telnet、SFTP 并列
- **按当前会话给命令提示** — 结合当前会话与设备命令方言
- **巡检是否纳入例行** — 由你决定

## AI 能做什么

在 Deck 对话里，agent 会调用内置工具完成任务；会改动系统的步骤仍需你确认。

### 设备与远程操作

- 查询已登记的设备与分组，并维护设备档案（角色、关键路径、已知坑），供后续对话复用。
- 通过 SSH 在一台或多台设备上执行同一条非交互命令；仅有 Telnet 的设备（常见于部分交换机、路由器）走 Telnet 批量执行。
- 经 SFTP 读改远端文件，并在本机与已登记设备之间上传或下载文件/目录。

### 本机

- 在 Termini 所在电脑上执行命令与多行脚本，需要时打开交互式终端；可列出、查看输出、向交互终端写入或结束本对话启动的进程。
- 对白名单内的只读查询可免单独批准（列目录、看 git 历史、依赖树等）。
- 跑一次性脚本（JavaScript / TypeScript / Python，移动端可用内置引擎）生成版式更完整的 Word / Excel / PPT / PDF，或做数据处理。

### 代码与本地文件

- 生成仓库结构图、按文本/正则搜索、按符号名定位，或用自然语言做语义检索。
- 批量读取与精确替换本地文本文件。
- 复用同一文件或网址此前的解析/识别结果，并翻阅被截断的长工具输出全文。

### 文档与图片

- 读取 PDF、Word、Excel；扫描件或图片型 PDF 可走视觉识别成文。
- 将 Markdown 导出为 Word 或 PDF；写入 Excel 表格作为交付物。
- 用视觉模型转写本机图片；在已配置图片生成模型时，可按文字描述生成图片。

### 本机桌面界面

- 读取本机窗口与控件结构，再点击、输入、发送快捷键，驱动本机图形应用（不含远程桌面）。

### 网络

- 用搜索引擎查时效信息；在你指定公开网址时抓取页面正文。

### 监控与发现

- 对设备做 SNMP 探测（取值 / 遍历 / 按型号建议候选 OID）。
- 起草、创建、查看与更新正式监控指标，便于按周期采集。

### agent 如何组织工作

- 维护多步任务待办；缺你才能提供的关键信息时，用带选项的问题向你确认。
- 拉起后台子代理并行调查，查看进度、等待结束或取消。
- 保存、查询与更新可复用技能；需要时搜索更多可用工具。
- 启动或停止按间隔重复调用某工具的后台循环，命中条件时唤醒对话。
- 在上下文被截断时回查更早会话内容；按你的要求发送 HTML 邮件简报或告警。
- 在任务需要时列出并读写应用内数据表。

## 截图

### Android

<table>
<tr>
<td align="center">
<img src="docs/screenshots/android/deck.png" width="280" alt="AI Deck"><br>
AI Deck 对话
</td>
<td align="center">
<img src="docs/screenshots/android/sftp.png" width="280" alt="SFTP"><br>
会话内 SFTP 文件浏览
</td>
</tr>
<tr>
<td align="center">
<img src="docs/screenshots/android/rdp.png" width="280" alt="RDP"><br>
同一工作区内的 RDP
</td>
<td align="center">
<img src="docs/screenshots/android/snippets.png" width="280" alt="Snippets"><br>
命令片段
</td>
</tr>
</table>

### Windows

<table>
<tr>
<td align="center">
<img src="docs/screenshots/windows/hosts.png" width="520" alt="主机清单"><br>
主机清单
</td>
<td align="center">
<img src="docs/screenshots/windows/terminal-ssh.png" width="520" alt="SSH 终端"><br>
SSH 会话终端
</td>
</tr>
<tr>
<td align="center">
<img src="docs/screenshots/windows/terminal-network.png" width="520" alt="网络设备 CLI"><br>
网络设备 CLI 会话
</td>
<td align="center">
<img src="docs/screenshots/windows/rdp.png" width="520" alt="RDP"><br>
Windows RDP 标签页
</td>
</tr>
<tr>
<td align="center" colspan="2">
<img src="docs/screenshots/windows/ai-deck.png" width="520" alt="AI Deck"><br>
在真实设备上做 AI 排障
</td>
</tr>
</table>

## 下载 / 文档 / 定价 / 登录

产品站统一入口：[https://terminiapp.com/](https://terminiapp.com/)

## 平台

| 平台 | 状态 |
| --- | --- |
| iOS | 已上架 |
| macOS | 已上架 |
| Windows | 已上架 |
| Linux | 即将提供 — 安装包将发布在本库 Releases |

## 关于本库

本库**不包含源代码**，仅用于产品介绍与反馈。

- 请通过 [Issue](https://github.com/chengpengvb/termini-app/issues) 提交 Bug 或功能建议
- 不接受按开源项目提交的 PR

## 隐私 / 条款

- [Privacy Policy](https://terminiapp.com/en/privacy)
- [Terms of Service](https://terminiapp.com/en/terms)
