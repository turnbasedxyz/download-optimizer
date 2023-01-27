# Download Optimizer
Use the IP address of a client to determine the best link for them to download from, based on their location.


## Installation
On a Linux or BSD (untested) system:

```
git clone https://github.com/drauger-os-development/download-optimizer
cd download-optimizer
./setup.sh
```
After installation, you will need to open port 80 on your firewall in order to use Download Optimizer. The easiest way to do that is with UFW:

```
sudo ufw enable
sudo ufw allow "nginx full"
```

## Removal
```
./uninstall.sh
```

Remember to close the ports if there not being used for anything else after you unistall.

sudo ufw status numbered

#### MY SERVER

  To                         Action      From
     --                         ------      ----
[ 1] 22/tcp                     ALLOW IN    Anywhere                  
[ 2] Nginx Full                 ALLOW IN    Anywhere                  
[ 3] 22/tcp (v6)                ALLOW IN    Anywhere (v6)             
[ 4] Nginx Full (v6)            ALLOW IN    Anywhere (v6) 

then type the following of the number of the open port for an example we used Nginx full so [ 2] and [ 4] are what we need to delete

sudo ufw delete 2 

( as an example )
