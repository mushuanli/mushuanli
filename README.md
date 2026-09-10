### Hi there 👋

<!--
**mushuanli/mushuanli** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
# AI相关
* Deepseek harness terminal, 提供本地cli运行模式，方便 ssh 操作（特别是 ssh + tmux + 跳板机实现手机远程操作）: https://github.com/mushuanli/dsht 
* Mind OS,  新信息文件系统（可建构在浏览器/ 本地文件系统上） + 抽象 LLM DAG + 信息管理功能，最终成为个人 AI 助理： https://github.com/mushuanli/itookit
* CC-Proxy,  claudecode 代理，方便切换不同供应商/不同模型并实时计费， 同时可以分析和跟踪 claudecode交互流程， 同时codex等（未验证）：https://github.com/mushuanli/cc-proxy
* Anki-helper, ai制作图文并茂的英语背书Anki卡片: https://github.com/mushuanli/anki-helper
* fd 扩展, -R 递归指定目录/文件列表， -N 排除指定目录/文件列表, -v 显示命令 & 文件路径信息, https://github.com/sharkdp/fd/
* 8821cu USB WIFI linux 驱动，支持最新Linux 7.x内核: https://github.com/mushuanli/8821cu-20210916
* chatGPT prompt 介绍： https://github.com/mushuanli/wsue/blob/master/dev/gpt/prompt.md


# 项目
## 成品
* *sniff抓包和解包工具* ，c语言实现，使用bpf加速，无依赖，带有包过滤功能，同时可以快速增加其他协议解包 https://github.com/wsue/sniff
* *异常解包工具* ，QTCREATOR界面，用于分析程序异常打印，并且输出对应代码和汇编上下文信息 https://github.com/wsue/excanalyse
* *封装objectdump* , 提供分析elf文件接口 https://github.com/wsue/objwrap
* *TCP转发工具* ，接收TCP请求然后连接外部服务器，主要用于某些环境LINUX无法直接上网时提供跳板 https://github.com/wsue/tcpproxy

## 脚本
* *strace输出处理*  ，过滤和处理strace输出   https://github.com/mushuanli/wsue/blob/master/dev/strace_parser.pl
* 重命名 strace生成的pid文件成可执行程序名 https://github.com/mushuanli/wsue/blob/master/dev/perl_util.pl
* 对centos重新打包  https://github.com/mushuanli/wsue/blob/master/dev/repack_centos.sh
* 对pod进行辅助管理的脚本，pod编号难定位，这里简化成按序号对pod操作 https://github.com/mushuanli/wsue/blob/master/dev/ekshelper.sh
* fluentbit 部署文件 https://github.com/mushuanli/wsue/blob/master/dev/configmap-fluentbit2fluentd.yaml
* 编译 valgrind脚本  https://github.com/mushuanli/wsue/blob/master/dev/build_valgrind.sh
* 拨号上网脚本  https://github.com/mushuanli/wsue/blob/master/config/vpn.sh
* 在chroot中安装centos环境 https://github.com/mushuanli/wsue/blob/master/ops/install_centos.sh
* 以docker方式运行wordpress https://github.com/mushuanli/wsue/blob/master/ops/wordpress_docker.sh
* 本地建立docker私有仓库 https://github.com/mushuanli/wsue/blob/master/ops/docker-private-registry-compose.yml

## 半成品
* letcode刷题c语言实现 https://github.com/mushuanli/letcode
* gowebserver, 简单实现下载、网页、认证功能，主要用于帮助内部验证 https://github.com/mushuanli/gowebserver
* 简单echo框架，用于辅助开发验证工具 https://github.com/wsue/echoserver

C函数
* C语言开发使用的一些常用操作函数，https://github.com/wsue/commonlib 
* 另外一些c开发使用的常用网络函数 https://github.com/mushuanli/wsue/blob/master/dev/netbase.cpp https://github.com/mushuanli/wsue/blob/master/dev/code_util.c

SSL
* SSL 协议API， C实现SSL协议 https://github.com/mushuanli/wsue/blob/master/dev/ssl.c
* SSL增加 OCSP stapling证书校验 https://github.com/mushuanli/wsue/tree/master/dev/ssl_stapling
* ssl协议验证工具，用于开发自己的SSL 连接验证 https://github.com/wsue/prototest

# 文档
OS
* eBPF介绍与编程 https://github.com/mushuanli/wsue/blob/master/dev/ebpf/README.md
* debian相关操作，包括软件、安装配置 https://github.com/mushuanli/wsue/blob/master/ops/debian.md
* docker入门配置 https://github.com/mushuanli/wsue/blob/master/ops/docker.md
* Linux省电模式 https://github.com/mushuanli/wsue/blob/master/ops/linux_powersave.md
* office软件问题解决 https://github.com/mushuanli/wsue/blob/master/ops/office
* 怎样建立chroot环境 https://github.com/mushuanli/wsue/blob/master/ops/schroot.txt
* wine 软件配置 https://github.com/mushuanli/wsue/blob/master/ops/wine.txt

K8s
* 安装 k8s https://github.com/mushuanli/wsue/blob/master/ops/kubernetes_install.md
* 在k8s上安装 fluent-bit https://github.com/mushuanli/wsue/blob/master/ops/fluent-bit-in-k8s.md
* 在单机环境中建立 kind, 模拟运行k8s https://github.com/mushuanli/wsue/blob/master/ops/k8ssim_kind.yaml
* 定位 k8s问题 https://github.com/mushuanli/wsue/blob/master/ops/kubernetes_debug.md


Cloud
* 从ISO建立OVA映像  https://github.com/mushuanli/wsue/blob/master/ops/create_ova_from_iso.md
* 把本机复制成 AWS AMI https://github.com/mushuanli/wsue/blob/master/ops/local_machine_to_ami.md
* 把本机复制成 AZURE IMAGE https://github.com/mushuanli/wsue/blob/master/ops/local_machine_to_azure%E2%80%94%E2%80%94image.md
* 通过GOVC管理ESXi https://github.com/mushuanli/wsue/blob/master/ops/manage_esxi_by_govc.md


Dev
* ios开发和mac系统环境安装软件等问题指南 https://github.com/mushuanli/wsue/blob/master/dev/ios.md
* bash编程 https://github.com/mushuanli/wsue/blob/master/dev/bash_program.md


# 个人
## 配置文件
* VIM配置 https://github.com/mushuanli/vimfiles https://github.com/mushuanli/wsue/blob/master/config/vimrc.local
* NVIM 配置(使用lua) https://github.com/mushuanli/nvimfiles
* TMUX配置 https://github.com/mushuanli/wsue/blob/master/config/tmux.conf

## 阅读
* 失控 https://github.com/mushuanli/wsue/tree/master/xmind/out_of_control
* 云计算 https://github.com/mushuanli/wsue/tree/master/xmind/cloud
