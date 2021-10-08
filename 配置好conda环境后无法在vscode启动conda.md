报错内容为：
“无法加载文件 C:\Users\lenovo\Documents\WindowsPowerShell\profile.ps1，因为在此系统上禁止运行脚本。”

管理员权限启动powershell执行该命令即可，然后将终端重新启动，报错就消失了

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned`

如果发现重启电脑后又出现了同样的问题，可以管理员权限启动powershell，执行该命令，这样会把配置写入注册表，直到下次重新修改配置才会变更

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`