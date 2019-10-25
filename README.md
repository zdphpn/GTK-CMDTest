# GTK-CMDTest
  gtk+glade+libusb实现的USB接口命令测试工具，仅应用在linux系统。

## 功能
  软件实现对设备(固件)接口(串口)命令的自动化测试，包含以下功能：
1. 可自定义编写测试文件(xml)、测试文件可包含多个分组、每个分组可包含多个测试命令
2. 测试命令可自定义发送、接收数据(正则进行匹配判断)、延时等
3. 测试流程高度灵活，包含按测试文件(包含的分组可配置是否激活)、按组(组内命令可配置是否激活)、定次循环等多种测试方法

## 构成
1. inc：文件夹，头文件
2. output：文件夹，编译输出
3. src：文件夹，源文件
4. ui：文件夹，窗口界面设计文件
 
5. 99-myusb.rules：打开USB读写权限的模板
6. example.xml：测试文件样例
7. install.sh：安装脚本
8. makefile：编译

## 使用

### 准备
  确保系统安装如下软件：pkg-config，libusb-1.0-0-dev，libgtk-3-dev，libxml2-dev

### 开始
1. 在cmdtest文件夹下打开终端
2. 终端执行 make
3. 终端执行 sudo ./install.sh 
4. 终端执行 cmdtest

