# Routeros-shell
需要ios手机app客户端（mikrotik）访问，只能安装7.21.3及以下的低版本。
云服务器安装命令：
```bash
VERSION=7.21.3 bash <(curl https://mikrotik.ltd/chr.sh)
```
1、ros常用命令记录：
首先做好安全防护，关闭风险端口，只保留winbox
```bash
/ip service disable telnet
/ip service disable ftp
/ip service disable www
/ip service disable api
/ip service disable api-ssl
/ip service disable ssh
```
查看当前系统配置的所有参数：
/export

查看接口参数：
/interface print

查看 IP 地址配置：
/ip address print

查看防火墙规则：
/ip firewall filter print

查看 CPU 和 内存 使用情况：
/system resource print

查看日志：
/log print


