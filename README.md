# barebones_linux
## busybox + the linux kernel 
nothing really
# HOW TO MAKE .ISO FILE
1. git clone the repo
2. create an empty .iso file using dd --> dd if=/dev/zero of=/boot.iso bs=1M count="whatever size you want"
3. change the filesystem of the .iso file to FAT using mkfs -t fat boot.iso
4. install syslinux bootloader and run syslinux boot.iso
5. mount the .iso file to a folder and copy bzImage and init.cpio
6. umount the folder
7. use qemu to try the most barebones functional linux kernel(the files will not save after reboot!!!!)
