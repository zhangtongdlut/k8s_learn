问题描述：重启电脑后之前设置的虚拟机网络都连接不上了

解决：
在vmware中打开
编辑->虚拟机网络编辑器
找到桥接模式的网络，如果找不到，请点击下面的"需要具备管理员特权才能修改网络配置 更改设置"
选择VMnet信息->桥接模式->已桥接至->选择本机的网卡