# ELEVATE_LABS_INTERNTASKS NO: 1
Tools used: kali linux, nmap.
steps i've did:
  Through #ifconfig command i got my IP address and my ip range.
  By nmap i discovered available devices in my local network.
  Results are saved by the command #nmap -sS <ip> -o scan_results.html.
  Through the nmap script engine i does vulnerabilities on oprn ports of the discovered machine.
  The command that i've used for vulnerability check #nmap --script=vulners.nse -sV -p 21 22 <IP> -o vulnrability_machine.txt
VULNERABILITY FOUNDED:
  SSH(22): CVE-2023-38408, Which allows REMOTE CODE EXECUTION.
  FTP(21): CVE-2011-2523, Which allows BACKDOOR EXECUTION.
