# homepage
my homepage about intro &amp; experience &amp; life &amp; book

## 工程结构
```
homepage
├─.github           # github配置
│  └─workflows      # 自动构建部署配置
├─components        # vue组件
├─docs              # 博客内容
│   ├─.vitepress    
│   │  ├─config.mts  # vitepress配置
│   │  ├─cache      # 缓存文件，可忽略提交
│   │  ├─dist       # 构建包
│   ├─index.md      # 博客首页
│   ├─2023          # 按照年份存放博文
│   └─public        # 博客使用的静态资源
├─.gitignore        # git提交忽略配置
├─deploy.sh         # 手动部署脚本
├─package.json      # node.js配置
├─pnpm-lock.yaml    # 依赖的锁定版本号
└─README.md         # 工程说明
```

## 工程开发
```
# 安装依赖
pnpm install
# 开发模式启动
pnpm dev
# 手动构建
pnpm build
# 生产模式启动构建成果
pnpm serve
# 预览构建成果
pnpm preview
# 上传构建成果到gh-pages分支（目前已不用该模式部署）
pnpm deploy
```

## 自动构建部署
push到GitHub仓库main分支，GitHub Actions 会自动触发，在GtHub服务器上自动构建并部署。

