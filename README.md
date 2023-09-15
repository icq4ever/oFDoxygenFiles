# about
with doxygen, can generate offline documentation for [Dash](https://kapeli.com/dash) / [Zeal](http://zealdocs.org/) / [Velocity](http://velocity.silverlakesoftware.com/)

# generate documentation on MacOS
## preRequirements
### [docsetutil](https://github.com/SwiftDocOrg/DocSetUtil)
since Xcode 9.3, docsetutil is removed. so install thatone from the unofficial mirror, with [homebrew](http://brew.sh)
```
brew install swiftdocorg/formulae/docsetutil
```

## generate documentation
1. run `doxygen` in `_OF_DIR_.libs/openFrameworksCompiled/project/doxygen/`
2. copy `icon.png` into `build/html/openFrameworks.docset/`
   1. you can open as right click of `openFrameworks.docset` -> `Show Package Contents` with finder
3. copy `fonts` directory into `build/html/openFrameworks.docset/Contents/Resources/Documentation/`
4. copy `Info.plist` into `openFrameworks.docset/Contents/Info.plist` (overwrite)
5. open `openFrameworks.docset` and test with Dash app.
