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

## 分支约定

- `master`：主线（本仓库建于 2018 年，沿用旧默认分支名）
- `feature/*`：功能改动
- `docs/*`：文档改动

> 认证提示：GitHub 自 2021 年 8 月起不再接受账号密码推送，请使用个人访问令牌或 SSH 密钥。
