# 虫子游戈：旧博客域名的兼容发布

本站已统一迁移到 Hugo。日常写作和网站源码只维护在 [czyouge/czyouge.github.io](https://github.com/czyouge/czyouge.github.io)。

- 主站：[www.czyouge.xyz](https://www.czyouge.xyz/)
- 本仓库继续托管 [blog.czyouge.xyz](https://blog.czyouge.xyz/)，保留旧文章的 `.html` 地址。
- `.github/workflows/hugo-mirror.yml` 从主仓库读取同一份源码并发布，默认每小时同步；也可在 Actions 中手动运行。
- 本仓库原有 `backup/`、`docs/`、Gmeek 配置仅保留作迁移存档，不再编辑或用于发布。原 Issues 和提交历史保留。
- 写作和预览操作见主仓库的 [README](https://github.com/czyouge/czyouge.github.io#readme)。

GitHub 可能暂停长期无仓库活动的定时任务；若发现同步停止，请在 Actions 中重新启用并运行镜像工作流。
