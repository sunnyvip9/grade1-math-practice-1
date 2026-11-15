# Roadmap

## 当前阶段

２０２６年１１月１５日：已在主人指定的实际仓库接入 GoatCounter，首页及四课共５个 HTML 各加载一次官方异步脚本，端点为 `https://sunnyvip9.goatcounter.com/count`，关闭作答点击事件采集。README 已补充统计后台和同步步骤。当前本地实现与验证完成，等待主人同步 GitHub 和部署后核实入账。

## 已完成

- 保存本仓库原５页、README 和１１６个原交付文件的实际哈希，核对１１０个未改文件，其中１０９个程序／样式／声音运行资源及１０１段配音全部不变。
- ５页接入 `https://sunnyvip9.goatcounter.com/count`，去掉新增脚本后与本仓库修改前原文完全一致。
- 针对实际仓库文件完成统计正常、脚本被拦截、接口失败及本地默认四种模式的５页路径、四课首题计分、原生声音、暂停／重开和手机排版检查。
- HTTP 预览的 README 包含本仓库真实路径，确认验证服务未误指向旧交付副本；Git 差异可见５个 HTML 和 README 已修改，新增项目规范和本进度文件。

## 待办

- 主人将改动同步到 GitHub，等待 Pages 更新。
- 部署后登录 GoatCounter 核实真实访问入账；本地模拟不能替代这项检查。

## 最近验证

四种浏览器模式及最终差异检查通过。测试统计请求全部拦截，正式计数未被测试污染；后台登录页可达。证据保存在 `E:/Projects/Ming_Video_Factory/outputs/math-practice-analytics-repo-checks/`。未提交、未推送，线上真实入账尚未验证。
