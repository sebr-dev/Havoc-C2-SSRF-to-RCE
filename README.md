# Havoc-C2-SSRF-to-RCE
This is a modified version of the CVE-2024-41570 SSRF PoC from [@chebuya](https://github.com/chebuya/Havoc-C2-SSRF-poc) chained with the auth RCE exploit from [@hyperreality](https://github.com/IncludeSecurity/c2-vulnerabilities/tree/main/havoc_auth_rce). This exploit executes code remotely to a target due to multiple vulnerabilities in [Havoc C2 Framework.](https://github.com/HavocFramework/Havoc)



https://github.com/user-attachments/assets/b75c5934-0326-4994-a695-c18bf95a1e25

<br>

```
usage: CVE-2024-41570.py [-h] -t TARGET -i IP -p PORT -U USERNAME -P PASSWORD [-A USER_AGENT] [-H HOSTNAME] [-d DOMAIN_NAME]
                         [-n PROCESS_NAME] [-ip INTERNAL_IP]

options:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        The listener target in URL format
  -i IP, --ip IP        The IP to open the socket with
  -p PORT, --port PORT  The port to open the socket with
  -U USERNAME, --username USERNAME
                        The username for authentication
  -P PASSWORD, --password PASSWORD
                        The password for authentication
  -A USER_AGENT, --user-agent USER_AGENT
                        The User-Agent for the spoofed agent
  -H HOSTNAME, --hostname HOSTNAME
                        The hostname for the spoofed agent
  -d DOMAIN_NAME, --domain-name DOMAIN_NAME
                        The domain name for the spoofed agent
  -n PROCESS_NAME, --process-name PROCESS_NAME
                        The process name for the spoofed agent
  -ip INTERNAL_IP, --internal-ip INTERNAL_IP
                        The internal ip for the spoofed agent
```
