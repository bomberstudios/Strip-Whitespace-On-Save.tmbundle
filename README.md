# Strip Whitespace On Save

TextMate 2 bundle: Strips trailing whitespace from current document when saving. Works nicely with my [Save On Focus Lost bundle](https://github.com/bomberstudios/Save-On-Focus-Lost.tmbundle). If you need whitespace highlighting, check the superb [Whitespace bundle by Mads Hartmann](http://mads379.github.com/posts/whitespace-tmbundle).

## Installation

- Clone the git repo to  `~/Library/Application Support/TextMate/Managed/Bundles`
- Relaunch TextMate 2

## Notes

**You need to be using at least TextMate version 2.0.0-alpha.9317**. Open Preferences » Software Update and **ALT-click the "Check Now"** button to get the most recent nightly build (this will grab a latest version than the one you get by just clicking the button).

**Caret position will be lost after saving**. This is a limitation of the current implementation of `callback.document.will-save` and hopefully will be fixed Really Soon Now™.

Enjoy it!
