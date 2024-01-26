### install openssl

---
## **UNDER CONSTRUCTION**
---

sudo apt-get install openssl

for windows, download from https://slproweb.com/products/Win32OpenSSL.html

### Add openssl to path

export PATH=$PATH:/usr/local/ssl/bin

### for windows

set PATH=%PATH%;C:\Program Files (x86)\OpenSSL-Win32\bin

### Generate a private key

openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /path/to/your/private-key.key -out /path/to/your/certificate.crt

### Check CN and SAN and save output to file

openssl x509 -in /path/to/your/certificate.crt -text -noout > /path/to/your/certificate.txt

openssl x509 -in /path/to/your/certificate.crt -text -noout
