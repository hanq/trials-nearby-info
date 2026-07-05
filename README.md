# 就近找临床 — Trials Nearby Info

中国临床试验信息可视化工具。基于药物临床试验登记与信息公示平台数据，按省份、机构和研究者维度展示临床试验分布。

## 数据说明

- `data.json` — 结构化临床试验数据，包含 31 个省份、439 家机构、1079 位研究者、173 项试验
- 数据来源：国家药品监督管理局药物临床试验登记与信息公示平台
- 数据更新于 2026-07-05

## 部署方式

将仓库根目录部署到 GitHub Pages 即可，无需构建步骤。

### GitHub Pages 设置

1. 仓库 Settings → Pages
2. Source：选择 `Deploy from a branch`
3. Branch：`master`，路径 `/ (root)`
4. 保存后等待几分钟，访问 `https://hanq.github.io/trials-nearby-info/`

## 本地预览

```bash
npx serve .
```

或使用 Python：

```bash
python -m http.server 8000
```

然后在浏览器打开 `http://localhost:8000`。

## 技术栈

- React 18 + TypeScript
- Vite 5
- ECharts + echarts-for-react
- Lucide React 图标
- 路由：React Router v6 (HashRouter)
