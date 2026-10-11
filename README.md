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
* [Deepseek harness terminal](https://github.com/mushuanli/dsht): 实现 dsh 的 cli 运行模式并增加计费、定制 prompt、agentic loop 等扩展，并可以进一步针对 dsh 进行深度定制。
* [Mind OS](https://mushuanli.github.io/itookit/),  信息流系统, 集中管理信息，使用数字分身、harness、DAG等实现主动、被动信息处理功能。包括扩展文件系统(支持assetdir, 数据库文件,tag), llm chat/harness/DAG 及数字分身.
* [个人信息Agent](https://github.com/mushuanli/pi-agent), MindOS 的个人智能节点，通过 MCP 接口将本地信息集成到 MindOS.

* [CC-Proxy](https://github.com/mushuanli/cc-proxy): claudecode proxy，在 proxy端观察并控制多个 claudecode 会话运行状态，同时提供计费和session sumarize 等信息。
* [Anki-helper](https://github.com/mushuanli/anki-helper): 使用工作流串联文本生成、图片生成、音频生成实现 多媒体 anki 卡片制作。
* [fd 扩展](https://github.com/sharkdp/fd/): 扩展fd功能实现排除、指定范围等功能。
* [https://github.com/mushuanli/8821cu-20210916]: 移植开源8821cu USB WIFI linux 驱动到最新Linux 7.x内核


# 历史项目
## C
* [tiny sniff](https://github.com/wsue/sniff): 网络抓包和解包工具 ，纯c语言实现无依赖，内部使用 bpf 和 mmap 加速
* [异常解包工具](https://github.com/wsue/excanalyse): QTCREATOR界面的异常分析工具，直观分析 coredump
* [objectdump库](https://github.com/wsue/objwrap): 分析elf文件接口 
* [TCP Proxy](https://github.com/wsue/tcpproxy): 纯C无依赖，进行 TCP 报文转发

## 脚本
* **strace/vargrind**:
* [strace清理](https://github.com/mushuanli/wsue/blob/master/dev/strace_parser.pl): 整理strace输出，更快梳理程序操作内容
* [转换strace pid成 exe](https://github.com/mushuanli/wsue/blob/master/dev/perl_util.pl): 重命名 strace生成的pid文件成可执行程序名,缩小分析范围
* [编译 valgrind脚本](https://github.com/mushuanli/wsue/blob/master/dev/build_valgrind.sh)
* 
* **系统裁剪定制、容器、虚拟机**:
* [裁剪centos并重新打包](https://github.com/mushuanli/wsue/blob/master/dev/repack_centos.sh): 裁剪 centos 并重新生成 iso二次发布
* [在chroot中安装centos环境](https://github.com/mushuanli/wsue/blob/master/ops/install_centos.sh): chroot中安装centos, 比docker提供更高磁盘IO
* [本地建立docker私有仓库](https://github.com/mushuanli/wsue/blob/master/ops/docker-private-registry-compose.yml)
* [从ISO建立OVA映像](https://github.com/mushuanli/wsue/blob/master/ops/create_ova_from_iso.md)
* [通过GOVC管理ESXi](https://github.com/mushuanli/wsue/blob/master/ops/manage_esxi_by_govc.md)
*
* **EKS/Azure/kubernetes**:
* [EKS/Azure辅助脚本](https://github.com/mushuanli/wsue/blob/master/dev/ekshelper.sh): 封装常用eks/azure操作
* [fluentbit 部署文件](https://github.com/mushuanli/wsue/blob/master/dev/configmap-fluentbit2fluentd.yaml): kubernetes常用日志服务器
* [把本机复制成 AWS AMI](https://github.com/mushuanli/wsue/blob/master/ops/local_machine_to_ami.md)
* [把本机复制成 AZURE IMAGE](https://github.com/mushuanli/wsue/blob/master/ops/local_machine_to_azure%E2%80%94%E2%80%94image.md)

# 库
* [C常用功能库](https://github.com/wsue/commonlib)
* [SSL协议库](https://github.com/mushuanli/wsue/blob/master/dev/ssl.c) [OCSP stapling认证](https://github.com/mushuanli/wsue/tree/master/dev/ssl_stapling)


# 文档
OS
* eBPF介绍与编程 https://github.com/mushuanli/wsue/blob/master/dev/ebpf/README.md
* debian相关操作，包括软件、安装配置 https://github.com/mushuanli/wsue/blob/master/ops/debian.md
* docker入门配置 https://github.com/mushuanli/wsue/blob/master/ops/docker.md
* Linux省电模式 https://github.com/mushuanli/wsue/blob/master/ops/linux_powersave.md
* 怎样建立chroot环境 https://github.com/mushuanli/wsue/blob/master/ops/schroot.txt
* wine 软件配置 https://github.com/mushuanli/wsue/blob/master/ops/wine.txt

K8s
* 安装 k8s https://github.com/mushuanli/wsue/blob/master/ops/kubernetes_install.md
* 在k8s上安装 fluent-bit https://github.com/mushuanli/wsue/blob/master/ops/fluent-bit-in-k8s.md
* 在单机环境中建立 kind, 模拟运行k8s https://github.com/mushuanli/wsue/blob/master/ops/k8ssim_kind.yaml
* 定位 k8s问题 https://github.com/mushuanli/wsue/blob/master/ops/kubernetes_debug.md


Cloud


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
