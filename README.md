# WebSiteCloner

## Description
This package implement a Web Site Cloner and his HTTP server to launch it.

## Requirements
This package require :
 - python3
 - python3 Standard Library

## Installation
```bash
pip install WebSiteCloner
```

## Launcher

 - Command line:
 ```bash
 WebSiteCloner -r -d ClonedWebSites -D "localhost:8000" -f "logs.log" -l DEBUG -S http "https://www.google.com/"
 WebClonerServer -f "logs.log" -S Apache -I "172.16.89.53" -H Set-Cookie:1278=1278,Set-Cookie:a=a,Test:haha -P 8000 "www.google.com"
 ```

 - Python:
 ```python
 import WebSiteCloner
 copy: WebSiteCloner.WebSiteCloner = WebSiteCloner.WebSiteCloner(
     "https://www.google.com/",
     recursive=True,
     directory="ClonedWebSites",
     replace_domain="localhost:8000",
     replace_scheme="http",
     loglevel=10,
     logfile="logs.log",
 )
 copy.launch()
 ```

## Links
 - [Github Page](https://github.com/mauricelambert/WebSiteCloner)
 - [Code Documentation](https://mauricelambert.github.io/info/python/security/WebSiteCloner.html)
 - [Download as python executable](https://mauricelambert.github.io/info/python/security/WebSiteCloner.pyz)

## Licence
Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).