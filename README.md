# framework_design

**Note:-**
First we need to create a object for the class after that we can access the methods using reference variable.
CommonMethods cm=new CommonMethods();

Here's the README file content:

---

# CommonMethods Class

The `CommonMethods` class provides a collection of methods commonly used in Selenium WebDriver automation. These methods are designed to facilitate interaction with web elements, manage browser windows, handle alerts, and perform various other tasks in web testing.

## Method List:

### Navigation:
1. `navigateToUrl(WebDriver driver, String url)`
    - Navigates the browser to the specified URL.

### Retrieving Information:
2. `getTitlePage(WebDriver driver)`
    - Returns the title of the current web page.

### Element Interaction:
3. `clickElement(WebDriver driver, WebElement element)`
    - Clicks on the given web element.
4. `sendKeysToElement(WebElement element, CharSequence... keys)`
    - Sends keys to a single web element.
5. `sendKeysToElements(Map<WebElement, CharSequence> elementTextMap)`
    - Sends keys to multiple web elements.
6. `getElementText(WebElement ele)`
    - Retrieves the text of the specified web element.
7. `getElementAttribute(WebElement element, String attributeName)`
    - Retrieves the value of the specified attribute of a web element.
8. `isElementPresent(WebElement ele)`
    - Checks if the web element is present on the page.
9. `scrollToElement(WebDriver driver, WebElement ele)`
    - Scrolls the page to bring the specified web element into view.
10. `selectDropdownByVisibleText(WebElement ele, String visibleText)`
    - Selects an option from a dropdown by visible text.
11. `selectDropDownByValue(WebElement ele, String value)`
    - Selects an option from a dropdown by value.
12. `selectDropDownByIndex(WebElement ele, int index)`
    - Selects an option from a dropdown by index.
13. `isElementDisplayed(WebElement ele)`
    - Checks if the web element is displayed.
14. `isElementEnabled(WebElement ele)`
    - Checks if the web element is enabled.
15. `isElementSelected(WebElement ele)`
    - Checks if the web element is selected.
16. `clearAndSendKeysToElement(Map<WebElement, CharSequence> elementTextMap)`
    - Clears the text from multiple web elements and sends keys.
17. `getNumberOfElements(List<WebElement> ele)`
    - Returns the number of web elements in a list.

### Dropdown Handling:
18. `deselectAllOptions(WebElement ele)`
    - Deselects all options from a dropdown.

### Frame and Window Handling:
19. `switchToDefaultContent(WebDriver driver)`
    - Switches to the default content of the web page.
20. `switchToFrame(WebElement ele, WebDriver driver)`
    - Switches to a frame within the web page.
21. `switchToWindowAtIndex(WebDriver driver, int index)`
    - Switches to a window by its index.
22. `maximizeWindow(WebDriver driver)`
    - Maximizes the browser window.
23. `minimizeWindow(WebDriver driver)`
    - Minimizes the browser window.
24. `enterFullscreenMode(WebDriver driver)`
    - Puts the browser window into fullscreen mode.
25. `switchToWindowHandle(WebDriver driver, String windowHandle)`
    - Switches to a window by its handle.
26. `switchToFrameByIndex(WebDriver driver, int index)`
    - Switches to a frame by its index.
27. `switchToFrameByNameOrId(WebDriver driver, String nameOrId)`
    - Switches to a frame by its name or ID.
28. `switchToFrameByElement(WebDriver driver, WebElement frameElement)`
    - Switches to a frame using a WebElement representing the frame.

### Other Actions:
29. `takeScreenshot(WebDriver driver, String fileName)`
    - Takes a screenshot of the current web page.
30. `openNewTabAndSwitchToIt(WebDriver driver)`
    - Opens a new tab and switches to it.
31. `openNewWindowAndSwitchToIt(WebDriver driver)`
    - Opens a new window and switches to it.
32. `switchToOriginalWindow(WebDriver driver, String originalWindowHandle)`
    - Switches back to the original window.

### Alert Handling:
33. `acceptAlert(WebDriver driver)`
    - Accepts an alert dialog.
34. `dismissAlert(WebDriver driver)`
    - Dismisses an alert dialog.
35. `getAlertText(WebDriver driver)`
    - Retrieves the text of an alert dialog.
36. `sendKeysToAlert(WebDriver driver, String keys)`
    - Sends keys to an alert dialog.

### Miscellaneous:
37. `getElementTagName(WebElement element)`
    - Retrieves the tag name of a web element.
38. `getElementCssValue(WebElement element, String propertyName)`
    - Retrieves the CSS value of a specified property of a web element.
39. `getTotalNumberOfWindows(WebDriver driver)`
    - Returns the total number of open windows.
40. `getAllOptions(WebElement dropdownElement)`
    - Returns a list of all options in a dropdown.
41. `getFirstSelectedOption(WebElement dropdownElement)`
    - Returns the text of the first selected option in a dropdown.
42. `getAllSelectedOptions(WebElement dropdownElement)`
    - Returns a list of all selected options in a dropdown.

---

## Abstract Method List:

1. `navigateToUrl(WebDriver driver, String url)`
2. `getTitlePage(WebDriver driver)`
3. `clickElement(WebDriver driver, WebElement element)`
4. `sendKeysToElement(WebElement element, CharSequence... keys)`
5. `sendKeysToElements(Map<WebElement, CharSequence> elementTextMap)`
6. `getElementText(WebElement ele)`
7. `getElementAttribute(WebElement element, String attributeName)`
8. `isElementPresent(WebElement ele)`
9. `scrollToElement(WebDriver driver, WebElement ele)`
10. `selectDropdownByVisibleText(WebElement ele, String visibleText)`
11. `selectDropDownByValue(WebElement ele, String value)`
12. `selectDropDownByIndex(WebElement ele, int index)`
13. `isElementDisplayed(WebElement ele)`
14. `isElementEnabled(WebElement ele)`
15. `isElementSelected(WebElement ele)`
16. `clearAndSendKeysToElement(Map<WebElement, CharSequence> elementTextMap)`
17. `getNumberOfElements(List<WebElement> ele)`
18. `deselectAllOptions(WebElement ele)`
19. `switchToDefaultContent(WebDriver driver)`
20. `switchToFrame(WebElement ele, WebDriver driver)`
21. `switchToWindowAtIndex(WebDriver driver, int index)`
22. `maximizeWindow(WebDriver driver)`
23. `minimizeWindow(WebDriver driver)`
24. `enterFullscreenMode(WebDriver driver)`
25. `switchToWindowHandle(WebDriver driver, String windowHandle)`
26. `switchToFrameByIndex(WebDriver driver, int index)`
27. `switchToFrameByNameOrId(WebDriver driver, String nameOrId)`
28. `switchToFrameByElement(WebDriver driver, WebElement frameElement)`
29. `takeScreenshot(WebDriver driver, String fileName)`
30. `openNewTabAndSwitchToIt(WebDriver driver)`
31. `openNewWindowAndSwitchToIt(WebDriver driver)`
32. `switchToOriginalWindow(WebDriver driver, String originalWindowHandle)`
33. `acceptAlert(WebDriver driver)`
34. `dismissAlert(WebDriver driver)`
35. `getAlertText(WebDriver driver)`
36. `sendKeysToAlert(WebDriver driver, String keys)`
37. `getElementTagName(WebElement element)`
38. `getElement

CssValue(WebElement element, String propertyName)`
39. `getTotalNumberOfWindows(WebDriver driver)`
40. `getAllOptions(WebElement dropdownElement)`
41. `getFirstSelectedOption(WebElement dropdownElement)`
42. `getAllSelectedOptions(WebElement dropdownElement)`

---

This README file provides a comprehensive overview of the `CommonMethods` class and its methods. It also includes a list of abstract method names for reference.

Feel free to modify the content as needed for your project documentation.

