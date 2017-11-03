# FancyProx
A in-browser proxy designed to bypass firewalls. It also supports larger caching enabling sites that have been loaded once to have a faster response time. This is all built to run on google appspot

### How does it work?

The application is truly simple but comes with certain limitations. First the website will take any **get** requests from the client and then replicate the same request on the server side, relaying those results back with minor changes. Anything that contains an easily discoverable URL will be replaced with a new relative URL ponting  to the proxy. Any images/multimedia content will be cached on the server to enable faster loading on something like a reload. Any request that generally contains sensitive data like **post** are rejected to protected user privacy. 

#### What makes it different?

- The caching system enables faster loading
- Pages are generally better preserved on FancyProx versus other proxies
- The proxy is completely free and hides possible firewall trigger-words 

#### Limitations 

* Data is not encrypted with HTTPS making it public
* Any urls loaded through javascript (ReactJS heavy website) end up crashing

### Features

- [x] General Proxy Support
- [x] Loading large images
- [x] URL Modification
- [x] Webpage Path Obfuscation
- [ ] HTTPS Support
- [ ] Javascript URL modification

### Libraries Used

* [App Engine](https://cloud.google.com/appengine/) - Hosting and caching support
* [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/) - Website scraping and modification

