JS Lint? _Check._  
Unit tests? _Check._  
Documentation? _Umm..._  

Don't worry -- documenting your JavaScript can be fun and easy! (Well, maybe just easy.)
 
This bundle provides tools for running and writing comments with [JsDoc Toolkit][jsdoc] directly from TextMate. JsDoc Toolkit is a great application for automatically generating documentation from commented JavaScript source code.

## Installation

Install from Github:

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles
    cd ~/Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/csaccheri/JsDoc-Toolkit.tmbundle.git "JsDoc Toolkit.tmbundle"
    osascript -e 'tell app "TextMate" to reload bundles'

Or use [GetBundles][getb] (search for "JsDoc Toolkit").

**Important!** You must have Java installed to run JsDoc Toolkit.

## Usage

### Snippets

This bundle includes a number of snippets to help you write JsDoc Toolkit-friendly comments. Use the `docblock` snippet (type `doc` then tab) to create a documentation comment block (starting with `/**`), then use the other snippets to generate the various tags JsDoc Toolkit supports.

Read the [JsDoc Toolkit tag reference][jsdot] for a description of each tag and how it's used.

### Commands

* **Document with JsDoc Toolkit** (⌃⌘J)
Generates HTML documentation from commented JavaScript source code using JsDoc Toolkit 2.4.0 and displays it in TextMate's Web Preview window. You can generate documentation from a single file, multiple selected files, or an entire directory.  
You can find the generated documentation in  
`~/Library/Application Support/TextMate/Bundles/JsDoc Toolkit.tmbundle/Support/bin/jsdoc-tookit/out`

* **Edit JsDoc Toolkit Configuration** (⌃⌘J)
Opens the configuration file used by the bundle to run JsDoc Toolkit. You can edit this file to change configuration options, such as whether to show private methods, use a different output template, etc. See [JsDoc Toolkit command line options][jsdop] for more information.

* **View Tag Reference** (⌃⌘J)
Opens the [JsDoc Toolkit tag reference][jsdot] in TextMate's Web Preview window.

## License

* **[JsDoc Toolkit][jsdoc]** ([MIT License][mit])

[mit]:    http://www.opensource.org/licenses/mit-license
[jsdoc]:  http://code.google.com/p/jsdoc-toolkit/
[jsdop]:  http://code.google.com/p/jsdoc-toolkit/wiki/CommandlineOptions
[jsdot]:  http://code.google.com/p/jsdoc-toolkit/wiki/TagReference
[getb]:   http://svn.textmate.org/trunk/Review/Bundles/GetBundles.tmbundle/