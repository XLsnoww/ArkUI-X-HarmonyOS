# ArkUI-X-HarmonyOS
ArkUI-X进一步将ArkUI扩展到了多个OS平台：目前支持OpenHarmony、HarmonyOS、Android、 iOS，后续会逐步增加更多平台支持。开发者基于一套主代码，就可以构建支持多平台的精美、高性能应用。


ArkUI跨平台框架支持HarmonyOS、Android、 iOS.

## 使用DevEco Studio开发ArkUI-X约束说明

DevEco Studio仅支持ArkUI-X源码开发和调试，各平台Native代码请使用对应平台的IDE编辑器进行开发和调试；

ArkUI-X支持在Android/iOS平台真机和模拟器上运行调试；

## 平台版本及构建工具要求：

OpenHarmony平台：支持API 10+；

Android平台：Android 8+，Level-26，version code: O，Codename: Oreo；

iOS平台：iOS 10+

## 安装ArkUI-X SDK
在File > Settings > ArkUI-X（macOS为DevEco Studio > Preferences > ArkUI-X）下，点击Location右侧的Edit，为SDK选择存储路径。
在弹出的SDK Setup页面选择存储路径，一直点击Next，直到完成SDK的安装后，点击Finish。

## 配置Android SDK安装目录环境变量
配置环境变量ANDROID_HOME，设置Android SDK安装目录。

## Windows环境变量设置方法： 在此电脑 > 属性 > 高级系统设置 > 高级 > 环境变量中，新建系统变量。变量名为ANDROID_HOME，变量值为Android SDK安装目录。

## macOS环境变量设置方法：
1.打开终端工具，执行以下命令，打开.bash_profile文件。

代码语言：shell

vi ~/.bash_profile
2.单击字母“i”，进入Insert模式。

3.输入以下内容，配置Android SDK安装目录。

代码语言：shell
AI代码解释
export ANDROID_HOME=/Users/xxx/Library/Android/sdk
4.编辑完成后，单击Esc键，退出编辑模式，然后输入“:wq”，单击Enter键保存。

5.执行以下命令，使配置的环境变量生效。

代码语言：shell
AI代码解释
source ~/.bash_profile
6.环境变量配置完成后，关闭并重启DevEco Studio。

创建工程
在DevEco Studio中创建跨平台模版工程。

点击File > New > Create Project。
Create Project
Create Project
在打开的模板市场中，选择ArkUI-XEmpty Ability，点击Next。
Empty Ability
Empty Ability
在工程配置页面，填写Project name和Save location，点击Finish，等待模版工程创建完成。
编译构建生成跨平台应用
DevEco Studio可打包生成不同平台的应用包。

在主菜单栏，单击Build > Build Hap(s)/APP(s) > Build APP(s)。

Build APP(s)
Build APP(s)
编译后的ArkTS代码、资源和平台胶水代码已生成到Android和iOS应用工程中，后续安装、运行和调试请使用Android Studio和Xcode。

多端运行效果
我们分别在Harmony、Android和iOS平台运行生成的跨平台应用，查看运行效果。


