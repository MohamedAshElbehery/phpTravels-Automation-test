In this program Eclipse IDE was used, JUNIT was used to write run cases and Selenium web drivers was used for test automation.

The code consists of 2 classes:
1-signUpTests.java
2-signUpHelpers.java

signUpTests:
- consits of 8 tests to test the registering process of phptravels.com/register .
- every test calls the helping methods to generate random user data.
- chrome gets automated and the data fields gets filled.
- signup button is clicked and messages or current URL gets intercepted.

signUpHelpers:
consists of the helper methods,
- public static String generateString() : used to generate random names and passwords.
- public static String generateEmail()  : used to generate random emails.
- public static String generateNumber() : used to generate random mobile numbers.
- public static void takeSnapShot(WebDriver webdriver, String fileWithPath) : used to capture screenshots of faliures.

Data logging:
- performance logs (including signup API requests and responses) gets intercepted and saved in log.txt .
- screenshots for faliures are captured and saved in phpTravelsTest folder.
- The code creates a report after every test, it opens automatically after all the test are done.

Limitations:
- the code only works for chrome browser.
