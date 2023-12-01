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

## 说明
- 阶段1<br>
  本地完成代码编写后，执行`npm run deploy`命令，执行deploy.sh脚本，完成半自动build和push代码至gh-pages分支；gh-pages分支为打包构建好的前端资源。
- 阶段2<br>
  在本地执行build之后，执行git commit，然后推送到远程仓库，推送到远程仓库会触发Github Action自动执行重新部署站点
[HOMEPAGE](https://tonyzhang1993.github.io/homepage/)

