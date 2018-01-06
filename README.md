# python-jump-android

首先感谢万能的github战友，原理：利用像素识别测量出起始和目标点之间的距离，乘以按压时间系数。

代码来源: https://github.com/wangshub/wechat_jump_game  本人只是小做改动，多谢大神的肩膀。
Tips:该来源中还包含ios及其他版本。

环境：
1.adb.exe、AdbWinApi.dll、AdbWinUsbApi.dll、fastboot.exe，配置android环境，用于执行shell截图和获取图片，如有可以不下载；
2.python.exe，配置python环境，用于执行脚本，如有可以不下载；

步骤：
1.双击python.exe，安装python运行环境，无需自定义的话默认下一步即可,安装过程中会自动配置python、pip等环境变量；
2.打开命令行，打开当前目录，执行 pip install -r requirements.txt；
3.将安卓手机用usb线连接到电脑，将安卓手机的 USB 调试模式打开，设置 > 更多设置 > 开发者选项，将开发者选项和usb调试都打开；
4.打开微信，打开跳一跳，点击开始游戏；
5.在命令行当前目录，执行 python wechat_jump_auto.py；
6.根据提示，输入y，按回车；
7.开始游戏！

Tips:如出现第一步就跳太近或跳太远的情况，请打开wechat_jump_auto.py，第46行,尝试替换成press_coefficient = 1,或press_coefficient = 1.392,可解决大部分兼容问题。config目录下有很多整理好的配置文件，可根据需要自行引用或修改。

仅供娱乐，不要玩太嗨，万一跳一跳要那啥，哈哈
