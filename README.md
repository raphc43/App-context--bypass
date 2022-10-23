# Problem
Unlike web scraping, mobile scraping (Hybrid apps) is 180 degrees different, as URLs in particular cannot be scraped directly by using Selenium/Appium. Its all due to this one particular boolean parameter called 'setWebContentsDebuggingEnabled' being set to false by default. 

# Solution
Hence this code solves the issue by enabling this parameter. It can injected in an app by using reverse engineering tools like 'frida'. Once done, URLs in any hybrid part of an app can be easily acquired by using Appium's 'get url method'.
