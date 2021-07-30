**1.Login as root, run shell in terminal:**

wget --no-check-certificate https://raw.githubusercontent.com/shinpekong/autokms/main/install.sh && chmod +x install.sh && ./install.sh

also, you can download offinstall.tar.gz
https://github.com/shinpekong/autokms/releases/download/0.0.0.1/offinstall.tar.gz

**2.When shell installed, check port 1688:**

netstat -nxtlp | grep 1688

**if back like this mean install KMS success, script will add service in boot:**

    * tcp   0   0 0.0.0.0:1688  0.0.0.0:*       LISTEN      3200/vlmcsd
    * tcp   0   0 :::1688       :::*            LISTEN      3200/vlmcsd

**3.Other help, you must use root do this:**

* service start：
    /etc/init.d/kms start
* service stop：
    /etc/init.d/kms stop
* service restart：
    /etc/init.d/kms restart
* service status：
    /etc/init.d/kms status
* service uninstall：
    /kms.sh uninstall 
