# Dark Mode for Outlook™ [Extension]
![](https://img.shields.io/badge/type-Extension-yellow.svg "Project type")
[![](https://img.shields.io/chrome-web-store/v/kjfbefcenipnnpbcbbklcidpjiamlcpl.svg "View on the Chrome Web Store")][chrome_link]
[![](https://img.shields.io/amo/v/dark-mode-for-outlook.svg "View on the Firefox Add-ons Page")][firefox_link]
[![](https://img.shields.io/badge/dynamic/json?label=edge%20add-on&prefix=v&query=%24.version&url=https%3A%2F%2Fmicrosoftedge.microsoft.com%2Faddons%2Fgetproductdetailsbycrxid%2Fncmfoiokkfipenppipihehpoikhacpep "View on the Edge Add-ons Page")][edge_link]
[![](https://img.shields.io/badge/dynamic/json?label=opera%20add-on&color=blue&query=%24.tag_name&url=https%3A%2F%2Fapi.github.com%2Frepos%2Fjerboa88%2Fdark-mode-for-outlook%2Freleases%2Flatest "View on the Opera Add-ons Page")][opera_link]
![](https://img.shields.io/github/repo-size/jerboa88/dark-mode-for-outlook.svg "Repository size")
[![](https://img.shields.io/github/license/jerboa88/dark-mode-for-outlook.svg "Project license")](LICENSE.md)


A browser extension/add-on that applies a better (unofficial) dark mode to Microsoft Outlook and removes the ad sidebar. Available for Chrome, Firefox, Edge, and Opera, and compatible with Firefox mobile!


## Installation
### Simple
The extension can be installed for your browser here:
| [![Chrome logo][chrome_logo]][chrome_link] | **[Chrome][chrome_link]** |
| - | - |
| [![Firefox logo][firefox_logo]][firefox_link] | **[Firefox][firefox_link]** |
| [![Edge logo][edge_logo]][edge_link] | **[Edge][edge_link]** |
| [![Opera logo][opera_logo]][opera_link] | **[Opera][opera_link]** |

**Notes:**
- It can also be installed on [Brave](https://support.brave.com/hc/en-us/articles/360017909112-How-can-I-add-extensions-to-Brave-), [Vivaldi](https://help.vivaldi.com/article/extensions/#install), and other Chromium-based browsers from the Chrome Web Store (or by sideloading).
- Installing add-ons for Firefox mobile is complicated at the moment, since Android's [new Geckoview-based browser](https://blog.mozilla.org/addons/2020/09/02/update-on-extension-support-in-the-new-firefox-for-android/) does not officially support all add-ons yet. If you still want to use this add-on on Firefox mobile, refer to [this page](https://support.mozilla.org/en-US/kb/find-and-install-add-ons-firefox-android#w_expanded-extension-support-in-firefox-for-android-nightly) for more information.


### Advanced
If you wish to build yourself, you can download the repository, run `npm install` to install dependencies, and build the project with `npm start`. Make sure you have npm and Node.js v10.0.0 or greater installed ([how?](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)). At the moment, Linux is required to run the build script, although you can perform all the steps in that script manually if you want to build on another OS.

Next, the build directory or zip file can be loaded into your browser of choice: [Chrome](https://developer.chrome.com/extensions/getstarted#manifest) / [Firefox](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/) / [Edge](https://docs.microsoft.com/en-us/microsoft-edge/extensions-chromium/getting-started/part1-simple-extension#run-your-extension-locally-in-your-browser-while-developing-it-side-loading) / [Opera](https://dev.opera.com/extensions/testing/)


## Usage
Just install the extension and you should be good to go! The extension does not have any other settings at the moment.

If you encounter any problems while using the extension, please create an issue [here](/issues), send me an email at extensions@johng.io, or create a pull request yourself to fix the issue.

I try to fix the extension as soon as possible when Outlook makes breaking changes, but keep in mind it may take some time for me to fit the work into my schedule and make all the changes that need to be made. Thanks for your patience :).


## Screenshots
Desktop site | &#8291;
:-:|:-:
![Screenshot 1](screenshots/desktop_mail.png) | ![Screenshot 2](screenshots/desktop_sidebar.png)
![Screenshot 3](screenshots/desktop_viewmessage.png) | ![Screenshot 4](screenshots/desktop_newmessage.png)

Mobile site | &#8291; | &#8291; | &#8291;
:-:|:-:|:-:|:-:
![Screenshot 1](screenshots/mobile_mail.png) | ![Screenshot 2](screenshots/mobile_sidebar.png) | ![Screenshot 3](screenshots/mobile_viewmessage.png) | ![Screenshot 4](screenshots/mobile_newmessage.png)


## Contributing
Contributions, issues, and forks are welcome. Please note that any code you contribute will be licensed under the same license as this project. By making any contributions, you agree to this.

**Guidelines:**
- SCSS is used to make writing styles easier and more maintainable. Please take advantage of its features
- Variables are defined in [_vars.scss](styles/_vars.scss) and should be used whenever possible instead of hardcoding values
- Any styles written should be specific enough to not affect unintended areas of the application, but not overly specific such that styles are broken every time Outlook releases an update (do not use Outlook's randomly generated class names)
- Styles should be as short as possible, and written in relation to other elements with hardcoded attributes. See [main.scss](styles/main.scss) for examples

[SemVer](http://semver.org/) is used for versioning this project, although the patch number is left out.


## License
This project is licensed under the MIT License. See [LICENSE.md](LICENSE.md) for details. Outlook is a trademark of Microsoft and this project is not affiliated with or endorsed by Microsoft in any way.


[chrome_link]: https://chrome.google.com/webstore/detail/dark-mode-for-outlook/kjfbefcenipnnpbcbbklcidpjiamlcpl
[firefox_link]: https://addons.mozilla.org/en-US/firefox/addon/dark-mode-for-outlook/
[edge_link]: https://microsoftedge.microsoft.com/addons/detail/ncmfoiokkfipenppipihehpoikhacpep
[opera_link]: https://addons.opera.com/en/extensions/details/dark-mode-for-outlook/

[chrome_logo]: https://cdnjs.cloudflare.com/ajax/libs/browser-logos/69.0.0/chrome/chrome_32x32.png
[firefox_logo]: https://cdnjs.cloudflare.com/ajax/libs/browser-logos/69.0.0/archive/firefox_57-70/firefox_57-70_32x32.png
[edge_logo]: https://cdnjs.cloudflare.com/ajax/libs/browser-logos/69.0.0/edge/edge_32x32.png
[opera_logo]: https://cdnjs.cloudflare.com/ajax/libs/browser-logos/69.0.0/opera/opera_32x32.png
