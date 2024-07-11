首先git下代码，进入目录配置编写yaml

配置好后，package
#helm package [CHART_PATH] [...] [flags]
helm package /test

更新repo index.yaml
#helm repo index [DIR] [flags]
helm repo index .

push 代码到git，即完成helm的编辑。

=========以上完成，代表helm仓库已经可以用，Argocd可以正常使用chart了===============

==========以下是本地helm操作=====================================
添加helm repo 到本地helm
#helm repo add [NAME] [URL] [flags]   URL:来自git setting-》pages里的服务地址
helm repo add myrepo  https://tyc5412.github.io/helm-c/

#更新repo内容：
#helm repo update [REPO1 [REPO2 ...]] [flags]
helm repo update myrepo