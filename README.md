# Kwick Browser
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/01ce263113c6405fa5e2b643d8fde0e2)](https://www.codacy.com/gh/CyberSafe-Labs/Kwick-Browser/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CyberSafe-Labs/Kwick-Browser&amp;utm_campaign=Badge_Grade)
<br>
<br>
A private fast open source browser project based on Min Browser
<br>
<br>
Disclaimer: Redistribution and use in source and binary forms, with or without
modification,are not permitted.
Commercial license is available for free at www.cybersafe.ezyro.com/license/
<br>
<br>
Support:
kwickbrowser@cybersafe.ezyro.com
<br>
<br>
# Developing
If you want to develop Kwick:

- First Obtain A <a href="www.cybersafe.ezyro.com/license">Commercial License</a>
- Install [Node](https://nodejs.org).
- Run `npm install` to install dependencies.
- Start Min in development mode by running `npm run start`.
- After you make changes, you can press `ctrl+r` twice to restart the browser.
<br>
In order to build Kwick from source, follow the installation instructions above, then use the following command to create binaries:

- `npm run buildWindows`

Depending on the platform you are building on, you may need to install additional dependencies:

- To build on Windows, you'll need to install Visual Studio. Once it's installed, you may also need to run `npm config set msvs_version 2019` (or the appropriate version).

<br>
### Contributing Translations

### Adding a new language

- Find the language code that goes with your language from [this list](https://electron.atom.io/docs/api/locales/#locales).
- In the `localization/languages` directory, create a new file, and name it "[your language code].json".
- Open your new file, and copy the contents of the <a href="https://github.com/CyberSafe-Labs/Kwick-Browser/blob/master/localization/languages/en-US.json">localization/languages/en-US.json</a> file into your new file.
- Change the "identifier" field in the new file to the language code from step 1.
- Inside the file, replace each English string in the right-hand column with the equivalent translation.
- (Optional) See your translations live by following the [development instructions](#installing) above. Kwick will display in the same language as your operating system, so make sure your computer is set to the same language that you're translating.
- That's it! Make a pull request with your changes.

#### Updating an existing language

- Find the language file for your language in the `localization/languages` directory.
- Look through the file for any items that have a value of "null", or that have a comment saying "missing translation".
- For each of these items, look for the item with the same name in the `en-US.json` file.
- Translate the value from the English file, replace "null" with your translation, and remove the "missing translation" comment.
- Make a pull request with the updated file.

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCyberSafe-Labs%2FKwick-Browser.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FCyberSafe-Labs%2FKwick-Browser?ref=badge_large)
