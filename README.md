## **这个是本人自定义ArchLinux安装镜像编译脚本**

#### 注意 本编译包带有预编译安装包，而且路径需自行修改,本人测试无法固定桌面壁纸
添加了
`lightdm xfce4 archlinuxcn-keyring htop iftop iotop ipmitool mesa libva-intel-driver nvidia-settings lib32-mesa lib32-nvidia-utils bbswitch extra-cmake-modules optimus-manager-qt optimus-manager xfce4-goodies pulseaudio pulseaudio-alsa networkmanager network-manager-applet nm-connection-editor chromium wqy-zenhei xfce4-pulseaudio-plugin pavucontrol lightdm-gtk-greeter yesplaymusic wimlib debootstrap `
#### 1.在开始编译前你先得安装如下软件包
`sudo pacman -S archiso qemu-desktop git edk2-ovmf nano `

#### 2. 然后克隆本项目
`git clone https://github.com/ghhccghk/mydiyarchiso`

#### 3. 执行
`git submodule update --init --recursive`
可以去到233目录下面来更新预编译软件包,233为本地软件包仓库。

#### 4.修改pacman.conf
第101行 `Server = file:///home/ghhc/archlive/233/repo` 改成 `Server = file://克隆完整目录/233/repo`

#### 5.执行build.sh

#### 版权说明
本编译脚本所产生的安装镜像中的部分非开源文件归各自版权人/公司所有，如使用本编译脚本所产生的商业纠纷与本人无关。
airootfs/usr/share/backgrounds/xfce/DSC00346.jpg 此图片本人拿过来当启动图片和桌面壁纸无任何商业用途。
