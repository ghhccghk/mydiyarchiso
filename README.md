## **这个是本人自定义ArchLinux安装镜像的预准备目录**

###注意 本编译包带有预编译安装包，而且路径需自行修改

####1.在开始编译前你先得安装如下软件包
`sudo pacman -S archiso qemu-desktop git edk2-ovmf nano `

####2. 然后克隆本项目
`git clone https://github.com/ghhccghk/mydiyarchiso`

####3. 执行`git submodule update --init --recursive`

####4.修改pacman.conf
第101行 `Server = file:///home/ghhc/archlive/233/repo` 改成 `Server = file://克隆完整目录/233/repo`

####5.执行build.sh
