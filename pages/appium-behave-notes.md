- #appium-playlist #docker #android #testing
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
### stack on MAC machine:

```
brew cask install visual-studio-code
brew install zsh-history-substring-search
brew install zsh
brew install zsh-lovers
brew install zsh-autosuggestions
brew install zsh-navigation-tools
brew install zsh-completions
brew install zsh-syntax-highlighting
brew install zsh-git-prompt
brew install zshdb
brew install git-flow
```
-
- ### pass example
- {{video https://www.youtube.com/watch?v=Ce-v1zTHhwU}}
-
- ### fail example
- {{video https://www.youtube.com/watch?v=uR8VLSwvf9Q}}
-
- ### resources:
	- https://github.com/louiscklaw/appium-python-client
	- https://github.com/louiscklaw/casetify-website-testing-tryout
	-
	-