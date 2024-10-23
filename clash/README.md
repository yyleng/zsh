## change selinux config

vim /etc/selinux/config

## create clash service

sudo mv clash.service /usr/lib/systemd/system
systemctl enable clash.service
systemctl start clash
systemctl restart clash

## Enable Proxy

export http_proxy=http://127.0.0.1:7890 && export https_proxy=http://127.0.0.1:7890
