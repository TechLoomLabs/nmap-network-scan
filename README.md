# nmap-network-scan
Elevate Labs  Task No. 1

### Step-by-Step Execution Guide ###
## Step 1 & 2 : Installation & Finding the local IP Range.
* Action : Installed Nmap and identified the local IP Range 
* Details : Found the local IPv4 address ("10.203.22.14")
* Subnet Range : "10.203.22.0/24"

## Step 3 & 4 : Running the TCP SYN Scan & Locating Ports.
* Action : Performed a stealth TCP SYN scan across the local subnet
* Commands : namp -sS IPv4

## Step 5 & 6 : 
* Action : Probed open ports to determine exact version running on the target machine 
* Command : nmap -sV IPv4

## Step 7 :
* Evaluation : Reviewed open ports to analyze network exposure. 
               Found unencrypted HTTP traffic and core windows file sharing ports.

## Step 8 : 
* Action : Exported the scan result into normal text and XML formats for reporting. 
* Commands : nmap -sS IPv4 -oN scan_result.txt
             nmap -sS IPv4 -oX scan_result.xml
