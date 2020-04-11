# VPN-IIT-Delhi

## On Linux UBUNTU 18.0

```
    sudo apt install openvpn
    Download all your required files from https://newcert.iitd.ac.in/usermanage/usercert.html
    Put all the files inside one folder
    On the same folder, right click and open terminal
    sudo wget https://raw.githubusercontent.com/jonathanio/update-systemd-resolved/master/update-systemd-resolved -P /etc/openvpn
    sudo chmod 777 /etc/openvpn/update-systemd-resolved
    sudo gedit client.ovpn
    Add the following 2 lines at the end:-
      up /etc/openvpn/update-systemd-resolved
      up /etc/openvpn/update-systemd-resolved
    sudo openvpn --script-security 2 --config client.ovpn
```

## On Windows 10

* Put all the downloaded files inside openvpn/clients folder. Click connect. It's done.
* openvpn is generally installed in the home directly else search for it.
