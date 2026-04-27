# AI-Native 产品观察台

只收录「如果把 AI 拿掉，产品就不存在」的那一类产品，按交互范式与 AI 能力双视图呈现。
每 3 天由 WorkBuddy automation 自动搜罗与增量更新，每轮新增上限 3 款。

在线访问：<https://seyazhu.github.io/ai-native-products/>

## 字段约定

每个产品条目必须包含：

- `name` / `url`（官网，非聚合文章）/ `tagline`
- `cat` / `cats`：交互范式分类（agent / coding / search / creative / design / productivity / meeting / vertical / cn）
- `capability`：AI 能力维度，三选一
  - `gen` 生成型：用户给提示，AI 产出成品
  - `agent` Agent 型：AI 有动作权，替你跑长任务
  - `embed` 嵌入型：AI 藏在既有工作流里
- `why`：解决了什么（1-2 句）
- `design`：为什么这么设计（1-2 句具体设计手法）
- `status`：`stable` / `new`（本轮新增）/ `updated`（本轮有更新）

## 本地预览

```bash
cd ai-native-products
python3 -m http.server 8765
# 访问 http://localhost:8765
```

## 自动更新

WorkBuddy automation id 为 `ai-native-3`，每 72 小时触发一次：
检索 → 增量更新 `products` 数组 / `META.version` / `changelog` → git commit & push → GitHub Pages 自动刷新。
