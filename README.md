# google-LLC-calculator-app-automation-using-selenium-and-appium

### Testcases
1. Sum any of 2 numbers (9+5=14)
2. Subtraction any of 2 numbers (8-3=5)
3. Do multiply of Result of Sum and Subtraction (14*5=70)
4. Divide the result of multiplication with 10 (70/10=7)
5. Solve this series (100+200-100*2/5)

### How I done this project
- Downloaded google LLC calculator for android
- put it in d drive
- Opened Android studio
- Opened emulator 
- Opened APK file
- Played the emulator
- Put ```adb devices``` this command on cmd to ensure emulator device is working or not
- Put ```appium -p 4723``` this command on cmd to open appium server
- Opened Appium inspector
- Set desired capabilites in json format: <br>
{  <br>
  "appium:deviceName": "emulator",  <br>
  "appium:uuid": "emulator-5554",  <br>
  "platformName": "Android",  <br>
  "appium:platfromVersion": "11",  <br>
  "appium:appPackage": "com.google.android.calculator",  <br>
  "appium:appActivity": "com.android.calculator2.Calculator",  <br>
  "appium:app": "D:\\APK\\calculator.apk"  <br>
  }  <br>
  
  - Ensured the connectivity between emulator and appium inspector
  - Opened Intellij Idea
  - do the expected tests in calculator
  -  Put ```gradle clean test``` this command in the terminal to see the test result
  - Put ```allure generate allure-results --clean -o allure-report``` and ```allure serve allure-results``` commands to generate reports
  
  
  
