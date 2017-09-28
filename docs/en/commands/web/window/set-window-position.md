# Set Window Position

Change the position of the specified window (Web context only)
## Example Usage

```java
// Java
driver.manage().window().setPosition(new Dimension(10, 10));

```

```python
# Python
self.driver.set_window_position(10, 10)

```

```javascript
// Javascript
// webdriver.io example
driver.windowHandlePosition("handleName", {x: 10, y: 10}); // Set by window handle hame
driver.windowHandlePosition({x: 10, y: 10}); // Current window



// wd example
await driver.setWindowPosition(10, 10, "handleName"); // Set position of window by handle name
await driver.setWindowPosition(10, 10); // Set current window

```

```ruby
# Ruby
@driver.reposition_window(10, 10)

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

 * [Java](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/WebDriver.Window.html#setPosition-org.openqa.selenium.Point-) 
 * [Python](http://selenium-python.readthedocs.io/api.html#selenium.webdriver.remote.webdriver.WebDriver.set_window_position) 
 * [Javascript (WebdriverIO)](http://webdriver.io/api/protocol/windowHandlePosition.html) 
 * [Javascript (WD)](https://github.com/admc/wd/blob/master/lib/commands.js#L604) 
 * [Ruby](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/Remote/W3C/Bridge:reposition_window) 
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
| Mac | [Mac](/docs/en/drivers/mac.md) | None | None | None |
| Windows | [Windows](/docs/en/drivers/windows.md) | None | None | None |

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

`POST /wd/hub/session/:session_id/window/:window_handle/position`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|
|window_handle|Handle of the window to get position of. If 'current' it will get position of current window.|

### JSON Parameters

|name|type|description|
|----|----|-----------|
| x | number | The x coordinate relative to the top left corner of the window |
| y | number | The y coordinate relative to the top left corner of the window |

### Response

null

## See Also

* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#post-sessionsessionidwindowwindowhandleposition)