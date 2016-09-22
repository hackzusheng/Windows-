# Windows-
各种Windows下提取技巧分享

## MySQL(Windows)远程提权漏洞

工具：mysql_win_remote_stuxnet_technique 在exploit文件夹里

## Trusted Service Paths

这个漏洞存在于二进制服务文件路径中Windows错误解释空格。这些服务通常都是以系统权限运行的，如果我们利用这些服务就可能提权到系统权限。

## Vulnerable Services

在讨论易受攻击服务利用的时候我们总谈论下面两类：

1.服务二进制文件(Service Binaries)

2.Windows服务(Windows Services)

## AlwaysInstallElevated

AlwaysInstallElevated是微软允许非授权用户以SYSTEM权限运行安装文件(MSI)的一种设置。然而，给予用于这种权利会存在一定的安全隐患。

## Unattended Installs

自动安装允许程序在不需要管理员关注下自动安装。这种解决方案用于在拥有较多雇员和时间紧缺的较大型组织中部署程序。如果管理员没有进行清理的话，那么会有一个名为Unattend的XML文件残存在系统上。

### PowerUp

PowerUp是一个由Will Schroeder写的PowerShell工具，它会查询当前机器上可用的提权漏洞。多数情况下，如果目标机器存在漏洞，那么我们就可以利用PowerUp工具来进行提权。

https://github.com/PowerShellEmpire/PowerTools/tree/master/PowerUp


