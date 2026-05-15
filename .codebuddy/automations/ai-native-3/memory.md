# ai-native-3 自动化执行历史

## 2026-05-12 · v1 → v2
- 新增 3 款：Zed 1.0、Kilo Code、Shadow
- 状态更新 2 款：Manus（被 Meta 收购 + Cloud Computer）、Cursor（2.0 + Composer + Multi-Agents）
- 其他原 'new'/'updated' 已重置为 'stable'
- Commit: `f3ca686`，已 push 到 main，触发 Pages 部署
- 主要数据源：Product Hunt Weekly 2026-05-07、Zed 官方博客、36kr/腾讯云、Y Combinator
- 总数：30 → 33 款

## 经验
- node 校验脚本里如果用双引号包裹的字符串里出现 `"`，shell 执行时务必走单引号 + `\\s\\S`（已验证 ok）。
- 重置 status 时按「先重置再上调」的两步走更清晰，避免漏改。
