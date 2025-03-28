# HostHatch 与 RackNerd VPS 一键 DD 脚本合集：快速安装 Windows 系统指南

## 准备工作：安装系统重装必备组件

在开始 DD 安装前，请确保已安装以下基础组件：

### Debian/Ubuntu 系统
bash
apt-get install -y xz-utils openssl gawk file wget screen && screen -S os

### RedHat/CentOS 系统
bash
yum install -y xz openssl gawk file glibc-common wget screen && screen -S os

若出现异常，建议更新软件源缓存：
- **RedHat/CentOS**:
  bash
  yum makecache && yum update -y
  
- **Debian/Ubuntu**:
  bash
  apt update -y && apt dist-upgrade -y
  

👉 [【点击查看】2025年最新 Racknerd 优惠码及特价云服务器方案汇总](https://bit.ly/Rack_Nerd)

## 智能一键安装脚本详解

这款全能 DD 脚本具有以下优势：
- 支持国内外各类 VPS 重装系统
- 特别优化对国内访问国外资源慢的 VPS
- 完美支持 Debian 11
- 内置 Oracle Cloud（甲骨文云）专用选项（23-25）

**安装命令**：
bash
wget --no-check-certificate -O AutoReinstall.sh https://d.02es.com/AutoReinstall.sh && chmod a+x AutoReinstall.sh && bash AutoReinstall.sh

### 使用说明
1. 输入 `Y` 确认自动获取 IP，或 `N` 手动设置
2. 25 合 1 系统选择界面，输入 99 可使用自定义镜像
3. 系统安装完成后会自动重启

## 25 合 1 系统默认密码清单

| 系统版本 | 默认密码 |
|---------|---------|
| CentOS 7.7 | Pwd@CentOS |
| CentOS 7/8 | cxthhhhh.com |
| Windows Server 2019/2016/2012 | cxthhhhh.com |
| Windows 10 LTSC Lite | www.nat.ee |
| Windows 7 系列 | 详见对应版本 |
| Oracle Cloud 专用镜像 | nat.ee |

> **重要提示**：谷歌云 DD 时若子网掩码显示为 255.255.255.255，需手动修正为 255.255.255.0

## 自定义 DD 包安装方法

bash
wget --no-check-certificate -qO InstallNET.sh 'https://d.02es.com/InstallNET.sh' && bash InstallNET.sh -dd '[Windows DD包直链地址]'

## 实用技巧
- Windows 服务器开启 Ping 功能：按 `Win+R` 输入相关命令
- Oracle Cloud 建议选择 Ubuntu 作为基础系统
- 使用精简版 DD 包可节省安装时间

如需更多 VPS 使用技巧和优质云服务器推荐，请持续关注我们的更新。