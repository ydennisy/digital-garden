---
id: b73caa67-93a4-4fef-bd84-6dd02778417a
title: Playwright
desc: ''
updated: 1611954740207
created: 1611954486115
---

# Playwright

## Debug in VSCode

A productive debugging approach is to use the node debugger within VS Code. To set this up, we first need to add the following `launch.json` file in a `.vscode` folder:

```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug Jest Tests",
      "type": "node",
      "request": "launch",
      "program": "${workspaceFolder}/node_modules/.bin/jest",
      "args": ["--runInBand"],
      "windows": {
        "program": "${workspaceFolder}/node_modules/jest/bin/jest"
      },
      "console": "integratedTerminal",
      "internalConsoleOptions": "neverOpen"
    }
  ]
}
```
We have called our launch configuration Debug Jest Tests and we are simply telling the node process to execute Jest. We can also change the config to run in `headless: false` mode:

```js
module.exports = {
  testEnvironmentOptions: {
    'jest-playwright': {
      browsers: ['chromium', 'firefox', 'webkit',
      launchOptions: {
        headless: false, // this is the change!
      },
    },
  },
};
```

You can now open the `Run` section in the left hand panel and execute your `jest` tests, setting breakpoints etc as you would in the browser console.

Voila!
