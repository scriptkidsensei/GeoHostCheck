
<h1 align="center"> :boom: Geohostcheck - Host Status Checker with Proxy support</h1>
<em><h5 align="center">(Programming Language - Python 3)</h5></em># 
<p align="center">
 <a href="#"><img alt="GeoHostCheck last commit " src="https://img.shields.io/github/last-commit/scriptkidsensei/GeoHostCheck/main?color=green&style=for-the-badge"></a>
 <a href="#"><img alt="GeoHostCheck License" src="https://img.shields.io/github/license/scriptkidsensei/GeoHostCheck?color=orange&style=for-the-badge"></a>
 
### FREE and OPEN-SOURCE!

*LICENSE : [MIT](https://github.com/scriptkidsensei/GeoHostCheck/blob/main/LICENSE)*

Check the status of an IP address or domain without banning your request!


## Features 
 
- Check the status of hosts with different protocols.
 
- Use proxy servers for checking.
  * 1 check = 1 proxy!
  
- Highly customizable with user agents.
  * Instant automatic user agent changes if proxy or request is banned
   
- Easy to use and robust.
  
- If you don't have a proxy list, geohc will automatically search and download it from the internet.
 


## Screenshots
 
![Header](https://raw.githubusercontent.com/scriptkidsensei/GeoHostCheck/main/img/Screenshot_20231022_230915.png)
 
#### Protocol Choice
 
![DeepinScreenshot_select-area_20231015171230](https://raw.githubusercontent.com/scriptkidsensei/GeoHostCheck/main/img/Screenshot_20231022_230936.png)

#### Status : up
![Screenshot 2](https://raw.githubusercontent.com/scriptkidsensei/GeoHostCheck/main/img/Screenshot_20231022_231211.png)
 
#### Status: down + User-agent
 
![Screenshot 3](https://raw.githubusercontent.com/scriptkidsensei/GeoHostCheck/main/img/Screenshot_20231022_231256.png)
 
#### Automatic proxy list installer!
 
![Screenshot 4](https://github.com/scriptkidsensei/GeoHostCheck/assets/55909183/523e67ac-26a0-473e-bb1d-70e734ef3976)
 
 
 
 ### Support Protocols 
 
 *Line : 449*
 
```python

if protocol == "ICMP":
#imcp proxy ping code...
 
 elif protocol == "UDP":
 send_udp_packet(target_ip, udp_port, protocol, proxy_address)
 elif protocol == "DNS":
 send_tls_request_to_dns(target_ip, tls_port, protocol, proxy_address, user_agent)
 elif protocol == "TCP":
 send_tcp_request(target_ip, tcp_port, protocol, proxy_address, user_agent)
 elif protocol == "TLS":
 send_tls_request(target_ip, tls_port, protocol, proxy_address, user_agent)
```
 
### Support Proxy types
 
```python
# Supports all proxy types
```
 
### User-Agents 
 
*Line : 26*
 
```python
user_agents = [
 "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36",
 "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Firefox/52.0 Safari/537.36",
 "Mozilla/5.0 (Linux; Android 5.1.1; ASUS_X00BD) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.101 Mobile Safari/537.36"
 "Mozilla/5.0 (Linux; Android 9; SM-A530W) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.101 Mobile Safari/537.36"
 "Mozilla/5.0 (Linux; Android 5.0; SM-N900) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Mobile Safari/537.36"
 "Mozilla/5.0 (Linux; Android 11; SM-N770F Build/RP1A.200720.012; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/91.0.4472.101 Mobile Safari/537.36"
 "Mozilla/5.0 (Linux; Android 7.0; LGMP450) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.101 Mobile Safari/537.36"
 "Dalvik/2.1.0 (Linux; U; Android 8.1.0; GOME 2018X38A Build/O11019)"
 "Mozilla/5.0 (iPhone; CPU iPhone OS 14_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/129.0.336390422 Mobile/15E148 Safari/604.1"
 "Mozilla/5.0 (Linux; Android 9; SM-A102U) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.86 Mobile Safari/537.36"
 "Mozilla/5.0 (Linux; Android 9; SM-N976N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.90 Mobile Safari/537.36"
 "Dalvik/1.6.0 (Linux; U; Android 8.1.0; E100 Build/KOT49H)"
]
```
## Documents

```
  TLS  | response = requests.get(f"https://{target_ip}", headers=headers
  HTTP | request = f"GET / HTTP/1.1\r\nHost: {target_ip}\r\n\r\n"
  UDP  | client_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
  TCP  | client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
  ICMP | response = sr1(IP(dst=target_ip) / ICMP(), verbose=0, timeout=2).... *LINE 452*
  DNS  | *LINE 393*
```

# Getting Started
### Requirements

- [Python3](https://www.python.org/downloads/)
- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
- [scapy](https://scapy.net/)
- [pynput](https://pypi.org/project/pynput/)
- [tkinter](https://www.geeksforgeeks.org/python-gui-tkinter/)
- [colorama](https://pypi.org/project/colorama/)
- [requests](https://pypi.org/project/requests/)
  
# Installation
 
You can install Geohostcheck by cloning this repository:

## - :penguin: LINUX -

```shell
git clone https://github.com/scriptkidsensei/GeoHostCheck.git
sudo bash Setup.sh
sudo python3 geohc.py
```

quick

```shell
git clone https://github.com/scriptkidsensei/GeoHostCheck && cd /GeoHostCheck && sudo bash Setup.sh && sudo python3 geohc.py
```

#### termux 

```shell
pkg update && pkg install python automake autoconf m4 build-essential git && git clone https://github.com/scriptkidsensei/GeoHostCheck && cd /GeoHostCheck && sudo bash Setup.sh
```
## - WINDOWS -
Install git [git-scm](https://git-scm.com/)

Open PowerShell or Command Prompt

```
Invoke-WebRequest -Uri https://www.python.org/ftp/python/3.9.6/python-3.9.6-amd64.exe -OutFile python-3.9.6-amd64.exe
Start-Process -Wait -FilePath .\python-3.9.6-amd64.exe
```
Press "Add Python 3.x to PATH",

And

```
git clone https://github.com/scriptkidsensei/GeoHostCheck
cd GeoHostCheck
sudo bash Setup.sh
python3 geohc.py
```

#### Quick usage
```
> python3 geohc.py -h

usage: geohc.py [-h] [--delete-proxy-list] [--install-proxy-list] [--info] [ip] [protocol]

GeoHostChecker

positional arguments:
  ip                    IP address or domain name
  protocol              Protocol to check (e.g., HTTP, ICMP)

options:
  -h, --help            show this help message and exit
  --delete-proxy-list   Delete proxy list
  --install-proxy-list  Install proxy list from the internet
  --info                IP Lookup

```
# :question: Why GeoHC?
Other check applications/sites send requests via static IP address, while geoHC constantly changes proxy (1 req = 1 proxy). 
If requests are banned, the script automatically changes user-agent. If you do not have a proxy list, geohc can download proxy lists from the internet.

 
It took me a lot of effort to make this python script. Please star this repo :D
