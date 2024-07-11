argocd原理：
k8s 运行一个 argocd 的application

这个app 配置了 helm位于github中的git地址和分支，
并监听git数据的更新，
当有数据更新时，argocd就会自动去刷新helm的更新对应k8s资源如pod等等