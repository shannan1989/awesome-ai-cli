# AI

## iFlow CLI

官网：https://platform.iflow.cn/

https://platform.iflow.cn/mcp

https://platform.iflow.cn/agents

MCP Server Directory: https://www.pulsemcp.com/servers

官方宣传文章：

https://mp.weixin.qq.com/s/uq70MDj2BWJGtEGcrkuj-w


## 常用 MCP 工具

### 12306 火车票查询
```sh
iflow mcp add-json '12306-mcp' "{\"command\":\"npx\",\"args\":[\"-y\",\"@iflow-mcp/12306-mcp@0.3.4\"]}"
```
### UNO-MCP五合叙事算子
文本增强工具，将普通故事内容转换为丰富详细的叙述，支持多种增强技术
```sh
iflow mcp add-json 'uno-mcp-fixed' "{\"command\":\"npx\",\"args\":[\"-y\",\"@iflow-mcp/uno-mcp-fixed\"]}"
```
### 哔哩哔哩
提供视频搜索、用户查询、精确匹配和弹幕获取功能。
```sh
iflow mcp add-json 'bilibili-mcp-server' "{\"command\":\"uvx\",\"args\":[\"--from\",\"iflow-mcp-bilibili-mcp-server\",\"bilibili\"]}"
```
### 小红书搜索评论工具
小红书平台的搜索、内容获取和评论发布工具，支持笔记搜索、内容分析和智能评论
```sh
iflow mcp add-json 'redbook-search-comment-mcp' "{\"command\":\"uvx\",\"args\":[\"--from\",\"iflow-mcp_redbook-search-comment-mcp\",\"redbook-search-comment-mcp\"]}"
```
## 常用 Agent 智能体

### 代码审查专家
专业的代码审查专家。主动审查代码的质量、安全性和可维护性。在编写或修改代码后立即使用。
```sh
iflow agent add "code-reviewer" --scope global
```
### 调试专家
专注于错误、测试失败和意外行为的调试专家。遇到任何问题时主动使用。
```sh
iflow agent add "debugger" --scope global
```
## 常用指令

### 清理项目
清理开发工件，同时保留您的工作代码
```sh
iflow commands add "cleanproject" --scope global
```
### 提交代码
分析您的更改并创建有意义的提交信息
```sh
iflow commands add "commit" --scope global
```
### 实现功能
智能地从任何来源实现功能-完美地适应您项目的架构
```sh
iflow commands add "implement" --scope global
```
### 重构代码
系统地重新构建您的代码-在保持功能的同时改善结构、可读性和可维护性
```sh
iflow commands add "refactor" --scope global
```
### 代码审查
多智能体分析（安全性、性能、质量、架构）
```sh
iflow commands add "review" --scope global
```
