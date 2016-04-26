# Mocha
Runs Mocha tests, all or selected. Then prints the result to an output window.

![Demo showing Mocha test result](https://raw.githubusercontent.com/compulim/vscode-mocha/master/demo.png)

## Usage
To run Mocha tests:
* Bring up Command Palette (`F1`, or `Ctrl+Shift+P` on Windows and Linux, or `Shift+CMD+P` on OSX)
* Type or select "Mocha: Run all tests"

You can also create keyboard shortcut with JSON below.
```
{
  "key": "ctrl+k r",
  "command": "mocha.runAllTests"
}
```

## How it works
This extensions finds and runs all test at `test/**/*.js`.

All tests will run under installed Node.js as indicated by environmental variable `PATH`.

## Configure Mocha
To configure Mocha, you can set it under File > Preferences > Workspace Settings. For example, the following JSON will set your Mocha to run in TDD mode.
```
{
  "mocha.options": {
    "ui": "tdd"
  }
}
```

## Commands

| Command | Title |
|---------|-------------|
| `mocha.runAllTests` | Mocha: Run all tests |
| `mocha.runFailedTests` | Mocha: Run failed tests |
| `mocha.runLastSetAgain` | Mocha: Run last set again |
| `mocha.runTestsByPattern` | Mocha: Run tests matching a pattern |
| `mocha.selectAndRunTest` | Mocha: Select and run a test |

## Change log
* 0.1.0 (2016-04-26)
  * Feature: Run tests by grep pattern
  * Feature: Rerun failed tests
  * Feature: Rerun last set of tests
  * Feature: Dump severe error to output channel
  * Fix: When selecting tests, it did not use Mocha options in workspace settings
* 0.0.1 (2016-04-25)
  * First public release

## Contributions
Love this extension? [Star](https://github.com/compulim/vscode-mocha/stargazers) us!

Want to make this extension even more awesome? [Send us your wish](https://github.com/compulim/vscode-mocha/issues/new/).

Hate how it is working? [File an issue](https://github.com/compulim/vscode-mocha/issues/new/) to us.
