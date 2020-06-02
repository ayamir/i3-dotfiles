# i3-dotfiles
本仓库存放我的dotfiles

软件依赖：
dunst rofi polybar py3status xautolock i3lock ffmpeg compton-tryone-git alacritty feh

使用方法：
只需要把文件夹移动到相应的目录下

Pictures：
存放的是我的壁纸文件，没必要全部下载或者拷贝，各取所需
假设你的图片文件夹是~/Pictures/
```bash
cp -r Pictures/Backgrounds ~/Pictures
```
dunst:
```bash
cp -r dunst/ ~/.config/
```
rofi:
```bash
cp -r rofi/ ~/.config/
```
polybar:
```bash
cp -r polybar/ ~/.config/
```
py3status:
```bash
cp -r py3status/ ~/.config/
```
compton-tryone-git:
```bash
cp compton.conf ~/.config/
```
alacritty；
```bash
cp -r alacritty/ ~/.config/
```
i3lock with blur：
```bash
sudo cp lock/lock.sh /usr/bin/lock && sudo cp lock/lock.png /usr/bin/
```
i3/config
关于i3/config建议结合讲解使用，防止出现问题
13行：将alt键重用为$mod1
26-30行：规定边框和窗口之间的间距
34行：屏幕没有活动5分钟后锁屏（避免看视频时锁屏请使用caffeine-ng）
开机启动部分：
38：交换Esc和Caps键
39：启动网络配置器
40：启动pamac
41：启动fcitx
42：启动xdman
43：启动坚果云
44：启动clipit（剪切板）
45：启动caffeine-ng
47：启动redshift（调节色温）（46行可以注释掉）
48：启动thunderbird
49：启动words-picker（可以注释掉）
50：启动compton
51：启动换壁纸脚本（注意路径）
52：启动polybar
66-88：分配对应窗口出现的默认工作区
91-10行：对应窗口悬浮而非平铺
104-113：按键对应启动应用
112：启动一个名为“WinDev2004Eval”的虚拟机
113：使用lock脚本锁屏
116-128：定义一个在工作区2启动IDEs的模式（如要使用，具体的路径自行注意）
131-139：定义一个启动libreoffice的模式
141-156：定义一个调整redshift等级的模式
163-164：定义快捷键启动rofi不同模式
196：$mod+q切换窗口出现的位置（当前聚焦窗口右或下）
222-231：定义工作区的名字
293-306：定义py3status的配色和出现位置
