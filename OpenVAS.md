### Installation
- Link: https://www.geeksforgeeks.org/installing-openvas-on-kali-linux/
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
