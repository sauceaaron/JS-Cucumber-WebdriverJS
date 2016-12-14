# JS-Cucumber-WebdriverJS

There are several packages available for working with Selenium in JavaScript .
The officially supported bindings are selenium-webdriver, also called WebDriverJS.

https://www.npmjs.com/package/selenium-webdriver
https://github.com/SeleniumHQ/selenium/wiki/WebDriverJs

## Install node.js

This framework uses Node.js to run tests with JavaScript.  You can download it from https://nodejs.org and install locally.

On Mac, you can also use homebrew

```
brew install nodejs
```

### NVM 

Alternately you can use NVM to install and manage multiple versions of node.js

https://github.com/creationix/nvm


## Dependencies


Install the dependencies using NPM.

```
npm install selenium-webdriver --save-dev
npm install cucumber --save-dev
```


## Sauce Labs credentials

To connect to Sauce labs you need to specify your username and access key.
For security, you should specify them as environment variables and not include them in your source code repository.

```
export SAUCE_USERNAME="YOUR_SAUCE_USERNAME"
export SAUCE_ACCESS_KEY="YOUR_SAUCE_ACCESS_KEY"
```

## Create a remote webdriver instance



SAUCE_URL="https://$SAUCE_USERNAME:$SAUCE_ACCESS_KEY@ondemand.saucelabs.com:80" 
\ cucumber.js
driver = 