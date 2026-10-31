# Modules

本 package 統一放置本 mono repository 的 Git submodules。各 module 保留自己的 repository、版本與工作要求；文件及實作之間的分工依 [FORMULATION](../FORMULATION.md)。

| Submodule | 用途 |
|---|---|
| [ai-native-founders-tw-web](ai-native-founders-tw-web/README.md) | 組織網站的實作、測試與建置 |

在 mono 根目錄執行 `git submodule update --init --recursive` 可依記錄的版本初始化 submodules。修改與提交的要求依 [AGENTS](../AGENTS.md)。

從網站目錄使用本機 mono 資料時，執行 `MONO_PATH=../.. pnpm build`。獨立 clone 網站 repository 時，`MONO_PATH` 應指定實際 mono 路徑。
