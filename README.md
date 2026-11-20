# 健康乡镇数字画像（BI 图表）

单页 HTML 可视化模块：极坐标玫瑰图 + 最大值/平均值/最小值三线对比 + 地区排名 + 指标明细 + 数据维护 + 配色配置。

## 目录结构

```
bi-chart/
├── index.html                       # 预览入口页（开箱即可看）
├── 健康城镇数字画像/
│   └── 健康乡镇数字画像.html         # 数据模块本体（交付/修改目标）
└── .gitignore                       # 忽略 Excel 数据表
```

## 预览方式

| 方式 | 操作 | 说明 |
| --- | --- | --- |
| 在线预览 | https://eyeglasscat.github.io/bi-chart/ | GitHub Pages 已开通（main 分支根目录），国内可直连 |
| 本地入口页 | 双击 `index.html` | 内嵌 iframe 直接渲染，附带「全屏打开 / 下载 HTML / 刷新预览」 |
| 直接打开模块 | 双击 `健康城镇数字画像/健康乡镇数字画像.html` | 单文件自包含，无需服务器 |
| Gitee | 仅作代码托管 | Gitee Pages 已于 2024 年下线，raw 直链返回 text/plain，无法在线渲染 |

> 在线预览与本地页面是两套浏览器存储，在线版默认是内置示例数据；要显示真实数据，请在页面内导入 Excel 或进入「数据维护」录入。

## 数据与配置

- 数据存于本机 `localStorage['healthTownPortrait/v2/health-town-portrait']`，配色存于 `localStorage['healthTownPortrait/v2/palette']`；首次打开为内置示例数据。
- 支持导入/导出 Excel、写回原文件、恢复内置数据。
- Excel 数据表不入库，仓库只跟踪 HTML 产物。

## 提交约定

```bash
git add -A && git commit -m "..." && git push origin main
git push origin main:master   # 同步默认分支
```
