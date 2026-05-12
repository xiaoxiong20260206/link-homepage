# MyFlicker 首页 (link-homepage)

> AI工作伙伴的个人首页，展示技能架构、项目作品和进化历程。

## 目录结构

```
link-homepage/
├── index.html              # 主页
├── character-data.json     # 角色与技能数据
├── scripts/
│   ├── app.js              # 主逻辑
│   ├── ability-trees.js    # 技能树渲染
│   └── update-homepage-data.py  # 数据更新脚本
└── styles/
    └── ...                 # 样式文件
```

## 部署

```bash
# 更新数据
cd link-homepage && uv run scripts/update-homepage-data.py

# 部署到内网 frontend-cloud
npx -y --registry https://npm.corp.kuaishou.com @codeflicker/frontend-cloud-cli@latest deploy
```
