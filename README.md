# Simple IP Response-Server
This is a simple PHP script for calling the Server with Wget or cURL to get your own public IP address.

## Example Calls
These are the example calls you can make on any CLI Device. On your Mac iTerm Terminal, your Raspberry Pi or your Ubuntu production server etc.

### Example call with wget:

```shell
# On Local DEV
wget -qO - 127.0.0.1:8000

# IPv4 call on my io7 Server
wget -qO - ip4.io7.pw

# IPv6 call on my io7 Server
wget -qO - ip6.io7.pw
...
```
### Example call with cURL:
```shell
curl 127.0.0.1:8000
curl ip4.io7.pw
```


## Setup Server
### Local setup / dev
Simply clone this repo and run the inline PHP-Server like

```bash
php -S localhost:8000
```

```bash
php -S 127.0.0.1:8000 -t ./
```
### Live Setup
Be aware that you have to specify on which IP type your server is listening (IPv4 or IPv6).
Best practice to Setup two different Servers which each one of them has a Subdomain for IPv4 and IPv6.


