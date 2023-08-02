# UOS 统信OS使用

## UOS关闭激活信息提示
提示信息：
```
Your system is not activated. Please activate as soon as possible for normal use.
```
关闭：
```
systemctl stop license.service
systemctl disable license.service
```

## 安装docker和docker-compose
```
curl -s https://github.com/ollcp/uos/raw/main/uos.sh | bash
```

## 防火墙常用操作
```
添加端口：
firewall-cmd --zone=public --add-port=80/tcp --permanent
删除端口：
firewall-cmd --zone=public --remove-port=80/tcp --permanent
添加服务：
firewall-cmd --zone=public --add-service=http --permanent
删除服务：
firewall-cmd --zone=public --remove-service=http --permanent
列出所有规则：
firewall-cmd --list-all
重新加载防火墙规则：
firewall-cmd --reload
列出所有可用的服务：
firewall-cmd --list-services
```
