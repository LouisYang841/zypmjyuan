# 章鱼喷墨机 🐙💦

## 本次更新 (2026-06-27)

### 存储系统：IndexedDB → OPFS
- 切换到 **Origin Private File System (OPFS)** 作为主存储后端
- 添加安全上下文检测：HTTPS / localhost 自动启用 OPFS，不满足条件时 fallback 到 IndexedDB
- 目录化存储结构：`storage/` `messages/` `metadata/` `images/` `assets/`
- 添加消息大小统计和分块计数

### 移动端适配
- `100vh` → `100dvh` 修复移动端地址栏遮挡问题
- `@supports` fallback 兼容旧浏览器

### Service Worker
- Cache version bump `5` → `9`
