
## Frp服务端一键配置脚本，脚本默認获取Frp最新版本  
## Frp server one-click configuration script. The script obtains the latest Frp version by default

[![GitHub Repo][repo-shield]][repo-url]
[![Stars][stars-shield]][stars-url]
[![Forks][forks-shield]][forks-url]

[repo-shield]: https://img.shields.io/badge/GitHub-mvscode%2Ffrps--onekey-brightgreen?style=flat-square&logo=github
[repo-url]: https://github.com/mvscode/frps-onekey
[stars-shield]: https://img.shields.io/github/stars/mvscode/frps-onekey.svg?style=flat-square&logo=github&color=yellow
[stars-url]: https://github.com/mvscode/frps-onekey/stargazers
[forks-shield]: https://img.shields.io/github/forks/mvscode/frps-onekey.svg?style=flat-square&logo=github&color=green
[forks-url]: https://github.com/mvscode/frps-onekey/network/members


*Frp 是一个高性能的反向代理应用，可以帮助您轻松地进行内网穿透，对外网提供服务，支持 tcp, http, https 等协议类型，并且 web 服务支持根据域名进行路由转发。*

* 详情：fatedier[<img alt="github" src="https://img.shields.io/badge/github/fatedier/frp-8da0cb?style=for-the-badge&labelColor=555555&logo=github" height="16">](https://github.com/fatedier/frp)
* 此脚本原作者：clangcn [<img alt="github" src="https://img.shields.io/badge/github/clangcn/onekey_install_shell-8da0cb?style=for-the-badge&labelColor=555555&logo=github" height="16">](https://github.com/clangcn/onekey-install-shell)

## Frps-Onekey-Install-Shell For CentOS/Debian/Ubuntu/Fedora (32bit/64bit)

### Install（安装）

#### Gitee
```Bash
wget https://gitee.com/mvscode/frps-onekey/raw/master/install-frps.sh -O ./install-frps.sh
chmod 700 ./install-frps.sh
./install-frps.sh install
```
#### Github
```Bash
wget https://raw.githubusercontent.com/mvscode/frps-onekey/master/install-frps.sh -O ./install-frps.sh
chmod 700 ./install-frps.sh
./install-frps.sh install
```


### Uninstall（卸载）
```Bash
./install-frps.sh uninstall
```
### Update（更新）
```Bash
./install-frps.sh update
```
### Server management（服务管理器）
```Bash
Usage: /etc/init.d/frps {start|stop|restart|status|config|version}
```
 
## Script ChangeLog
---------------------------------------
### [1.0.1] - 2024-06-07

#### Changed
* frps program config file change to frps.toml from frps.int

### [1.0.2] - 2024-06-13

#### Update
* Update frp server config format to follow up the latest version.
  ```
  bind_addr --> bindAddr
  bind_port --> bindPort
  kcp_bind_port --> kcpBindPort
  etc..
  ```

### [1.0.3] - 2024-06-16

#### Amendment
* Amend function name to frps

#### Changed
* Change curl common to get server ip from wget common


### [1.0.4] - 2024-06-18

#### Update
* Add trace option at log level, default is still info

* Update shell update function, ask the user if they want to update

 
  
