建repo，写README.md
repo Setting->Pages
Build and deployment:Deploy from a branch
Branch:
    main /root

一会后，会自动生成 website
Your site is live at https://tyc5412.github.io/helm-c/
点击能正常显示readme.md内容，则helm 仓库完成，

helm 添加repo 
#helm repo add [NAME] [URL] [flags]   URL:来自git setting-》pages里的服务地址
helm repo add myrepo  https://tyc5412.github.io/helm-c/