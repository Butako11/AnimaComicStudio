# 下载与更新

请打开本 GitHub 项目的 **Releases（发行版）**，选择目标版本。当前文档对应 **v1.2.6**。

| 你需要什么 | 文件 |
| --- | --- |
| 第一次使用，完整环境与模型 | `AnimaComicStudio-v1.2.6-Windows-Offline.zip`（约 9.9 GB） |
| 已有旧版，只更新程序 | `AnimaComicStudio-v1.2.6-增量更新-透明差分与退出修复.zip`（约 92 MB） |

完整包可能通过发布页中的外部网盘链接提供，或拆成多个分卷。分卷形式需要下载全部分卷到同一文件夹，再从第一个分卷解压；具体以发布页说明为准。

GitHub 自动提供的 **Source code (zip)** 是仓库文件快照，不等于包含运行时和模型的完整软件包。

## 新用户

完整解压到磁盘空间充足的目录，运行 `启动软件.cmd`。请勿直接从压缩包中启动程序。填写自己的 API Key 后，先测试每章 10 张、1 章。

## 已有用户

1. 在旧版网页中点击保存退出，等待引擎停止。
2. 将更新包解压到原软件根目录，即同时含 `启动软件.cmd`、`runtime`、`engine` 的那一层。
3. 覆盖同名程序文件后重新启动。
4. 保留 `user_data`、`projects`、模型与输出目录；不要删除原软件再安装。

## 下载校验

下载页应同时提供对应的 `.sha256.txt` 文件。Windows PowerShell 可检查：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\AnimaComicStudio-v1.2.6-Windows-Offline.zip'
```

与发布者给出的 SHA256 相同，说明下载文件与发布文件一致。若提示校验和错误或解压损坏，先重新下载出错文件；不要把尚未下载完整的压缩包当作可用软件。
