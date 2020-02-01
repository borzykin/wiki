**Java**
* [Javax Gmail](https://github.com/borzykin/wiki/wiki/Javax-Mail-simple-guide)
* [Date/Time](https://github.com/borzykin/wiki/wiki/Date-Time)
* [Math round](https://github.com/borzykin/wiki/wiki/Math-Roundings)
* [Console UI (Switch)](https://github.com/borzykin/wiki/wiki/Console-UI-(Switch))
* [Read/Write Properties](https://github.com/borzykin/wiki/wiki/Read-Write-properties)
* [Java version, suiteXmlFile и Encoding](https://github.com/borzykin/wiki/wiki/Java-version,-suiteXmlFile-%D0%B8-Encoding)

**Automation**  
* [Appium setup Win10](https://github.com/borzykin/wiki/wiki/Setup-Appium-on-Win-10)
* [Appium Hello world](https://github.com/borzykin/wiki/wiki/Appium-%22Hello-world%22)
* [Rest Assured](https://github.com/borzykin/wiki/wiki/Rest-Assured-(Draft))
* [Enum for locators](https://github.com/borzykin/wiki/wiki/Enum-for-locators)
* [Stream filtering](https://github.com/borzykin/wiki/wiki/Filter-WebElemets-with-stream)
* [RestRail integration via testng listeners](https://github.com/borzykin/wiki/wiki/RestRail-integration-via-testng-listeners)
* [Custom Annotation to pass ID](https://github.com/borzykin/wiki/wiki/Custom-Annotation-to-pass-ID)
* [Cucumber Java](https://github.com/borzykin/wiki/wiki/Cucumber-Java-quick-guide)

**WebDriver**  
* [Basic setup](https://github.com/borzykin/wiki/wiki/Selenium-Basic-Setup)
* [BaseTest and DriverFactory](https://github.com/borzykin/wiki/wiki/BaseTest-and-DriverFactory)
* [PageObjects](https://github.com/borzykin/wiki/wiki/PageObjects)
* [Log4J](https://github.com/borzykin/wiki/wiki/Log4j)
* [Alerts Windows Frames](https://github.com/borzykin/wiki/wiki/Alerts---Windows---Frames)

Set to Array (Java 11):
Integer[] array = set.toArray(Integer[]::new);

Sort HashMap by value

    private Map<String, Double> sortByValue(final Map<String, Double> input) {
        return input.entrySet()
                .stream()
                .sorted((Map.Entry.<String, Double>comparingByValue().reversed()))
                .collect(Collectors.toMap(Map.Entry::getKey, Map.Entry::getValue, (e1, e2) -> e1, LinkedHashMap::new));
    }

Скриншоты
```Java
File tempFile = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
try {
  Files.copy(tempFile, new File("screen.png"));
} catch (IOException e) {
  e.printStackTrace();
}
```
