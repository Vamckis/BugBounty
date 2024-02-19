### To get the active hosts list
- nmap -sP 192.168.1.0/24 | awk '/is up/ {print up}; {gsub (/\(|\)/,""); up = $NF}'
- nmap -T4 -A -v -Pn --script http-auth-finder,http-auth,http-config-backup,http-csrf,http-dombased-xss,http-form-fuzzer,http-frontpage-login,http-iis-webdav-vuln,http-internal-ip-disclosure,http-passwd,http-rfi-spider,http-robots.txt,http-sql-injection,http-stored-xss,http-webdav-scan,ms-sql-info,ssl-enum-ciphers,ssl-heartbleed,ssl-poodle <hostname>
