# vulmap-windows
Host-based local vulnerability scanner. Finds installed software on the host, asks their vulnerabilities to vulmon.com API and print vulnerabilities with available exploits. All found exploits can be downloaded by Vulmap.

## Screenshots
![Screenshot from terminal](https://raw.githubusercontent.com/yavuzatlas/vulmap-windows/master/bir.jpg)

![Screenshot-2 from terminal](https://raw.githubusercontent.com/yavuzatlas/vulmap-windows/master/iki.jpg)

## Recommended Platform
Compatible with PowerShell v3 and higher

### Examples

.EXAMPLE
PS> Invoke-Vulmap

Default mode. Conducts a vulnerability scanning.

.EXAMPLE
PS> Invoke-Vulmap -OnlyExploitableVulns

Conducts a vulnerability scanning and only shows vulnerabilities that have exploits

.EXAMPLE
PS> Invoke-Vulmap -DownloadExploit EDB9386

Downloads given exploit

.EXAMPLE
PS> Invoke-Vulmap -DownloadAllExploits

Scans the computer and downloads all available exploits
