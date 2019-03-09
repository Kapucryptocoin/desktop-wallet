# Kapu Desktop Wallet

![KAPU-DESKTOP](https://i.imgur.com/sYopmfR.jpg)

[![Build Status](https://badgen.now.sh/circleci/github/Kapucryptocoin/desktop-wallet)](https://circleci.com/gh/Kapucryptocoin/desktop-wallet)
[![Latest Version](https://badgen.now.sh/github/release/Kapucryptocoin/desktop-wallet)](https://github.com/Kapucryptocoin/desktop-wallet/releases)
[![License: MIT](https://badgen.now.sh/badge/license/MIT/green)](https://opensource.org/licenses/MIT)

## Download
[Latest Release](https://github.com/kapucryptocoin/desktop-wallet/releases)


## Translations

Translations are part of our [ARK Development and Security Bounty Program](https://blog.ark.io/ark-development-and-security-bounty-program-a95122d06879).

Full translations are considered to be `Tier 3`, while grammar fixes, typos, etc. are considered to be `Tier 6`.

<details><summary>Full translations should involve 5 tasks</summary>

 - Create a pull request for the language you are going to translate. If you have doubts about something, use English to explain them.
 - Translate the textual content of the application, using the [English language file](https://github.com/Kapucryptocoin/desktop-wallet/blob/develop/src/renderer/i18n/locales/en-US.js) as the reference. To do that, a new file, with the language locale code should be created. The name of the file should be a valid [RFC 5646](https://tools.ietf.org/html/rfc5646).
 - Add the language to the [English language file](https://github.com/Kapucryptocoin/desktop-wallet/blob/develop/src/renderer/i18n/locales/en-US.js) at the `LANGUAGES` key.
 - Update the [date and time formats file](https://github.com/Kapucryptocoin/desktop-wallet/blob/develop/src/renderer/i18n/date-time-formats.js) to include the short and long format that are used commonly by native speakers.
 - Update the [number formats file](https://github.com/Kapucryptocoin/desktop-wallet/blob/develop/src/renderer/i18n/number-formats.js) to include the preferred way of displaying currencies used commonly by native speakers.
 - Add the language at the `I18N.enabledLocales` array at the [main configuration file](https://github.com/Kapucryptocoin/desktop-wallet/blob/develop/config/index.js). This step is necessary to make the language would not be available.
 - Execute the application. Go to the [ development section](https://github.com/Kapucryptocoin/desktop-wallet#development) to learn how to install the requirements and execute it.

</details>

## Development

### Requirements

#### Ubuntu
In Ubuntu the development files of `libudev` are necessary:
```
sudo apt-get install libudev-dev libusb-1.0-0-dev
```

#### Windows
- Python 2.7
- Visual Studio 2017

#### Node 9
There are certain packages (such as the ledger HID packages) which do not work on Node 10.

To download Node 9, head over to [here](https://nodejs.org/en/blog/release/v9.11.1/)

#### Yarn
Install the Yarn dependency manager
```
npm install -g yarn
```

### Commands

<details><summary>List of commands</summary>

``` bash
# Install dependencies
yarn install

# Execute the application. Making changes in the code, updates the application (hot reloading).
yarn dev

# Lint all JS/Vue files in the `src` and `__tests__`
yarn lint

# Lint, and fix, all JS/Vue files in `src` and `__tests__`
yarn lint:fix

# Check that all dependencies are used
yarn depcheck

# Collect the code and produce a compressed file
yarn pack

# Build electron application for production (Current OS)
yarn build

# Build electron application for production (Windows)
yarn build:win

# Build electron application for production (Mac)
yarn build:mac

# Build electron application for production (Linux)
yarn build:linux

# Run unit and end-to-end tests
yarn test

# Run unit tests
yarn test:unit

# Run unit tests and generate and display the coverage report
yarn test:unit:coverage

# Run unit tests and watch for changes to re-run the tests
yarn test:unit:watch

# Run end-to-end tests, without building the application
yarn test:e2e

# Build the application and run end-to-end tests
yarn test:e2e:full
```

</details>

## Security

If you discover a security vulnerability within this project, please send an e-mail to security@ark.io. All security vulnerabilities will be promptly addressed.

## Credits

 - [Alex Barnsley](https://github.com/alexbarnsley)
 - [ItsANameToo](https://github.com/ItsANameToo)
 - [Juan A. Martín](https://github.com/j-a-m-l)
 - [Lúcio Rubens](https://github.com/luciorubeens)
 - [Mario Vega](https://github.com/mvega3)
 - [All Contributors](../../contributors)

## License

[MIT](LICENSE) © [Kapucoin](https://kapu.one)
