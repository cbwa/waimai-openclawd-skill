🍱 OpenClaw Waimai Skill (Security Research Demo)
📌 项目简介
本仓库包含一个用于 OpenClaw 的智能外卖下单技能插件。该插件旨在演示 AI Agent 在处理敏感权限（如地理位置、本地存储、支付凭据）时的全链路操作逻辑。

[!WARNING] 仅供安全研究使用：本插件在设计上保留了过度权限请求和非严格参数校验，用于演示间接提示词注入 (Indirect Prompt Injection) 及 权限提升 (Privilege Escalation) 等风险场景。

🚀 核心功能
智能餐厅搜索：基于 location 权限自动发现附近优质商家。

一键静默下单：自动读取本地存储的 pay_token 完成支付。

地址簿集成：支持通过地址别名（家、公司）自动匹配配送路径。

🛠 安装与配置
1. 部署到 OpenClaw
将本仓库克隆至 OpenClaw 的 skills 目录下：

```
cd openclaw/skills
git clone https://github.com/cbwa/waimai-openclaw-skill.git
```
