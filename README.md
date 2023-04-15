# kubebuilder-test
kubebuilder_demo

## 初始化项目架构
```shell
kubebuilder init --domain myid.dev --repo github.com/dierbei/kubebuilder-test
```

## 初始化 CRD
```shell
# y y
kubebuilder create api --group mygroup --version v1alpha1 --kind MyResource
```

## 生成部署清单
```shell
make manifests
```

## 部署
```shell
make install
```

## 生成新版本
```shell
# n n
kubebuilder create api --group mygroup --version v1beta1 --kind MyResource --resource=true
```