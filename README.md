# BugBounty
Includes Steps of my BugBounties

### Step1: Google Dorking
- inurl:netflix.com password|credential|username filetype:log
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private filetype:pdf
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private | WS_FTP | ws_ftp | log | LOG filetype:log
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private filetype:xls
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private filetype:csv
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private filetype:doc
- inurl:netflix.com not for distribution | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private filetype:txt

# Run Chandrahasa - Automation tool of steps 2,3,4
- chmod +x chandrahasa.sh 
- ./chandrahasa.sh websitename.com

### Step2: Subdomainer
- ./subdomainer -t netflix.com -f true

### Step3: httpx
- cat all.txt | httpx -mc 200,403 -o liveallurls.txt
 
### Step4: Nuclei
- nuclei -t /root/nuclei-templates/ -l all-live.txt -es info -o nucleiall.txt

