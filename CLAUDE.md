# 一年级数学练习网站 · 项目规范

## 源码与范围

当前实际 Git 仓库为 `E:/Github/grade1-math-practice-1`，这是后续网站修改和用户同步 GitHub 的源目录。`E:/Projects/Ming_Video_Factory/outputs/math-practice-github-pages/` 是之前的视频工程交付副本，修改该副本不会自动同步本仓库。

根目录 `index.html` 为四课首页；`queue/`、`date/`、`reading/`、`stairs/` 分别为排队、推迟、读书、爬楼，每课包含 HTML、已构建 JS／CSS 和配音。四期教学内容、声音与交互均已验收。保持相对路径，不增加构建依赖，精准修改请求相关文件。

## 访问统计

主人已授权接入 GoatCounter，站点 `sunnyvip9.goatcounter.com`，统计端点 `https://sunnyvip9.goatcounter.com/count`。首页及四课５页各加一段官方异步脚本，`no_events:true`，只统计访问，不采集作答点击、答案、分数，不在儿童页面展示计数器。不修改课程程序、样式、声音或计分规则。README 记录统计后台和部署步骤。

修改前原页和哈希、浏览器及服务验证保存在视频工程独立的 `outputs/math-practice-analytics-repo-checks/`，不放入本仓库运行目录。验证必须针对本仓库真实文件，覆盖统计正常、脚本被拦截、接口失败及本地不计数，保留原始证据。模拟统计请求必须拦截，不向正式后台写入测试访问。

## 交付

完成后更新 `ROADMAP.md`，核对 Git 差异和未改资源哈希。授权仅本地修改；提交、推送及发布由主人决定，不自动执行。原始校验中的待发布状态不能改写为线上入账已验证。
