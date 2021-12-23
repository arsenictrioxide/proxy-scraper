Scrape more than 1K HTTP proxies in less than 2 seconds.

Scraping fresh public proxies from different sources:

sslproxies.org (HTTP, HTTPS)
free-proxy-list.net (HTTP, HTTPS)
us-proxy.org (HTTP, HTTPS)
socks-proxy.net (Socks4, Socks5)
proxyscrape.com (HTTP, Socks4, Socks5)
proxy-list.download (HTTP, HTTPS, Socks4, Socks5)
Installation
Use this command to install dependencies.

pip3 install -r requirements.txt
Usage
For scraping:

python3 proxyScraper.py -p http
With -p or --proxy, You can choose your proxy type. Supported proxy types are: HTTP - HTTPS - Socks (Both 4 and 5) - Socks4 - Socks5
With -o or --output, create and write to a .txt file. (Default is output.txt)
With -v or --verbose, more details.
With -h or --help, Show help to who did't read this README.
For checking:

python3 proxyChecker.py -t 20 -s google.com -l output.txt
With -t or --timeout, dismiss the proxy after -t seconds (Default is 20)
With -p or --proxy, check HTTPS or HTTP proxies (Default is HTTP)
With -l or --list, path to your list.txt. (Default is output.txt)
With -s or --site, check with specific website like google.com. (Default is google.com)
With -r or --random_agent, it will use a random user agent per proxy.
With -v or --verbose, more details.
With -h or --help, Show help to who did't read this README.
Good to know
Dead proxies will be removed and just alive proxies will stay.
This script is also able to scrape Socks, but proxyChecker only check HTTP(S) proxies.
Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Credit
Proxy Scraper
Proxy Checker
License
