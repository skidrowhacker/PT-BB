Yasir-Alenzi [Skidrow] - Twitter:@firfox20   [ Domain/Sub Enum , Hunting ] 

# Gatherd All Subs  and Export to .txt files Ex: 1.txt , 2.txt
# Total 1,2 .txt Subs - >   using wc 1.txt 2.txt = > {32838} Subs Identfied 
# sorting the 1&2.txt to 3.txt - > cat 1.txt 2.txt |sort -u > 3.txt
# Checking for Live 3.txt Subs using cat 3.txt |httpx -mc 200 > live.txt
# wc live.txt [ there is 476 live subs identfied ] 
# Check for ip probing , server tech , version , title , .. etc using cat live.txt |httpx -mc 200 -ip -probe -title -td -sc > info.txt
# After that i seprate diffrent techs into diffrent .txt file Ex : cat info.txt |grep 'WordPress'  > wp.txt , cat info.txt |grep 'Windows Server' > ws.txt
#After that i get only IPS into seprate File using cat *.txt| grep -o '[0-9]\{1,3\}\.[0-9]\{1,3\}\.[0-9]\{1,3\}\.[0-9]\{1,3\}'  > ip.txt
#After that i Start Hunting ... 


## Tips##
# - >  [Check for all Possible OWASP Top Ten Vulnerabilities]
# - >  [Directory/Paramters Fuzzing] 
# - >  [Dorking] 
# - >  [waybackurls]
# - >  [Fuzz for JS files ]
# - >  [Sub Crawl ]
# - >  [Check Ports and their Servicess runing for Vulnerabilities ]
# - >  [Check for Possbile  CVES ]
# - >  [Enum Plugins , Server Version for Vulnerabilities ]
# - >  [check  Subs Enum for STO]
# - >  [Check Manuly for XSS, SQLI , .. etc] 
# - >  [check for techs used in web and their possible Vulnerabilities ] 
# - >  [ Check Page Source you may find SDE / Links that lead to Vulnerabilities]
# - > [ Check for Domain Enum Road Map  - > [ https://pbs.twimg.com/media/F7bKuHxXsAA1AVo?format=jpg&name=large]
