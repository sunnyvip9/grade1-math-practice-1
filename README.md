# 四课网站 · GitHub Pages 上传说明

本包为已验收的四课练习网站：排队、推迟、读书、爬楼，每课１０题、满分１００分。题目、配音、计分与解析流程保持已验收版本。无需安装 Node 或运行构建命令。

## 文件放在哪里

先解压 ZIP，打开解压后的目录。将里面的文件及四个课程文件夹上传到 GitHub 仓库根目录，保持以下结构：

```text
index.html
.nojekyll
README.md
queue/
  index.html
  app.js
  app.css
  audio/
date/
reading/
stairs/
```

`date/`、`reading/`、`stairs/` 与 `queue/` 的结构相同。不要只上传 ZIP，也不要把整个外层 `math-practice-github-pages` 文件夹再套进仓库。上传完后，仓库根目录应直接看到 `index.html` 和四个课程文件夹。

## 建议分五批上传

GitHub 网页每次最多上传１００个文件，每个文件最多２５ MiB。本包超过１００个文件，各个文件均小于１ MiB，建议在仓库根目录依次操作 `Add file → Upload files`：

1. 上传根目录的 `index.html`、`.nojekyll`、`README.md`。
2. 将整个 `queue` 文件夹拖入上传区，保留内部 `audio/` 目录，提交保存。
3. 同样上传整个 `date` 文件夹。
4. 同样上传整个 `reading` 文件夹。
5. 同样上传整个 `stairs` 文件夹。

每次均从仓库根目录发起上传。不要进入 `queue/` 后又拖入整个 `queue` 文件夹，以免形成重复嵌套。五批全部上传完成后再启用 Pages。[GitHub 上传文件官方说明](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) 。

## 手动开启 GitHub Pages

在仓库中打开 `Settings → Pages`，在 `Build and deployment` 中，将 `Source` 设为 `Deploy from a branch`，分支选择实际上传文件的分支，通常为 `main`，文件夹选择 `/(root)`，保存。使用 GitHub Free 时，本方案选择公开仓库。

`.nojekyll` 已随包提供，表示直接发布准备好的静态文件。无需自行添加构建流程或安装依赖。[发布源设置官方说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) ，[静态网站说明](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) 。

发布完成后，以 Pages 页面显示的实际网站链接为准。项目网站通常类似 `https://USERNAME.github.io/REPOSITORY/`，这是格式示例，尚未设置正式网址。

## 四个课程直达入口

| 课程 | 相对于网站首页的地址 |
| --- | --- |
| 排队问题 | `queue/` |
| 推迟问题 | `date/` |
| 读书问题 | `reading/` |
| 爬楼问题 | `stairs/` |

每课都有「返回主题首页」。首次播放声音需要点击「开始」或「重听」；每次练习的分数仅保留在当前页面，刷新或离开后重新开始。

## 发布后检查

打开首页，分别进入四课并返回；在手机上各答一题，确认声音、对错反馈、分数及解析正常。如果没有声音，先检查课程 `audio/` 文件夹是否完整上传。页面打不开时，检查 `index.html` 是否位于发布分支根目录，目录名大小写及文件夹层级是否保持原样。

本次仅交付本地上传包，没有自动上传或发布。正式网址确认后，再生成首页二维码和四课直达二维码。
