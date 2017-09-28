# Click

Double-clicks at the current mouse coordinates (set by moveto).
## Example Usage

```java
// Java
Actions action = new Actions(driver);
action.moveTo(element);
action.doubleClick();
action.perform();

```

```python
# Python
actions = ActionChains(driver)
actions.move_to_element(element)
actions.double_click()
actions.perform()

```

```javascript
// Javascript
// webdriver.io example
driver.moveTo(element)
  .doubleClick();


// wd example
await driver.moveTo(element);
await driver.doubleclick();

```

```ruby
# Ruby
@driver.action.move_to(element).double_click.perform

```

```php
# PHP
// TODO PHP sample

```

```csharp
// C#
// TODO C# sample

```



## Client Docs

 * [Java](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/interactions/Actions.html#doubleClick--) 
 * [Python](http://selenium-python.readthedocs.io/api.html#selenium.webdriver.common.action_chains.ActionChains.double_click) 
 * [Javascript (WebdriverIO)](http://webdriver.io/api/action/doubleClick.html) 
 * [Javascript (WD)](https://github.com/admc/wd/blob/master/lib/commands.js#L1686) 
 * [Ruby](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/ActionBuilder:double_click) 
 * [PHP](https://github.com/appium/php-client/) 
 * [C#](https://github.com/appium/appium-dotnet-driver/) 

## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | None | None | None |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | None | None | None |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | None | None | None |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | None | None | None |
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

`POST /session/:session_id/doubledoubleClick`

### URL Parameters

None

### JSON Parameters

None

### Response

null

## See Also

* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#sessionsessioniddoubledoubleClick)