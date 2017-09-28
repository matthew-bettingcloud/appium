# Set Timeouts

Configure the amount of time that a particular type of operation can execute for before they are aborted
## Example Usage

```java
// Java
driver.manage().timeouts().pageLoadTimeout(30, TimeUnit.SECONDS);

```

```python
# Python
self.driver.set_page_load_timeout(5000)

```

```javascript
// Javascript
// webdriver.io example
driver.timeouts('pageLoad', 5000)


// wd example
await driver.setPageLoadTimeout(5000);

```

```ruby
# Ruby
@driver.page_load(5) # Ruby translates it to seconds

```

```php
# PHP
// TODO PHP sample

```

```csharp
// C#
// TODO C# sample

```


## Description

The types of timeouts are 'page load', ['script'](/docs/en/commands/session/async-script.md) and ['implicit'](/docs/en/commands/session/implicit.md). (The example usage is just 'page load')


## Client Docs

 * [Java](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/remote/RemoteWebDriver.RemoteWebDriverOptions.RemoteTimeouts.html#pageLoadTimeout-long-java.util.concurrent.TimeUnit-) 
 * [Python](http://selenium-python.readthedocs.io/api.html#selenium.webdriver.remote.webdriver.WebDriver.set_page_load_timeout) 
 * [Javascript (WebdriverIO)](http://webdriver.io/guide/testrunner/timeouts.html#Selenium-timeouts) 
 * [Javascript (WD)](https://github.com/admc/wd/blob/master/lib/commands.js#L714) 
 * [Ruby](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/Timeouts:page_load=) 
 * [PHP](https://github.com/appium/php-client/) 
 * [C#](https://github.com/appium/appium-dotnet-driver/) 

## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients 

|Language|Support|
|--------|-------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |
|[Python](https://github.com/appium/python-client/releases/latest)| All |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |

## HTTP API Specifications

### Endpoint

`POST /session/:session_id/timeouts`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|

### JSON Parameters

|name|type|description|
|----|----|-----------|
| type | string | The type of operation to set the timeout for. Valid values are: 'script' for script timeouts, 'implicit' for modifying the implicit wait timeout and 'page load' for setting a page load timeout. |
| ms | number | The amount of time, in milliseconds, that time-limited commands are permitted to run |

### Response

null

## See Also

* [W3C Specification](https://www.w3.org/TR/webdriver/#set-timeouts)
* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#sessionsessionidtimeouts)