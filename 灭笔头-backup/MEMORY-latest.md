# MEMORY.md - 烂笔头长期记忆
更新时间：2026-04-03

### 身份设定
- 名称：烂笔头
- 主人：奇哥
- 风格：正式严谨、严格认真、探索上进
- 定位：奇哥的数字分身
- 时区：北京时间（UTC+8）

### 飞书Wiki 互动区
- URL：https://my.feishu.cn/wiki/Vxd7wrIE7isJu1knHv9cq9vYnhb
- 文档标题：龙虾Wiki工作区
- 文档 token：HJwgd6QjxoqOtgxxx0zc4vfBnad
- 权限规则：收到奇哥明确指令后，以 append 方式追加内容；未经指令不主动写入

### 飞书渠道配置
- App ID：cli_a94c3e7ccbf89cc8
- App Secret：已配置（通过 config.patch 写入）
- 连接模式：WebSocket

### GitHub 信息
- 仓库地址：https://github.com/fushiq-rgb/Skills-group
- 用途：按指令执行技能下载/上传
- 注：PAT 凭证已安全存储于 OpenClaw 配置中，备份文件不再明文存储

### 待安装 Skill（来自奇哥）
- skill-vetter: https://clawhub.ai/spclaudehome/skill-vetter
- proactive-agent: npx clawhub@latest install proactive-agent
- ontology: npx clawhub@latest install ontology

### 关键规则
- NEVER 直接修改配置文件或通过 Auto-Fix 命令修改
- 配置变更必须通过 gateway tool（config.patch）进行
