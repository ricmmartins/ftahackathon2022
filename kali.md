## Connecting to Kali

* Connect to the Kali VM over RDP on port 33892. 

```<Public IP Address Of AzureFirewall>:33892```
*  When prompted to choose the setup for the first startup, click to select “Use default config”  
* Create an entry in the HOSTS file (/etc/hosts) on Kali VM to map a name to the Public IP address of the OWASP Juice Shop site published on Application Gateway. Add the linne below at the end of the file:

```<Public IP Address Of the Application Gateway>  juiceshopthruazwaf.com```
 
 
## Commands to run on Kali after the ARM deployment

```
wget --no-check-certificate https://http.kali.org/kali/pool/main/k/kali-archive-keyring/kali-archive-keyring_2022.1_all.deb
sudo apt install ./kali-archive-keyring_2022.1_all.deb
sudo apt-get update
sudo apt-get -y install xrdp
sudo systemctl enable xrdp
echo xfce4-session >~/.xsession
sudo service xrdp restart
```
