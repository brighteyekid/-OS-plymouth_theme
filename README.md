# पवित्र OS-plymouth_theme
This is the custom plymouth theme for the पवित्र OS 

To use is as default bootsplash :- 
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/pavitraos/pavitraos.plymouth 100
sudo update-alternatives --config default.plymouth
sudo update-initramfs -u
