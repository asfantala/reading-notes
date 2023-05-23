# Web Scraping

### What are the key differences between scraping static and dynamic websites?
- The differences between static and dynamic websites:

- Static websites have static content, which means that the content does not change frequently. Dynamic websites have dynamic content, which means that the content can change frequently.
- Static websites store their HTML code on the server. Dynamic websites generate their HTML code on the client side.
- Static websites are easier to scrape than dynamic websites. This is because static websites have static content, which means that the content is always in the same place. Dynamic websites have dynamic content, which means that the content can change frequently, making it more difficult to scrape.
### Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.
- Respect Robots.txt

Robots.txt is a file that tells web crawlers which pages they can and cannot access on a website. If you are scraping a website, it is important to respect Robots.txt and only crawl the pages that are allowed.

- Make the crawling slower

Crawling a website too quickly can put a strain on the website's servers and may result in you being blocked. It is important to crawl a website slowly and make sure that you are not making too many requests in a short period of time.

- Do not follow the same crawling pattern

Websites can often detect web crawlers by the patterns in their requests. To avoid being blocked, it is important to vary your crawling pattern. This means making requests at different times of day, from different IP addresses, and using different user agents.

### What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

- Playwright is a web automation framework that can be used to automate tasks on websites. Playwright can be used for web scraping tasks, such as extracting data from websites.
 For example, Playwright can be used to scrape websites that require authentication or that use JavaScript to dynamically generate content.


### Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.
- XPath is a language that can be used to select nodes in an XML document. XPath can be used in web scraping to select HTML elements from a webpage.
example:  
//div[@class="product-name"]