## 准备

kali vm + smb服务  按照课内材料在kali上安装smb
Windows vm
最好将文件放在共享目录下并将out软链接到/var/www/html
把工具放在/var/www/html/tools中

## 使用方法

./Generator.py

./Generator.py tun0

./Generator.py eth0

按提示在windows上打开payloads.sln,编译程序(可能需要修改生成程序的路径)

所有结果都生成在out中

所有url和命令都在usage.md,直接复制命令


## C\#
- [x] inject 进程注入 exe
- [x] hollowing exe
- [x] inject dll
- [x] hollowing dll
- [x] Dotnet2jscript inject dll
- [x] Dotnet2jscript hollowing dll
- [x] BypassCLM exe 
`C:\Windows\Microsoft.NET\Framework64\v4.0.30319\installutil.exe /logfile= /LogToConsole=false /U C:\Users\admin\Desktop\BypassCLM.exe`
- [x] aspx
- [X] compiler绕过白名单
- [x] Installer直接反弹shell绕过白名单

---
## ps1
- [x] inject.ps1 直接注入
- [x] reflection.ps1 powershell反射 inject/hollow
- [x] netreflection.ps1net反射dll <span style="color:red">__路径可能需要修改__</span>
- [x] msfvenom直接生成的 

---
## vba
- [x] loader.vba 普通方法 x86
- [x] vba执行powershell 调用WMI 6.8.2 可以是x64 必须修改为runner.doc

---
## hta
- [x] 绕过白名单

---
## xsl
- [x] Compiler白名单绕过
http://<ip>/other/test.xml
http://<ip>/other/test.txt
- [X] wmic执行powershell 放到了Csharp中





