Link: https://github.com/AlexisAhmed/BugBountyToolkit

### Docker Image 1
- docker pull hackersploit/bugbountytoolkit
- docker run -it hackersploit/bugbountytoolkit /bin/bash
- cd toolkit
- waf00f demo.testfire.net

### Docker Image 2
- docker pull chvancooten/bugbountyscanner
- docker run -v $(pwd):/root/bugbounty -it chvancooten/bugbountyscanner /bin/bash
- docker run -it --rm chvancooten/bugbountyscanner -d demo.testfire.net --quick > bugbountyscanner_report.txt
- ./BugBountyScanner.sh -d demo.testfire.net --quick > bugbountyscanner_report.txt
  
### Installation:
- git clone https://github.com/AlexisAhmed/BugBountyToolkit.git
- cd BugBountyToolkit
- chmod +x install.sh
- ./install.sh

### Installed Tools:
- altdns : Subdomain discovery through alterations and permutations
- amass
- awscli
- bucket_finder
- CloudFlair
- commix
- dirb
- dirsearch
- dnsenum
- dnsrecon
- dotdotpwn
- droopescan
- fierce
- ffuf
- gobuster
- gitGraber
- httprobe
- joomscan
- Knockpy
- masscan
- massdns
- Nikto
- Nmap
- Recon-ng
- s3recon
- S3Scanner
- sqlmap
- subfinder
- Sublist3r
- subjack
- SubOver
- teh_s3_bucketeers
- thc-hydra
- theHarvester
- tmux
- virtual-host-discovery
- wafw00f
- waybackurls
- wfuzz
- whatweb
- wpscan
- XSStrike
- zsh
