# Site Sniffer in Python 🐽

Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.

#

## Installation

Install sitesniffer with pip

```bash
  pip install sitesniffer
```

## Usage
To use SiteSniffer, you need to import it first:
```bash
  from sitesniffer import SiteSniffer
```

Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
```bash
  sniffer = SiteSniffer('https://example.com')
```

You can then call the methods of the SiteSniffer object to get various details about the website:
```bash
  print(sniffer.ip_address())
  print(sniffer.domain_info())
  print(sniffer.status_code())
  # See docs for full list
```

Each of the methods in this package returns the corresponding detail of the website. For example, get_ip_address() returns the IP address of the website.

## Example

```bash
  from sitesniffer import SiteSniffer

  sniffer = SiteSniffer('https://google.com')
  print(sniffer.ip_address())
```
## Output
```bash
  142.250.185.110
```
#

## Essential Python Libraries for Web Scraping and HTTP Requests

The following Python libraries are essential for working with the Site Sniffer package:

* requests: used for sending HTTP requests and receiving responses.
* socket, ssl, and idna: used for working with IP addresses and SSL certificates.
* whois: used for querying WHOIS information for a domain.
* re: used for working with regular expressions.
* time: used for timing how long it takes to load a webpage.
* BeautifulSoup: used for parsing HTML.



## The defined functions included (docs):

| Function Name  | Function Description |
| ------------- | ------------- |
| SiteSniffer | A class for extracting information about a website, such as its IP address, SSL certificate information, and load time. |
| extract_protocol | Extracts the protocol from the URL. |
| extract_hostname | Extracts the hostname from the URL. |
| extract_path | Extracts the path from the URL. |
| ip_address | Returns the IP address of the domain. |
| domain_info | Returns the domain information for the website. |
| status_code | Returns the HTTP status code of the website. |
| ssl_info | Returns the SSL certificate information for the website. |
| load_time | Returns the website's load time. |
| links | Returns a list of links found on the website. |
| is_mobile_friendly | Checks if the website is mobile-friendly. |
| has_responsive_design | Checks if the website has a responsive design. |
| has_cookies | Checks if the website uses cookies. |
| has_google_analytics | Checks if the website has Google Analytics installed. |
| page_meta_description | Returns the website's meta description. |
| has_meta_description | Checks if the website has a meta description. |
| page_keywords | Returns the website's keywords. |
| has_keywords | Checks if the website has keywords. |

#
[![License: MIT](https://img.shields.io/badge/License-MIT-darkgrey.svg)](https://opensource.org/licenses/MIT)
