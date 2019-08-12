# splash_screen

## install
copy files in /usr/share/plymouth/themes/
```
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/notilo-logo/notilo-logo.plymouth 200
sudo update-alternatives --set default.plymouth /usr/share/plymouth/themes/notilo-logo/notilo-logo.plymouth
#sudo update-alternatives --config default.plymouth
sudo update-initramfs -u
```

## test
```
sudo plymouthd
sudo plymouth --show-splash
sudo plymouth quit
```

ex:
```
sudo plymouthd && sudo plymouth --show-splash && sleep 20 && sudo plymouth quit
```
