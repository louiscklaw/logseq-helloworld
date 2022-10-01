- ### Purpose:
	- to test mobile apps of hk observatory
	  environment:
	- linux
	- appium
	- python 3.6.1, behave, python-appium-client
-
- ### To setup:
- ```
  $ pip
  ```
### to execute:

```
$ virtualenv venv
$ source venv/bin/activate
```
### install python libraries:
- ```
  $ pip install -r requirements.txt
  ```
- start appium -> connect to android / genymotion appium:
- ```
  $ python behave
  $ behave ./features/HKOApp_9DayForecast.feature
  ```