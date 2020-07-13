```sh
sudo apt update && sudo apt upgrade
sudo apt install raspberrypi-kernel-headers aircrack-ng bc -y
git clone https://github.com/aircrack-ng/rtl8188eus
cd rtl8188eus
sudo -i
echo "blacklist r8188eu" > "/etc/modprobe.d/realtek.conf"
exit
sudo make
sudo make install

git clone https://github.com/MrExpen/airmon-ng.git
cd airmon-ng
sudo chmod +x airmon-ng1
sudo cp airmon-ng1 /user/bin

sudo reboot
```
