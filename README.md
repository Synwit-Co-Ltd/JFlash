# JFlash
add Synwit MCU Support to Segger J-Flash.

## for JLink V7.62 and before

Step 1. 将 `Synwit` 文件夹复制到 \<Jlink installation directory>/Devices 目录下   
Step 2. 将 `JLinkDevices.xml` 文件中 \<DataBase> 和 \</DataBase> 之间的内容复制粘贴到 \<Jlink installation directory>/JLinkDevices.xml 文件中的 \<DataBase> 后面

## for newer versions of JLink

Step 1. 检查如下目录（后面以 \<SEGGER> 指代）下是否有 JLinkDevices 文件夹，若没有则新建
```
OS      Location
Windows C:\Users\<USER>\AppData\Roaming\SEGGER
Linux   $HOME/.config/SEGGER
macOS   $HOME/Library/Application Support/SEGGER
```

Step 2. \<SEGGER>/JLinkDevices 目录下新建 Synwit 文件夹，将 `JLinkDevices.xml` 文件复制到 \<SEGGER>/JLinkDevices/Synwit 目录下   
Step 3. \<SEGGER>/JLinkDevices/Synwit 目录下新建 Devices 文件夹，将 `Synwit` 文件夹复制到 \<SEGGER>/JLinkDevices/Synwit/Devices 目录下

备注：对于 Windows 系统，将 C:\\Users\\\<USER>\\AppData\\Roaming\\SEGGER 中的 \<USER> 替换为实际用户名（以 lucy 为例），然后将 C:\\Users\\lucy\\AppData\\Roaming\\SEGGER 粘贴到 Windows 文件资源管理器的地址栏中回车，即可打开 SEGGER 目录。
