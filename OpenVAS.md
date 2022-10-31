- Link1: https://www.geeksforgeeks.org/installing-openvas-on-kali-linux/
- Link2: https://www.kali.org/blog/configuring-and-tuning-openvas-in-kali-linux/
- Youtube Link: https://www.youtube.com/watch?v=LGh2SetiKaY

- apt update                      
- apt upgrade -y
- apt dist-upgrade -y
- gvm-feed-update

### Installation of OpenVAS
- apt install openvas
- gvm-setup
- gvm-check-setup

### Passowrd Reset
- gvmd --user=admin --new-password=pass;

- Sudo gvm-start
- sudo gvm-stop

### Create User
- sudo runuser -u _gvm -- gvmd --create-user=admin2 --new-password=12345 
- sudo runuser -u _gvm -- gvmd --user=admin --new-password=new_password 

### Access UI in browser
- https://127.0.0.1:9392

### Steps to follow:
- Adminisration --> Feed Status
- Configuration --> Targets, Port Lists, Scan Configs
- Scans --> Tasks, Reports, Results, Vulnerabilities

Check for QoD (Quality Of Defects) for each scan.
