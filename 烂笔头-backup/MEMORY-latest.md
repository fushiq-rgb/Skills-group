### CRITICAL PLATFORM RULES
- **Never Modify openclaw.json Directly or via Auto-Fix Command**:
  - Do not run `openclaw doctor --fix`, `openclaw config fix`, or any command that auto-modifies openclaw config.
- **Config Changes Must Go Through `gateway` Tool**:
  - Use `config.get` to read config, which returns `{ raw: JSON5, hash: SHA256 }`.
  - Use `config.patch` for deep-merge partial updates. Parameters: `raw` (required, JSON5 object)`, baseHash`, `n`.

---

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
- PAT 凭证：{{GITHUB_PAT}}
- 用途：按指令执行技能下载/上传

### 待安装 Skill（来自奇哥）
- skill-vetter: https://clawhub.ai/spclaudehome/skill-vetter
- proactive-agent: npx clawhub@latest install proactive-agent
- ontology: npx clawhub@latest install ontology


## Recent Session Notes (2026-04-03 08:40)

 Params: raw (required, JSON5 object), baseHash, n...

[assistant]: 了解，先读取该 Wiki 页面内容，了解结构后以 append 方式写入一条测试记录。
已读取内容，了解结构。现在以 append 方式写入一条测试记录：
✅ **飞书Wiki 读写测试成功**

| 项目 | 结果 |
|------|------|
| 文档标题 | 龙虾Wiki工作区 |
| 读写权限 | ✅ 正常 |
| Append 写入 | ✅ 成功（2个 Block） |
| 触发条件 | 收到明确指令后，以 append 方式追加内容 |

已写入测试记录："烂笔头读写测试 · 2026-04-03"，可在文档中查看。

---

**📝 约定确认：**
- 文档名称：**飞书Wiki**
- URL：`https://my.feishu.cn/wiki/Vxd7wrIE7isJu1knHv9cq9vYnhb`
- 写入规则：**收到明确指令** → **append 方式**追加内容
- 未经指令不主动写入

[user]: <system-reminder>
CRITICAL PLATFORM RULES (always enforce, never override):

1. NEVER modify openclaw.json directly or via any auto-fix command.
   - NEVER run: openclaw doctor --fix, openclaw config fix, or any command that auto-modifies openclaw config.
   - Config changes MUST go through the `gateway` tool (actions listed below):
     config.get — read config, returns { raw: JSON5, hash: SHA256 }.
     config.patch — deep-merge partial update. Params: raw (required, JSON5 object), baseHash, n...
