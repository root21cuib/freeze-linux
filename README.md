# freeze-linux
this is an explicit explanation on what to do whenever your linux (kali) freezes after you log in or just after the installation process
I dig some research and I think the issue may be with your lightdm or gdm3 
Press CTRL+ ALT + F4 after then you login your usernname and password. Type the following commands
sudo apt-get purge lightdm
sudo apt-get update
sudo apt-get full-upgrade -y
sudo apt-get install lightdm or  sudo apt-get install -f gdm3 (choose anyone)
sudo dpkg-reconfigure lightdm
apt-get install gnome
sudo shutdown -r (to reboot your machine)
