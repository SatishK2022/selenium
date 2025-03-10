# Selenium
- Selenium is a powerful tool for controlling web browsers through programs and performing browser automation. It is functional for all browsers, works on all major OS and its scripts are written in various languages i.e Python, Java, C#, etc, we will be working with Python.

## Installation
- pip install selenium

## Selenium Commands
- driver.get("URL") : To open the URL
- driver.find_element_by_name("name") : To find the element by name
- driver.find_element_by_id("id") : To find the element by id
- driver.find_element_by_xpath("xpath") : To find the element by xpath
- driver.find_element_by_link_text("text") : To find the element by link text
- driver.find_element_by_partial_link_text("text") : To find the element by partial link text
- driver.find_element_by_tag_name("name") : To find the element by tag name
- driver.find_element_by_class_name("name") : To find the element by class name
- driver.find_element_by_css_selector("selector") : To find the element by css selector
- driver.close() : To close the current tab
- driver.quit() : To close the browser

## Example
```python
from selenium import webdriver

driver = webdriver.Chrome()
driver.get("https://www.google.com")
search_box = driver.find_element_by_name("q")
search_box.send_keys("Selenium")
search_box.submit()
```