# dsh-workbuddy-connect — 第三方镜像备份（非官方）

本仓库是 **DSH（DeepSeek Harness）插件 `dsh-workbuddy-connect`** 的源码快照镜像，由 ZiLe1433 于 2026-10-22 备份，目的是在原作者停止维护时保留可用的源码副本。

## 来源与版本

| 项目 | 值 |
| --- | --- |
| 插件名 | `dsh-workbuddy-connect` |
| 版本 | 0.7.6 |
| 原仓库 | https://github.com/corrinehu/dsh-workbuddy-connect |
| 作者 | corrinehu |
| 备份时间 | 2026-10-22 |
| 备份位置 | `%DSH_HOME%/profiles/desktop/node_modules/dsh-workbuddy-connect` |

## 说明

该插件把 WorkBuddy 桌面 App 里已登录的模型接入 DeepSeek Harness（复用 WorkBuddy 的登录态，不额外发起 OAuth）。

- `lib/index.js` — 宿主侧插件（provider 注册、模型目录、设置）
- `lib/client.js` — Web 客户端 bundle（模型选择 UI）
- `lib/bin.js` — CLI 入口
- `lib/host-heartbeat-*.js` — 宿主心跳与状态同步
- `cordis.patch.yml` — DSH 插件 bundle 的加载补丁
- `README.md` / `README.en.md` — 中英文使用说明

本快照为 npm 发布包 `dsh-workbuddy-connect@0.7.6` 的完整内容（含 `lib`、README、LICENSE、patch）。原仓库未包含 TS 源码的构建产物差异，`lib/*.d.ts` 已保留类型声明。

## 许可

上游采用 MIT License（见 `LICENSE`，Copyright (c) 2026 Corrine Hu）。本镜像原样保留许可与版权声明，未作修改。

## 免责

- 本仓库为**非官方镜像**，与原作者无关，不代表原作者立场。
- 内容按“原样”提供，不承诺兼容未来版本的 DSH / WorkBuddy。
- 如果原作者恢复维护或提出异议，请优先使用原仓库，并可在 Issues 中告知以便下线本镜像。
