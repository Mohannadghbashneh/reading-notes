## Web Scraping

## Reading:
### What is Web Scraping?
- Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites. Web scraping software may directly access the World Wide Web using the Hypertext Transfer Protocol or a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

### Techniques for Web Scraping
- Human copy-and-paste
- Text pattern matching
- HTML parsing
- HTTP programming
- DOM parsing
- Vertical aggregation
- Semantic annotation recognizing
- Computer vision web-page analysis

### Web Scraping best practices to follow to scrape without getting blocked
- Respect Robots.txt
- Make the crawling slower, do not slam the server, treat websites nicely
- Do not follow the same crawling pattern
- Make requests through Proxies and rotate them as needed
- Rotate User Agents and corresponding HTTP Request Headers between requests
- Use a headless browser like Puppeteer, Selenium or Playwright
- Beware of Honey Pot Traps
- Check if Website is Changing Layouts
- Avoid scraping data behind a login
- Use captcha solving services

### Beautiful Soup
- Beautiful Soup is a Python library designed for quick turnaround projects like screen-scraping.
- Three features make it powerful:
- Beautiful Soup provides a few simple methods and Pythonic idioms for navigating, searching, and modifying a parse tree: a toolkit for dissecting a document and extracting what you need. It doesn't take much code to write an application
- Beautiful Soup automatically converts incoming documents to Unicode and outgoing documents to UTF-8. You don't have to think about encodings, unless the document doesn't specify an encoding and Beautiful Soup can't detect one. Then you just have to specify the original encoding.
- Beautiful Soup sits on top of popular Python parsers like lxml and html5lib, allowing you to try out different parsing strategies or trade speed for flexibility.