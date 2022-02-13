## Cấu hình RDP cho Ubuntu 18.04, 20.04, 20.10, 21.04

Tham khảo tại https://c-nergy.be/blog/?p=16817

Lưu ý chạy lệnh script trên tài khoản không phải quyền root
```
chmod +x  xrdp-installer-1.2.3.sh
bash xrdp-installer-1.2.3.sh

# Cấu hình fix lỗi
nano /etc/xrdp/startwm.sh

Và dán đoạn lệnh bên dưới vào
unset DBUS_SESSION_BUS_ADDRESS
unset XDG_RUNTIME_DIR
. $HOME/.profile
```
