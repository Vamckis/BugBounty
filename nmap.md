### To get the active hosts list
- nmap -sP 192.168.1.0/24 | awk '/is up/ {print up}; {gsub (/\(|\)/,""); up = $NF}'
