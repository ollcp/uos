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
