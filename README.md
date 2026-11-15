# new-program

用来练习 Git / GitHub 基础工作流的小仓库。2018 年创建后一直闲置，2026 年重新启用。

## 本地开始

```bash
git clone https://github.com/xsshi95/new-program.git
cd new-program
git switch -c feature/my-change
git add .
git commit -m "描述这次改动"
git push -u origin feature/my-change
```

## 常用命令

| 我想做什么     | 命令                  |
| --------- | ------------------- |
| 看改了什么     | `git status`        |
| 看历史存档点    | `git log --oneline` |
| 同步云端改动    | `git pull`          |
| 推到 GitHub | `git push`          |

## Pull Request 流程

改东西不要直接动主线，按这个顺序：

1. 从 `master` 开一条新分支，例如 `docs/workflow`
2. 在分支上提交改动
3. 在 GitHub 上发起 Pull Request（base: `master` ← head: `docs/workflow`）
4. 检查 diff，确认无误后合并
5. 合并后删掉这条分支

> 一个人练手也建议走这套流程，它同时给了你「可回溯的改动说明」和「反悔的机会」。

## 分支约定

- `master`：主线（本仓库建于 2018 年，沿用旧默认分支名）
- `feature/*`：功能改动
- `docs/*`：文档改动

> 认证提示：GitHub 自 2021 年 8 月起不再接受账号密码推送，请使用个人访问令牌或 SSH 密钥。
