# 代码变更记录

---

- 变更的日期：2026-02-23 21:42
- 变更的文件：.github/workflows/lint.yml
- 变更的位置：code_coverage job
- 变更的内容：
```yaml
    permissions:
      contents: read
      pull-requests: write
```
- 变更的原因：修复 GitHub Actions Code Coverage Report 任务权限不足的问题。该任务需要向 PR 添加覆盖率报告评论，但默认权限不允许。添加 `pull-requests: write` 权限使 Action 能够成功发布评论。

---
