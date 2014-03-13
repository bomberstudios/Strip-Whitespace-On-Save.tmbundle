# Strip Whitespace On Save

TextMate 2 bundle: Strips trailing whitespace from current document when saving. Works nicely with my [Save On Focus Lost bundle](https://github.com/bomberstudios/Save-On-Focus-Lost.tmbundle). If you need whitespace highlighting, check the superb [Whitespace bundle by Mads Hartmann](http://mads379.github.com/posts/whitespace-tmbundle). If you happen to need new lines at EOF, then check Mike Szyndel's [Ensure New Line at the EOF bundle](https://github.com/hajder/Ensure-New-Line-at-the-EOF.tmbundle), which is based on mine.

## Installation

- Clone the git repo to  `~/Library/Application Support/Avian/Bundles`
- Relaunch TextMate 2

## Strip Whitespace on specific filetypes

If you want the bundle to affect some filetypes only, it's easy.

Say you want to avoid stripping white space on CSV files.

Just open the bundle editor (Bundles menu › Edit Bundles... or pressing Ctrl + Alt + Command + B) and add `-text.tabular.csv` in the Scope Selector field of the command (see attached screenshot : )

![screenshot 2013-12-05 20 35 46](https://f.cloud.github.com/assets/3832/1686305/20f9cb7e-5de5-11e3-8b76-1c09d9e40137.png)

If you need to exclude multiple file types, just add `(space)-scope.namespace`. For example, if you want to exclude CSV and YAML, you'd write: `-text.tabular.csv -source.yaml`.

If you want the bundle to work only on specific file types, use the namespace only, without the minus sign (i.e: if you want to strip CSV files only, you'd write `text.tabular.csv`). If you need to include multiple file types just add them separated by comma (i.e: `text.tabular.csv, source.yaml, text.html.markdown`).

If you want to know which scope corresponds to each language, just hit Ctrl + Shift + P ('Show Scope' command) on a document of that type, and you'll get a nice tooltip with the scope namespaces that apply at the current cursor's position.


## Notes

**You need to be using at least TextMate version 2.0.0-alpha.9317**. Open Preferences » Software Update and **ALT-click the "Check Now"** button to get the most recent nightly build (this will grab a latest version than the one you get by just clicking the button).

Enjoy it!
