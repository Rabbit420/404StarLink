## veinmind-tools <https://github.com/chaitin/veinmind-tools>
<!--auto_detail_badge_begin_0b490ffb61b26b45de3ea5d7dd8a582e-->
![Language](https://img.shields.io/badge/Language-Golang/Python-blue)
![Author](https://img.shields.io/badge/Author-长亭科技-orange)
![GitHub stars](https://img.shields.io/github/stars/chaitin/veinmind-tools.svg?style=flat&logo=github)
![Version](https://img.shields.io/badge/Version-V1.6.5-red)
![Time](https://img.shields.io/badge/Join-20220316-green)
<!--auto_detail_badge_end_fef74f2d7ea73fcc43ff78e05b1e7451-->

veinmind-tools 是由长亭科技自研，基于<a href="https://github.com/chaitin/libveinmind">veinmind-sdk</a>打造的容器安全工具集

## 🔥 Demo
![](https://dinfinite.oss-cn-beijing.aliyuncs.com/image/20220415144819.gif)


## 🕹️ 快速开始
### 1. 确保机器上正确安装 docker
```
docker info
```
### 2. 安装 [veinmind-runner](https://github.com/chaitin/veinmind-tools/tree/master/veinmind-runner) 镜像
```
docker pull veinmind/veinmind-runner:latest
```
### 3. 下载 [veinmind-runner](https://github.com/chaitin/veinmind-tools/tree/master/veinmind-runner) 平行容器启动脚本
```
wget -q https://download.veinmind.tech/scripts/veinmind-runner-parallel-container-run.sh -O run.sh && chmod +x run.sh
```
### 4. 快速扫描本地镜像
```
./run.sh scan-host
```


## 🔨 工具列表

| 工具                                                      | 功能              | 
|---------------------------------------------------------|-----------------|
| [veinmind-runner](https://github.com/chaitin/veinmind-tools/blob/master/veinmind-runner/README.md)            | 扫描工具运行宿主        |
| [veinmind-malicious](https://github.com/chaitin/veinmind-tools/blob/master/plugins/go/veinmind-malicious)     | 扫描镜像中的恶意文件      |
| [veinmind-weakpass](https://github.com/chaitin/veinmind-tools/blob/master/plugins/go/veinmind-weakpass)       | 扫描镜像中的弱口令       |
| [veinmind-sensitive](https://github.com/chaitin/veinmind-tools/blob/master/plugins/python/veinmind-sensitive) | 扫描镜像中的敏感信息      |
| [veinmind-backdoor](https://github.com/chaitin/veinmind-tools/blob/master/plugins/python/veinmind-backdoor)   | 扫描镜像中的后门        |
| [veinmind-history](https://github.com/chaitin/veinmind-tools/blob/master/plugins/python/veinmind-history)     | 扫描镜像中的异常历史命令    |
| [veinmind-asset](https://github.com/chaitin/veinmind-tools/blob/master/plugins/go/veinmind-asset)             | 扫描镜像中的资产信息      |
| [veinmind-webshell](https://github.com/chaitin/veinmind-tools/blob/master/plugins/go/veinmind-webshell)       | 扫描镜像中的 Webshell |
    
PS: 目前所有工具均已支持平行容器的方式运行

## ☁️ 云原生设施兼容性
| 名称                                                          | 类别 | 是否兼容 |
|-------------------------------------------------------------|------|----------|
| [Jenkins](https://github.com/chaitin/veinmind-jenkins)      | CI/CD | ✔️ |
| Gitlab CI                                                   | CI/CD | ✔️ |
| [Github Action](https://github.com/chaitin/veinmind-action) | CI/CD | ✔️ |
| DockerHub                                                   | 镜像仓库 | ✔️ |
| Docker Registry                                             | 镜像仓库 | ✔️ |
| Harbor                                                      | 镜像仓库 | ✔️ |
| Docker                                                      | 容器运行时 | ✔️ |
| Containerd                                                  | 容器运行时 | ✔️ |


<!--auto_detail_active_begin_e1c6fb434b6f0baf6912c7a1934f772b-->
## 项目相关


## 最近更新

#### [v1.6.5] - 2022-12-16

**更新**  
- veinmind-iac 支持扫描 k8s 集群

#### [v1.6.4] - 2022-12-02

**更新**  
- veinmind-iac 增加部分 k8s 相关规则

#### [v1.6.3] - 2022-11-24

**更新**  
- 修复 git 仓库拖取问题  
- git 扫描支持配置代理

#### [v1.6.0] - 2022-11-12

**更新**  
- 新增 veinmind-iac 插件，支持扫描 IaC 文件风险

#### [v1.5.4] - 2022-11-02

**更新**  
- 新增 veinmind-unsafe-mount 插件  
- 移除项目内 python 依赖

<!--auto_detail_active_end_f9cf7911015e9913b7e691a7a5878527-->
