- Link1: https://www.geeksforgeeks.org/installing-openvas-on-kali-linux/
- Link2: https://www.kali.org/blog/configuring-and-tuning-openvas-in-kali-linux/

- sudo apt update                      
- sudo apt upgrade -y
- sudo apt dist-upgrade -y
### Installation of OpenVAS
- sudo apt install openvas
- gvm-setup
- gvm-check-setup

### Passowrd Reset
- gvmd --user=admin --new-password=passwd;
- Sudo gvm-start
- sudo gvm-stop

### Create User
- sudo runuser -u _gvm -- gvmd --create-user=admin2 --new-password=12345 
- sudo runuser -u _gvm -- gvmd --user=admin --new-password=new_password 

### Access toll Ui in browser
- https://127.0.0.1:9392
