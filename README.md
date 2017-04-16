# api documentation for  [blessed (v0.1.81)](https://github.com/chjj/blessed)  [![npm package](https://img.shields.io/npm/v/npmdoc-blessed.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-blessed) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-blessed.svg)](https://travis-ci.org/npmdoc/node-npmdoc-blessed)
#### A high-level terminal interface library for node.js.

[![NPM](https://nodei.co/npm/blessed.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/blessed)

[![apidoc](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-blessed/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christopher Jeffrey"
    },
    "bin": {
        "blessed": "./bin/tput.js"
    },
    "browserify": {
        "transform": [
            "./browser/transform.js"
        ]
    },
    "bugs": {
        "url": "http://github.com/chjj/blessed/issues"
    },
    "dependencies": {},
    "description": "A high-level terminal interface library for node.js.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "f962d687ec2c369570ae71af843256e6d0ca1129",
        "tarball": "https://registry.npmjs.org/blessed/-/blessed-0.1.81.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "a45575fee63fac158fd467087ec172f657bfec6b",
    "homepage": "https://github.com/chjj/blessed",
    "keywords": [
        "curses",
        "tui",
        "tput",
        "terminfo",
        "termcap"
    ],
    "license": "MIT",
    "main": "./lib/blessed.js",
    "maintainers": [
        {
            "name": "chjj"
        }
    ],
    "name": "blessed",
    "optionalDependencies": {},
    "preferGlobal": false,
    "repository": {
        "type": "git",
        "url": "git://github.com/chjj/blessed.git"
    },
    "scripts": {},
    "tags": [
        "curses",
        "tui",
        "tput",
        "terminfo",
        "termcap"
    ],
    "version": "0.1.81"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module blessed](#apidoc.module.blessed)
1.  [function <span class="apidocSignatureSpan"></span>blessed ()](#apidoc.element.blessed.blessed)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ANSIImage (options)](#apidoc.element.blessed.ANSIImage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>BigText (options)](#apidoc.element.blessed.BigText)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Box (options)](#apidoc.element.blessed.Box)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Button (options)](#apidoc.element.blessed.Button)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Checkbox (options)](#apidoc.element.blessed.Checkbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Element (options)](#apidoc.element.blessed.Element)
1.  [function <span class="apidocSignatureSpan">blessed.</span>FileManager (options)](#apidoc.element.blessed.FileManager)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Form (options)](#apidoc.element.blessed.Form)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Image (options)](#apidoc.element.blessed.Image)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Input (options)](#apidoc.element.blessed.Input)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Layout (options)](#apidoc.element.blessed.Layout)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Line (options)](#apidoc.element.blessed.Line)
1.  [function <span class="apidocSignatureSpan">blessed.</span>List (options)](#apidoc.element.blessed.List)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ListBar (options)](#apidoc.element.blessed.ListBar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ListTable (options)](#apidoc.element.blessed.ListTable)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Listbar (options)](#apidoc.element.blessed.Listbar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Loading (options)](#apidoc.element.blessed.Loading)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Log (options)](#apidoc.element.blessed.Log)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Message (options)](#apidoc.element.blessed.Message)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Node (options)](#apidoc.element.blessed.Node)
1.  [function <span class="apidocSignatureSpan">blessed.</span>OverlayImage (options)](#apidoc.element.blessed.OverlayImage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>PNG (options)](#apidoc.element.blessed.PNG)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Program (options)](#apidoc.element.blessed.Program)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ProgressBar (options)](#apidoc.element.blessed.ProgressBar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Prompt (options)](#apidoc.element.blessed.Prompt)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Question (options)](#apidoc.element.blessed.Question)
1.  [function <span class="apidocSignatureSpan">blessed.</span>RadioButton (options)](#apidoc.element.blessed.RadioButton)
1.  [function <span class="apidocSignatureSpan">blessed.</span>RadioSet (options)](#apidoc.element.blessed.RadioSet)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Screen (options)](#apidoc.element.blessed.Screen)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ScrollableBox (options)](#apidoc.element.blessed.ScrollableBox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ScrollableText (options)](#apidoc.element.blessed.ScrollableText)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Table (options)](#apidoc.element.blessed.Table)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Terminal (options)](#apidoc.element.blessed.Terminal)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Text (options)](#apidoc.element.blessed.Text)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Textarea (options)](#apidoc.element.blessed.Textarea)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Textbox (options)](#apidoc.element.blessed.Textbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Tput (options)](#apidoc.element.blessed.Tput)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Video (options)](#apidoc.element.blessed.Video)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ansiimage (options)](#apidoc.element.blessed.ansiimage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>asort (obj)](#apidoc.element.blessed.asort)
1.  [function <span class="apidocSignatureSpan">blessed.</span>attrToBinary (style, element)](#apidoc.element.blessed.attrToBinary)
1.  [function <span class="apidocSignatureSpan">blessed.</span>bigtext (options)](#apidoc.element.blessed.bigtext)
1.  [function <span class="apidocSignatureSpan">blessed.</span>box (options)](#apidoc.element.blessed.box)
1.  [function <span class="apidocSignatureSpan">blessed.</span>button (options)](#apidoc.element.blessed.button)
1.  [function <span class="apidocSignatureSpan">blessed.</span>checkbox (options)](#apidoc.element.blessed.checkbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>cleanTags (text)](#apidoc.element.blessed.cleanTags)
1.  [function <span class="apidocSignatureSpan">blessed.</span>dropUnicode (text)](#apidoc.element.blessed.dropUnicode)
1.  [function <span class="apidocSignatureSpan">blessed.</span>element (options)](#apidoc.element.blessed.element)
1.  [function <span class="apidocSignatureSpan">blessed.</span>escape (text)](#apidoc.element.blessed.escape)
1.  [function <span class="apidocSignatureSpan">blessed.</span>filemanager (options)](#apidoc.element.blessed.filemanager)
1.  [function <span class="apidocSignatureSpan">blessed.</span>findFile (start, target)](#apidoc.element.blessed.findFile)
1.  [function <span class="apidocSignatureSpan">blessed.</span>form (options)](#apidoc.element.blessed.form)
1.  [function <span class="apidocSignatureSpan">blessed.</span>generateTags (style, text)](#apidoc.element.blessed.generateTags)
1.  [function <span class="apidocSignatureSpan">blessed.</span>hsort (obj)](#apidoc.element.blessed.hsort)
1.  [function <span class="apidocSignatureSpan">blessed.</span>image (options)](#apidoc.element.blessed.image)
1.  [function <span class="apidocSignatureSpan">blessed.</span>input (options)](#apidoc.element.blessed.input)
1.  [function <span class="apidocSignatureSpan">blessed.</span>layout (options)](#apidoc.element.blessed.layout)
1.  [function <span class="apidocSignatureSpan">blessed.</span>line (options)](#apidoc.element.blessed.line)
1.  [function <span class="apidocSignatureSpan">blessed.</span>list (options)](#apidoc.element.blessed.list)
1.  [function <span class="apidocSignatureSpan">blessed.</span>listbar (options)](#apidoc.element.blessed.listbar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>listtable (options)](#apidoc.element.blessed.listtable)
1.  [function <span class="apidocSignatureSpan">blessed.</span>loading (options)](#apidoc.element.blessed.loading)
1.  [function <span class="apidocSignatureSpan">blessed.</span>log (options)](#apidoc.element.blessed.log)
1.  [function <span class="apidocSignatureSpan">blessed.</span>merge (a, b)](#apidoc.element.blessed.merge)
1.  [function <span class="apidocSignatureSpan">blessed.</span>message (options)](#apidoc.element.blessed.message)
1.  [function <span class="apidocSignatureSpan">blessed.</span>node (options)](#apidoc.element.blessed.node)
1.  [function <span class="apidocSignatureSpan">blessed.</span>overlayimage (options)](#apidoc.element.blessed.overlayimage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>parseTags (text, screen)](#apidoc.element.blessed.parseTags)
1.  [function <span class="apidocSignatureSpan">blessed.</span>png (options)](#apidoc.element.blessed.png)
1.  [function <span class="apidocSignatureSpan">blessed.</span>program (options)](#apidoc.element.blessed.program)
1.  [function <span class="apidocSignatureSpan">blessed.</span>progressbar (options)](#apidoc.element.blessed.progressbar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>prompt (options)](#apidoc.element.blessed.prompt)
1.  [function <span class="apidocSignatureSpan">blessed.</span>question (options)](#apidoc.element.blessed.question)
1.  [function <span class="apidocSignatureSpan">blessed.</span>radiobutton (options)](#apidoc.element.blessed.radiobutton)
1.  [function <span class="apidocSignatureSpan">blessed.</span>radioset (options)](#apidoc.element.blessed.radioset)
1.  [function <span class="apidocSignatureSpan">blessed.</span>screen (options)](#apidoc.element.blessed.screen)
1.  [function <span class="apidocSignatureSpan">blessed.</span>scrollablebox (options)](#apidoc.element.blessed.scrollablebox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>scrollabletext (options)](#apidoc.element.blessed.scrollabletext)
1.  [function <span class="apidocSignatureSpan">blessed.</span>sprintf (src)](#apidoc.element.blessed.sprintf)
1.  [function <span class="apidocSignatureSpan">blessed.</span>stripTags (text)](#apidoc.element.blessed.stripTags)
1.  [function <span class="apidocSignatureSpan">blessed.</span>table (options)](#apidoc.element.blessed.table)
1.  [function <span class="apidocSignatureSpan">blessed.</span>terminal (options)](#apidoc.element.blessed.terminal)
1.  [function <span class="apidocSignatureSpan">blessed.</span>text (options)](#apidoc.element.blessed.text)
1.  [function <span class="apidocSignatureSpan">blessed.</span>textarea (options)](#apidoc.element.blessed.textarea)
1.  [function <span class="apidocSignatureSpan">blessed.</span>textbox (options)](#apidoc.element.blessed.textbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>toString ()](#apidoc.element.blessed.toString)
1.  [function <span class="apidocSignatureSpan">blessed.</span>tput (options)](#apidoc.element.blessed.tput)
1.  [function <span class="apidocSignatureSpan">blessed.</span>tryRead (file)](#apidoc.element.blessed.tryRead)
1.  [function <span class="apidocSignatureSpan">blessed.</span>video (options)](#apidoc.element.blessed.video)
1.  object <span class="apidocSignatureSpan">blessed.</span>Element.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>Program.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>Screen.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>Tput.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>aliases
1.  object <span class="apidocSignatureSpan">blessed.</span>ansiimage.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>bigtext.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>button.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>checkbox.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>classes
1.  object <span class="apidocSignatureSpan">blessed.</span>colors
1.  object <span class="apidocSignatureSpan">blessed.</span>filemanager.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>form.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>helpers
1.  object <span class="apidocSignatureSpan">blessed.</span>layout.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>list.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>listbar.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>listtable.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>loading.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>log.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>message.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>node.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>overlayimage.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>progressbar.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>prompt.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>question.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>radiobutton.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>scrollablebox.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>table.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>terminal.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>textarea.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>textbox.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>unicode
1.  object <span class="apidocSignatureSpan">blessed.</span>video.prototype
1.  object <span class="apidocSignatureSpan">blessed.</span>widget

#### [module blessed.Element](#apidoc.module.blessed.Element)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Element (options)](#apidoc.element.blessed.Element.Element)

#### [module blessed.Element.prototype](#apidoc.module.blessed.Element.prototype)
1.  boolean <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_detached
1.  boolean <span class="apidocSignatureSpan">blessed.Element.prototype.</span>draggable
1.  boolean <span class="apidocSignatureSpan">blessed.Element.prototype.</span>visible
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_align (line, width, align)](#apidoc.element.blessed.Element.prototype._align)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getBottom (get)](#apidoc.element.blessed.Element.prototype._getBottom)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getCoords (get, noscroll)](#apidoc.element.blessed.Element.prototype._getCoords)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getHeight (get)](#apidoc.element.blessed.Element.prototype._getHeight)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getLeft (get)](#apidoc.element.blessed.Element.prototype._getLeft)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getPos ()](#apidoc.element.blessed.Element.prototype._getPos)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getRight (get)](#apidoc.element.blessed.Element.prototype._getRight)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrink (xi, xl, yi, yl, get)](#apidoc.element.blessed.Element.prototype._getShrink)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrinkBox (xi, xl, yi, yl, get)](#apidoc.element.blessed.Element.prototype._getShrinkBox)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrinkContent (xi, xl, yi, yl)](#apidoc.element.blessed.Element.prototype._getShrinkContent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getTop (get)](#apidoc.element.blessed.Element.prototype._getTop)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getWidth (get)](#apidoc.element.blessed.Element.prototype._getWidth)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_parseAttr (lines)](#apidoc.element.blessed.Element.prototype._parseAttr)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_parseTags (text)](#apidoc.element.blessed.Element.prototype._parseTags)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_render ()](#apidoc.element.blessed.Element.prototype._render)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_wrapContent (content, width)](#apidoc.element.blessed.Element.prototype._wrapContent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearBaseLine (i)](#apidoc.element.blessed.Element.prototype.clearBaseLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearLine (i)](#apidoc.element.blessed.Element.prototype.clearLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearPos (get, override)](#apidoc.element.blessed.Element.prototype.clearPos)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteBottom (n)](#apidoc.element.blessed.Element.prototype.deleteBottom)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteLine (i, n)](#apidoc.element.blessed.Element.prototype.deleteLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteTop (n)](#apidoc.element.blessed.Element.prototype.deleteTop)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>disableDrag ()](#apidoc.element.blessed.Element.prototype.disableDrag)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableDrag (verify)](#apidoc.element.blessed.Element.prototype.enableDrag)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableInput ()](#apidoc.element.blessed.Element.prototype.enableInput)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableKeys ()](#apidoc.element.blessed.Element.prototype.enableKeys)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableMouse ()](#apidoc.element.blessed.Element.prototype.enableMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>focus ()](#apidoc.element.blessed.Element.prototype.focus)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>free ()](#apidoc.element.blessed.Element.prototype.free)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getBaseLine (i)](#apidoc.element.blessed.Element.prototype.getBaseLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getContent ()](#apidoc.element.blessed.Element.prototype.getContent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getLine (i)](#apidoc.element.blessed.Element.prototype.getLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getLines ()](#apidoc.element.blessed.Element.prototype.getLines)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getScreenLines ()](#apidoc.element.blessed.Element.prototype.getScreenLines)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getText ()](#apidoc.element.blessed.Element.prototype.getText)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>hide ()](#apidoc.element.blessed.Element.prototype.hide)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertBottom (line)](#apidoc.element.blessed.Element.prototype.insertBottom)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertLine (i, line)](#apidoc.element.blessed.Element.prototype.insertLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertTop (line)](#apidoc.element.blessed.Element.prototype.insertTop)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>key ()](#apidoc.element.blessed.Element.prototype.key)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.onScreenEvent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onceKey ()](#apidoc.element.blessed.Element.prototype.onceKey)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onceScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.onceScreenEvent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>parseContent (noTags)](#apidoc.element.blessed.Element.prototype.parseContent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>popLine (n)](#apidoc.element.blessed.Element.prototype.popLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>pushLine (line)](#apidoc.element.blessed.Element.prototype.pushLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeHover ()](#apidoc.element.blessed.Element.prototype.removeHover)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeKey ()](#apidoc.element.blessed.Element.prototype.removeKey)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeLabel ()](#apidoc.element.blessed.Element.prototype.removeLabel)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.removeScreenEvent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>render ()](#apidoc.element.blessed.Element.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>sattr (style, fg, bg)](#apidoc.element.blessed.Element.prototype.sattr)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>screenshot (xi, xl, yi, yl)](#apidoc.element.blessed.Element.prototype.screenshot)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setBack ()](#apidoc.element.blessed.Element.prototype.setBack)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setBaseLine (i, line)](#apidoc.element.blessed.Element.prototype.setBaseLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setContent (content, noClear, noTags)](#apidoc.element.blessed.Element.prototype.setContent)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setFront ()](#apidoc.element.blessed.Element.prototype.setFront)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setHover (options)](#apidoc.element.blessed.Element.prototype.setHover)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setIndex (index)](#apidoc.element.blessed.Element.prototype.setIndex)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setLabel (options)](#apidoc.element.blessed.Element.prototype.setLabel)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setLine (i, line)](#apidoc.element.blessed.Element.prototype.setLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setText (content, noClear)](#apidoc.element.blessed.Element.prototype.setText)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>shiftLine (n)](#apidoc.element.blessed.Element.prototype.shiftLine)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>show ()](#apidoc.element.blessed.Element.prototype.show)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>strWidth (text)](#apidoc.element.blessed.Element.prototype.strWidth)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>toggle ()](#apidoc.element.blessed.Element.prototype.toggle)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>unkey ()](#apidoc.element.blessed.Element.prototype.unkey)
1.  [function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>unshiftLine (line)](#apidoc.element.blessed.Element.prototype.unshiftLine)
1.  string <span class="apidocSignatureSpan">blessed.Element.prototype.</span>type

#### [module blessed.Program](#apidoc.module.blessed.Program)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Program (options)](#apidoc.element.blessed.Program.Program)
1.  [function <span class="apidocSignatureSpan">blessed.Program.</span>bind (program)](#apidoc.element.blessed.Program.bind)
1.  number <span class="apidocSignatureSpan">blessed.Program.</span>total
1.  object <span class="apidocSignatureSpan">blessed.Program.</span>global
1.  object <span class="apidocSignatureSpan">blessed.Program.</span>instances

#### [module blessed.Program.prototype](#apidoc.module.blessed.Program.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>HPositionRelative (param)](#apidoc.element.blessed.Program.prototype.HPositionRelative)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>HVPosition (row, col)](#apidoc.element.blessed.Program.prototype.HVPosition)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>VPositionRelative (param)](#apidoc.element.blessed.Program.prototype.VPositionRelative)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_attr (param, val)](#apidoc.element.blessed.Program.prototype._attr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_bindMouse (s, buf)](#apidoc.element.blessed.Program.prototype._bindMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_bindResponse (s)](#apidoc.element.blessed.Program.prototype._bindResponse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_buffer (text)](#apidoc.element.blessed.Program.prototype._buffer)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_listenInput ()](#apidoc.element.blessed.Program.prototype._listenInput)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_listenOutput ()](#apidoc.element.blessed.Program.prototype._listenOutput)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_log (pre, msg)](#apidoc.element.blessed.Program.prototype._log)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_ncoords ()](#apidoc.element.blessed.Program.prototype._ncoords)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_owrite (text)](#apidoc.element.blessed.Program.prototype._owrite)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_twrite (data)](#apidoc.element.blessed.Program.prototype._twrite)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_write (text)](#apidoc.element.blessed.Program.prototype._write)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ae ()](#apidoc.element.blessed.Program.prototype.ae)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>alternate ()](#apidoc.element.blessed.Program.prototype.alternate)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>alternateBuffer ()](#apidoc.element.blessed.Program.prototype.alternateBuffer)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>as ()](#apidoc.element.blessed.Program.prototype.as)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>attr (param, val)](#apidoc.element.blessed.Program.prototype.attr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>back (param)](#apidoc.element.blessed.Program.prototype.back)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>backspace ()](#apidoc.element.blessed.Program.prototype.backspace)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bel ()](#apidoc.element.blessed.Program.prototype.bel)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bell ()](#apidoc.element.blessed.Program.prototype.bell)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bg (color, val)](#apidoc.element.blessed.Program.prototype.bg)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bindMouse ()](#apidoc.element.blessed.Program.prototype.bindMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bindResponse ()](#apidoc.element.blessed.Program.prototype.bindResponse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cbt (param)](#apidoc.element.blessed.Program.prototype.cbt)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cha (param)](#apidoc.element.blessed.Program.prototype.cha)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charAttributes (param, val)](#apidoc.element.blessed.Program.prototype.charAttributes)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charPosAbsolute (param)](#apidoc.element.blessed.Program.prototype.charPosAbsolute)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charset (val, level)](#apidoc.element.blessed.Program.prototype.charset)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cht (param)](#apidoc.element.blessed.Program.prototype.cht)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>civis ()](#apidoc.element.blessed.Program.prototype.civis)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>clear ()](#apidoc.element.blessed.Program.prototype.clear)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cnl (param)](#apidoc.element.blessed.Program.prototype.cnl)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cnorm ()](#apidoc.element.blessed.Program.prototype.cnorm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>copyRectangle ()](#apidoc.element.blessed.Program.prototype.copyRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>copyToClipboard (text)](#apidoc.element.blessed.Program.prototype.copyToClipboard)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cpl (param)](#apidoc.element.blessed.Program.prototype.cpl)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cr ()](#apidoc.element.blessed.Program.prototype.cr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>csr (top, bottom)](#apidoc.element.blessed.Program.prototype.csr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cub (param)](#apidoc.element.blessed.Program.prototype.cub)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cud (param)](#apidoc.element.blessed.Program.prototype.cud)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cuf (param)](#apidoc.element.blessed.Program.prototype.cuf)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cup (row, col)](#apidoc.element.blessed.Program.prototype.cup)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorBackward (param)](#apidoc.element.blessed.Program.prototype.cursorBackward)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorBackwardTab (param)](#apidoc.element.blessed.Program.prototype.cursorBackwardTab)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorCharAbsolute (param)](#apidoc.element.blessed.Program.prototype.cursorCharAbsolute)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorColor (color)](#apidoc.element.blessed.Program.prototype.cursorColor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorDown (param)](#apidoc.element.blessed.Program.prototype.cursorDown)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorForward (param)](#apidoc.element.blessed.Program.prototype.cursorForward)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorForwardTab (param)](#apidoc.element.blessed.Program.prototype.cursorForwardTab)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorNextLine (param)](#apidoc.element.blessed.Program.prototype.cursorNextLine)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorPos (row, col)](#apidoc.element.blessed.Program.prototype.cursorPos)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorPrecedingLine (param)](#apidoc.element.blessed.Program.prototype.cursorPrecedingLine)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorReset ()](#apidoc.element.blessed.Program.prototype.cursorReset)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorShape (shape, blink)](#apidoc.element.blessed.Program.prototype.cursorShape)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorUp (param)](#apidoc.element.blessed.Program.prototype.cursorUp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursor_invisible ()](#apidoc.element.blessed.Program.prototype.cursor_invisible)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cuu (param)](#apidoc.element.blessed.Program.prototype.cuu)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cvvis ()](#apidoc.element.blessed.Program.prototype.cvvis)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>da (param, callback)](#apidoc.element.blessed.Program.prototype.da)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dch (param)](#apidoc.element.blessed.Program.prototype.dch)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>debug ()](#apidoc.element.blessed.Program.prototype.debug)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deccara ()](#apidoc.element.blessed.Program.prototype.deccara)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deccra ()](#apidoc.element.blessed.Program.prototype.deccra)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decdc ()](#apidoc.element.blessed.Program.prototype.decdc)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decefr ()](#apidoc.element.blessed.Program.prototype.decefr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decelr ()](#apidoc.element.blessed.Program.prototype.decelr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decera ()](#apidoc.element.blessed.Program.prototype.decera)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decfra ()](#apidoc.element.blessed.Program.prototype.decfra)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decic ()](#apidoc.element.blessed.Program.prototype.decic)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decll (param)](#apidoc.element.blessed.Program.prototype.decll)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrara ()](#apidoc.element.blessed.Program.prototype.decrara)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decreqtparm (param)](#apidoc.element.blessed.Program.prototype.decreqtparm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqlp (param, callback)](#apidoc.element.blessed.Program.prototype.decrqlp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqm (param)](#apidoc.element.blessed.Program.prototype.decrqm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqmp (param)](#apidoc.element.blessed.Program.prototype.decrqmp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrst ()](#apidoc.element.blessed.Program.prototype.decrst)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsace (param)](#apidoc.element.blessed.Program.prototype.decsace)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsca (param)](#apidoc.element.blessed.Program.prototype.decsca)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decscl ()](#apidoc.element.blessed.Program.prototype.decscl)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decscusr (param)](#apidoc.element.blessed.Program.prototype.decscusr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsera ()](#apidoc.element.blessed.Program.prototype.decsera)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decset ()](#apidoc.element.blessed.Program.prototype.decset)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsle ()](#apidoc.element.blessed.Program.prototype.decsle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsmbv (param)](#apidoc.element.blessed.Program.prototype.decsmbv)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decstbm (top, bottom)](#apidoc.element.blessed.Program.prototype.decstbm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decstr ()](#apidoc.element.blessed.Program.prototype.decstr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decswbv (param)](#apidoc.element.blessed.Program.prototype.decswbv)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dectcem ()](#apidoc.element.blessed.Program.prototype.dectcem)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dectcemh ()](#apidoc.element.blessed.Program.prototype.dectcemh)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteChars (param)](#apidoc.element.blessed.Program.prototype.deleteChars)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteColumns ()](#apidoc.element.blessed.Program.prototype.deleteColumns)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteLines (param)](#apidoc.element.blessed.Program.prototype.deleteLines)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>destroy ()](#apidoc.element.blessed.Program.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deviceStatus (param, callback, dec, noBypass)](#apidoc.element.blessed.Program.prototype.deviceStatus)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableGpm ()](#apidoc.element.blessed.Program.prototype.disableGpm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableModifiers (param)](#apidoc.element.blessed.Program.prototype.disableModifiers)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableMouse ()](#apidoc.element.blessed.Program.prototype.disableMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dl (param)](#apidoc.element.blessed.Program.prototype.dl)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>down (param)](#apidoc.element.blessed.Program.prototype.down)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dsr (param, callback, dec, noBypass)](#apidoc.element.blessed.Program.prototype.dsr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dynamicColors (param)](#apidoc.element.blessed.Program.prototype.dynamicColors)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ech (param)](#apidoc.element.blessed.Program.prototype.ech)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>echo (text, attr)](#apidoc.element.blessed.Program.prototype.echo)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ed (param)](#apidoc.element.blessed.Program.prototype.ed)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>el (param)](#apidoc.element.blessed.Program.prototype.el)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableFilterRectangle ()](#apidoc.element.blessed.Program.prototype.enableFilterRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableGpm ()](#apidoc.element.blessed.Program.prototype.enableGpm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableLocatorReporting ()](#apidoc.element.blessed.Program.prototype.enableLocatorReporting)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableMouse ()](#apidoc.element.blessed.Program.prototype.enableMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enter_alt_charset_mode ()](#apidoc.element.blessed.Program.prototype.enter_alt_charset_mode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseChars (param)](#apidoc.element.blessed.Program.prototype.eraseChars)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseInDisplay (param)](#apidoc.element.blessed.Program.prototype.eraseInDisplay)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseInLine (param)](#apidoc.element.blessed.Program.prototype.eraseInLine)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseRectangle ()](#apidoc.element.blessed.Program.prototype.eraseRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>exit_alt_charset_mode ()](#apidoc.element.blessed.Program.prototype.exit_alt_charset_mode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>feed ()](#apidoc.element.blessed.Program.prototype.feed)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ff ()](#apidoc.element.blessed.Program.prototype.ff)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>fg (color, val)](#apidoc.element.blessed.Program.prototype.fg)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>fillRectangle ()](#apidoc.element.blessed.Program.prototype.fillRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>flush ()](#apidoc.element.blessed.Program.prototype.flush)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>form ()](#apidoc.element.blessed.Program.prototype.form)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>forward (param)](#apidoc.element.blessed.Program.prototype.forward)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getCursor (callback)](#apidoc.element.blessed.Program.prototype.getCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getCursorColor (callback)](#apidoc.element.blessed.Program.prototype.getCursorColor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getTextParams (param, callback)](#apidoc.element.blessed.Program.prototype.getTextParams)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getWindowSize (callback)](#apidoc.element.blessed.Program.prototype.getWindowSize)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>has (name)](#apidoc.element.blessed.Program.prototype.has)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hideCursor ()](#apidoc.element.blessed.Program.prototype.hideCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hpa (param)](#apidoc.element.blessed.Program.prototype.hpa)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hpr (param)](#apidoc.element.blessed.Program.prototype.hpr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ht ()](#apidoc.element.blessed.Program.prototype.ht)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hvp (row, col)](#apidoc.element.blessed.Program.prototype.hvp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ich (param)](#apidoc.element.blessed.Program.prototype.ich)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>il (param)](#apidoc.element.blessed.Program.prototype.il)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ind ()](#apidoc.element.blessed.Program.prototype.ind)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>index ()](#apidoc.element.blessed.Program.prototype.index)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>initMouseTracking ()](#apidoc.element.blessed.Program.prototype.initMouseTracking)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertChars (param)](#apidoc.element.blessed.Program.prototype.insertChars)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertColumns ()](#apidoc.element.blessed.Program.prototype.insertColumns)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertLines (param)](#apidoc.element.blessed.Program.prototype.insertLines)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>kbs ()](#apidoc.element.blessed.Program.prototype.kbs)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>key (key, listener)](#apidoc.element.blessed.Program.prototype.key)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>left (param)](#apidoc.element.blessed.Program.prototype.left)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lineHeight ()](#apidoc.element.blessed.Program.prototype.lineHeight)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>linePosAbsolute (param)](#apidoc.element.blessed.Program.prototype.linePosAbsolute)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>listen ()](#apidoc.element.blessed.Program.prototype.listen)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>loadLEDs (param)](#apidoc.element.blessed.Program.prototype.loadLEDs)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>log ()](#apidoc.element.blessed.Program.prototype.log)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lrestoreCursor (key, hide)](#apidoc.element.blessed.Program.prototype.lrestoreCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lsaveCursor (key)](#apidoc.element.blessed.Program.prototype.lsaveCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>manipulateWindow ()](#apidoc.element.blessed.Program.prototype.manipulateWindow)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc ()](#apidoc.element.blessed.Program.prototype.mc)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc0 ()](#apidoc.element.blessed.Program.prototype.mc0)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc4 ()](#apidoc.element.blessed.Program.prototype.mc4)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc5 ()](#apidoc.element.blessed.Program.prototype.mc5)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc5p ()](#apidoc.element.blessed.Program.prototype.mc5p)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mediaCopy ()](#apidoc.element.blessed.Program.prototype.mediaCopy)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>move (x, y)](#apidoc.element.blessed.Program.prototype.move)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nel ()](#apidoc.element.blessed.Program.prototype.nel)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>newline ()](#apidoc.element.blessed.Program.prototype.newline)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nextLine ()](#apidoc.element.blessed.Program.prototype.nextLine)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>normalBuffer ()](#apidoc.element.blessed.Program.prototype.normalBuffer)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nul ()](#apidoc.element.blessed.Program.prototype.nul)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>omove (x, y)](#apidoc.element.blessed.Program.prototype.omove)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>onceKey (key, listener)](#apidoc.element.blessed.Program.prototype.onceKey)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>out (name)](#apidoc.element.blessed.Program.prototype.out)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pO ()](#apidoc.element.blessed.Program.prototype.pO)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pause (callback)](#apidoc.element.blessed.Program.prototype.pause)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pf ()](#apidoc.element.blessed.Program.prototype.pf)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>po ()](#apidoc.element.blessed.Program.prototype.po)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pos (row, col)](#apidoc.element.blessed.Program.prototype.pos)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>print (text, attr)](#apidoc.element.blessed.Program.prototype.print)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>print_screen ()](#apidoc.element.blessed.Program.prototype.print_screen)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_non ()](#apidoc.element.blessed.Program.prototype.prtr_non)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_off ()](#apidoc.element.blessed.Program.prototype.prtr_off)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_on ()](#apidoc.element.blessed.Program.prototype.prtr_on)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ps ()](#apidoc.element.blessed.Program.prototype.ps)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rc (key, hide)](#apidoc.element.blessed.Program.prototype.rc)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rcA ()](#apidoc.element.blessed.Program.prototype.rcA)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>removeKey (key, listener)](#apidoc.element.blessed.Program.prototype.removeKey)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rep (param)](#apidoc.element.blessed.Program.prototype.rep)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>repeat (ch, i)](#apidoc.element.blessed.Program.prototype.repeat)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>repeatPrecedingCharacter (param)](#apidoc.element.blessed.Program.prototype.repeatPrecedingCharacter)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>req_mouse_pos (param, callback)](#apidoc.element.blessed.Program.prototype.req_mouse_pos)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reqmp (param, callback)](#apidoc.element.blessed.Program.prototype.reqmp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestAnsiMode (param)](#apidoc.element.blessed.Program.prototype.requestAnsiMode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestLocatorPosition (param, callback)](#apidoc.element.blessed.Program.prototype.requestLocatorPosition)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestParameters (param)](#apidoc.element.blessed.Program.prototype.requestParameters)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestPrivateMode (param)](#apidoc.element.blessed.Program.prototype.requestPrivateMode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reset ()](#apidoc.element.blessed.Program.prototype.reset)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetColors (param)](#apidoc.element.blessed.Program.prototype.resetColors)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetCursor ()](#apidoc.element.blessed.Program.prototype.resetCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetMode ()](#apidoc.element.blessed.Program.prototype.resetMode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetTitleModes ()](#apidoc.element.blessed.Program.prototype.resetTitleModes)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>response (name, text, callback, noBypass)](#apidoc.element.blessed.Program.prototype.response)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreCursor (key, hide)](#apidoc.element.blessed.Program.prototype.restoreCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreCursorA ()](#apidoc.element.blessed.Program.prototype.restoreCursorA)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restorePrivateValues ()](#apidoc.element.blessed.Program.prototype.restorePrivateValues)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreReportedCursor ()](#apidoc.element.blessed.Program.prototype.restoreReportedCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resume ()](#apidoc.element.blessed.Program.prototype.resume)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>return ()](#apidoc.element.blessed.Program.prototype.return)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverse ()](#apidoc.element.blessed.Program.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverseAttrInRectangle ()](#apidoc.element.blessed.Program.prototype.reverseAttrInRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverseIndex ()](#apidoc.element.blessed.Program.prototype.reverseIndex)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ri ()](#apidoc.element.blessed.Program.prototype.ri)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>right (param)](#apidoc.element.blessed.Program.prototype.right)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rm ()](#apidoc.element.blessed.Program.prototype.rm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmacs ()](#apidoc.element.blessed.Program.prototype.rmacs)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmcup ()](#apidoc.element.blessed.Program.prototype.rmcup)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmove (x, y)](#apidoc.element.blessed.Program.prototype.rmove)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rs2 ()](#apidoc.element.blessed.Program.prototype.rs2)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rsetx (x)](#apidoc.element.blessed.Program.prototype.rsetx)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rsety (y)](#apidoc.element.blessed.Program.prototype.rsety)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveCursor (key)](#apidoc.element.blessed.Program.prototype.saveCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveCursorA ()](#apidoc.element.blessed.Program.prototype.saveCursorA)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>savePrivateValues ()](#apidoc.element.blessed.Program.prototype.savePrivateValues)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveReportedCursor (callback)](#apidoc.element.blessed.Program.prototype.saveReportedCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sc (key)](#apidoc.element.blessed.Program.prototype.sc)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scA ()](#apidoc.element.blessed.Program.prototype.scA)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scrollDown (param)](#apidoc.element.blessed.Program.prototype.scrollDown)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scrollUp (param)](#apidoc.element.blessed.Program.prototype.scrollUp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sd (param)](#apidoc.element.blessed.Program.prototype.sd)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selData (a, b)](#apidoc.element.blessed.Program.prototype.selData)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selectChangeExtent (param)](#apidoc.element.blessed.Program.prototype.selectChangeExtent)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selectiveEraseRectangle ()](#apidoc.element.blessed.Program.prototype.selectiveEraseRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sendDeviceAttributes (param, callback)](#apidoc.element.blessed.Program.prototype.sendDeviceAttributes)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setAttrInRectangle ()](#apidoc.element.blessed.Program.prototype.setAttrInRectangle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setBackground (color, val)](#apidoc.element.blessed.Program.prototype.setBackground)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setCharProtectionAttr (param)](#apidoc.element.blessed.Program.prototype.setCharProtectionAttr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setConformanceLevel ()](#apidoc.element.blessed.Program.prototype.setConformanceLevel)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setCursorStyle (param)](#apidoc.element.blessed.Program.prototype.setCursorStyle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setForeground (color, val)](#apidoc.element.blessed.Program.prototype.setForeground)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setG (val)](#apidoc.element.blessed.Program.prototype.setG)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setLocatorEvents ()](#apidoc.element.blessed.Program.prototype.setLocatorEvents)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMarginBellVolume (param)](#apidoc.element.blessed.Program.prototype.setMarginBellVolume)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMode ()](#apidoc.element.blessed.Program.prototype.setMode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMouse (opt, enable)](#apidoc.element.blessed.Program.prototype.setMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setPointerMode (param)](#apidoc.element.blessed.Program.prototype.setPointerMode)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setResources ()](#apidoc.element.blessed.Program.prototype.setResources)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setScrollRegion (top, bottom)](#apidoc.element.blessed.Program.prototype.setScrollRegion)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTerminal (terminal)](#apidoc.element.blessed.Program.prototype.setTerminal)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTitle (title)](#apidoc.element.blessed.Program.prototype.setTitle)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTitleModeFeature ()](#apidoc.element.blessed.Program.prototype.setTitleModeFeature)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setWarningBellVolume (param)](#apidoc.element.blessed.Program.prototype.setWarningBellVolume)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setupDump ()](#apidoc.element.blessed.Program.prototype.setupDump)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setupTput ()](#apidoc.element.blessed.Program.prototype.setupTput)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setx (x)](#apidoc.element.blessed.Program.prototype.setx)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sety (y)](#apidoc.element.blessed.Program.prototype.sety)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sgr (param, val)](#apidoc.element.blessed.Program.prototype.sgr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>shiftIn ()](#apidoc.element.blessed.Program.prototype.shiftIn)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>shiftOut ()](#apidoc.element.blessed.Program.prototype.shiftOut)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>showCursor ()](#apidoc.element.blessed.Program.prototype.showCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sigtstp (callback)](#apidoc.element.blessed.Program.prototype.sigtstp)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>simpleInsert (ch, i, attr)](#apidoc.element.blessed.Program.prototype.simpleInsert)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sm ()](#apidoc.element.blessed.Program.prototype.sm)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>smacs ()](#apidoc.element.blessed.Program.prototype.smacs)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>smcup ()](#apidoc.element.blessed.Program.prototype.smcup)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>softReset ()](#apidoc.element.blessed.Program.prototype.softReset)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>su (param)](#apidoc.element.blessed.Program.prototype.su)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tab ()](#apidoc.element.blessed.Program.prototype.tab)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tabClear (param)](#apidoc.element.blessed.Program.prototype.tabClear)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tabSet ()](#apidoc.element.blessed.Program.prototype.tabSet)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tbc (param)](#apidoc.element.blessed.Program.prototype.tbc)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>term (is)](#apidoc.element.blessed.Program.prototype.term)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>text (text, attr)](#apidoc.element.blessed.Program.prototype.text)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>unkey (key, listener)](#apidoc.element.blessed.Program.prototype.unkey)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>up (param)](#apidoc.element.blessed.Program.prototype.up)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vi ()](#apidoc.element.blessed.Program.prototype.vi)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vpa (param)](#apidoc.element.blessed.Program.prototype.vpa)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vpr (param)](#apidoc.element.blessed.Program.prototype.vpr)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vtab ()](#apidoc.element.blessed.Program.prototype.vtab)
1.  [function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>write (text)](#apidoc.element.blessed.Program.prototype.write)
1.  string <span class="apidocSignatureSpan">blessed.Program.prototype.</span>type

#### [module blessed.Screen](#apidoc.module.blessed.Screen)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Screen (options)](#apidoc.element.blessed.Screen.Screen)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.</span>bind (screen)](#apidoc.element.blessed.Screen.bind)
1.  number <span class="apidocSignatureSpan">blessed.Screen.</span>total
1.  object <span class="apidocSignatureSpan">blessed.Screen.</span>global
1.  object <span class="apidocSignatureSpan">blessed.Screen.</span>instances

#### [module blessed.Screen.prototype](#apidoc.module.blessed.Screen.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_cursorAttr (cursor, dattr)](#apidoc.element.blessed.Screen.prototype._cursorAttr)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_destroy ()](#apidoc.element.blessed.Screen.prototype._destroy)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_dockBorders ()](#apidoc.element.blessed.Screen.prototype._dockBorders)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_focus (self, old)](#apidoc.element.blessed.Screen.prototype._focus)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_getAngle (lines, x, y)](#apidoc.element.blessed.Screen.prototype._getAngle)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_getPos ()](#apidoc.element.blessed.Screen.prototype._getPos)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_initHover ()](#apidoc.element.blessed.Screen.prototype._initHover)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_listenKeys (el)](#apidoc.element.blessed.Screen.prototype._listenKeys)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_listenMouse (el)](#apidoc.element.blessed.Screen.prototype._listenMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_reduceColor (color)](#apidoc.element.blessed.Screen.prototype._reduceColor)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>alloc (dirty)](#apidoc.element.blessed.Screen.prototype.alloc)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>attrCode (code, cur, def)](#apidoc.element.blessed.Screen.prototype.attrCode)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>blankLine (ch, dirty)](#apidoc.element.blessed.Screen.prototype.blankLine)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cleanSides (el)](#apidoc.element.blessed.Screen.prototype.cleanSides)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>clearRegion (xi, xl, yi, yl, override)](#apidoc.element.blessed.Screen.prototype.clearRegion)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>codeAttr (code)](#apidoc.element.blessed.Screen.prototype.codeAttr)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>copyToClipboard (text)](#apidoc.element.blessed.Screen.prototype.copyToClipboard)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorColor (color)](#apidoc.element.blessed.Screen.prototype.cursorColor)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorReset ()](#apidoc.element.blessed.Screen.prototype.cursorReset)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorShape (shape, blink)](#apidoc.element.blessed.Screen.prototype.cursorShape)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>debug ()](#apidoc.element.blessed.Screen.prototype.debug)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteBottom (top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteBottom)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteLine (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteLine)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteLineNC (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteLineNC)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteTop (top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteTop)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>destroy ()](#apidoc.element.blessed.Screen.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>displayImage (file, callback)](#apidoc.element.blessed.Screen.prototype.displayImage)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>draw (start, end)](#apidoc.element.blessed.Screen.prototype.draw)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableInput (el)](#apidoc.element.blessed.Screen.prototype.enableInput)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableKeys (el)](#apidoc.element.blessed.Screen.prototype.enableKeys)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableMouse (el)](#apidoc.element.blessed.Screen.prototype.enableMouse)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enter ()](#apidoc.element.blessed.Screen.prototype.enter)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>exec (file, args, options, callback)](#apidoc.element.blessed.Screen.prototype.exec)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>fillRegion (attr, ch, xi, xl, yi, yl, override)](#apidoc.element.blessed.Screen.prototype.fillRegion)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusNext ()](#apidoc.element.blessed.Screen.prototype.focusNext)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusOffset (offset)](#apidoc.element.blessed.Screen.prototype.focusOffset)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPop ()](#apidoc.element.blessed.Screen.prototype.focusPop)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPrev ()](#apidoc.element.blessed.Screen.prototype.focusPrev)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPrevious ()](#apidoc.element.blessed.Screen.prototype.focusPrevious)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPush (el)](#apidoc.element.blessed.Screen.prototype.focusPush)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertBottom (top, bottom)](#apidoc.element.blessed.Screen.prototype.insertBottom)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertLine (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.insertLine)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertLineNC (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.insertLineNC)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertTop (top, bottom)](#apidoc.element.blessed.Screen.prototype.insertTop)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>key ()](#apidoc.element.blessed.Screen.prototype.key)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>leave ()](#apidoc.element.blessed.Screen.prototype.leave)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>log ()](#apidoc.element.blessed.Screen.prototype.log)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>onceKey ()](#apidoc.element.blessed.Screen.prototype.onceKey)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>postEnter ()](#apidoc.element.blessed.Screen.prototype.postEnter)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>readEditor (options, callback)](#apidoc.element.blessed.Screen.prototype.readEditor)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>realloc ()](#apidoc.element.blessed.Screen.prototype.realloc)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>removeKey ()](#apidoc.element.blessed.Screen.prototype.removeKey)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>render ()](#apidoc.element.blessed.Screen.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>resetCursor ()](#apidoc.element.blessed.Screen.prototype.resetCursor)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>restoreFocus ()](#apidoc.element.blessed.Screen.prototype.restoreFocus)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>rewindFocus ()](#apidoc.element.blessed.Screen.prototype.rewindFocus)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>saveFocus ()](#apidoc.element.blessed.Screen.prototype.saveFocus)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>screenshot (xi, xl, yi, yl, term)](#apidoc.element.blessed.Screen.prototype.screenshot)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>setEffects (el, fel, over, out, effects, temp)](#apidoc.element.blessed.Screen.prototype.setEffects)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>setTerminal (terminal)](#apidoc.element.blessed.Screen.prototype.setTerminal)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>sigtstp (callback)](#apidoc.element.blessed.Screen.prototype.sigtstp)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>spawn (file, args, options)](#apidoc.element.blessed.Screen.prototype.spawn)
1.  [function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>unkey ()](#apidoc.element.blessed.Screen.prototype.unkey)
1.  string <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>type

#### [module blessed.Tput](#apidoc.module.blessed.Tput)
1.  [function <span class="apidocSignatureSpan">blessed.</span>Tput (options)](#apidoc.element.blessed.Tput.Tput)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.</span>_prefix (term)](#apidoc.element.blessed.Tput._prefix)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.</span>_tprefix (prefix, term, soft)](#apidoc.element.blessed.Tput._tprefix)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.</span>print ()](#apidoc.element.blessed.Tput.print)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.</span>sprintf (src)](#apidoc.element.blessed.Tput.sprintf)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.</span>tryRead (file)](#apidoc.element.blessed.Tput.tryRead)
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>_alias
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>acsc
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>alias
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>aliasMap
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>bools
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>cpaths
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>ipaths
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>numbers
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>strings
1.  object <span class="apidocSignatureSpan">blessed.Tput.</span>utoa
1.  string <span class="apidocSignatureSpan">blessed.Tput.</span>termcap

#### [module blessed.Tput.prototype](#apidoc.module.blessed.Tput.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>GetConsoleCP ()](#apidoc.element.blessed.Tput.prototype.GetConsoleCP)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_captoinfo (cap, s, parameterized)](#apidoc.element.blessed.Tput.prototype._captoinfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_compile (info, key, str)](#apidoc.element.blessed.Tput.prototype._compile)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_debug ()](#apidoc.element.blessed.Tput.prototype._debug)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_prefix (term)](#apidoc.element.blessed.Tput.prototype._prefix)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_print (code, print, done)](#apidoc.element.blessed.Tput.prototype._print)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_tprefix (prefix, term, soft)](#apidoc.element.blessed.Tput.prototype._tprefix)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_tryCap (file, term)](#apidoc.element.blessed.Tput.prototype._tryCap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useInternalCap (name)](#apidoc.element.blessed.Tput.prototype._useInternalCap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useInternalInfo (name)](#apidoc.element.blessed.Tput.prototype._useInternalInfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useVt102Cap ()](#apidoc.element.blessed.Tput.prototype._useVt102Cap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useXtermCap ()](#apidoc.element.blessed.Tput.prototype._useXtermCap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useXtermInfo ()](#apidoc.element.blessed.Tput.prototype._useXtermInfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compile (info)](#apidoc.element.blessed.Tput.prototype.compile)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileAll (start)](#apidoc.element.blessed.Tput.prototype.compileAll)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileTermcap (term)](#apidoc.element.blessed.Tput.prototype.compileTermcap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileTerminfo (term)](#apidoc.element.blessed.Tput.prototype.compileTerminfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectBrokenACS (info)](#apidoc.element.blessed.Tput.prototype.detectBrokenACS)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectFeatures (info)](#apidoc.element.blessed.Tput.prototype.detectFeatures)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectMagicCookie ()](#apidoc.element.blessed.Tput.prototype.detectMagicCookie)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectPCRomSet (info)](#apidoc.element.blessed.Tput.prototype.detectPCRomSet)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectPadding ()](#apidoc.element.blessed.Tput.prototype.detectPadding)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectSetbuf ()](#apidoc.element.blessed.Tput.prototype.detectSetbuf)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectUnicode ()](#apidoc.element.blessed.Tput.prototype.detectUnicode)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>getAll ()](#apidoc.element.blessed.Tput.prototype.getAll)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>has (name)](#apidoc.element.blessed.Tput.prototype.has)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>inject (info)](#apidoc.element.blessed.Tput.prototype.inject)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>injectTermcap (term)](#apidoc.element.blessed.Tput.prototype.injectTermcap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>injectTerminfo (term)](#apidoc.element.blessed.Tput.prototype.injectTerminfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseACS (info)](#apidoc.element.blessed.Tput.prototype.parseACS)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseExtended (data)](#apidoc.element.blessed.Tput.prototype.parseExtended)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseTermcap (data, file)](#apidoc.element.blessed.Tput.prototype.parseTermcap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseTerminfo (data, file)](#apidoc.element.blessed.Tput.prototype.parseTerminfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>readTermcap (term)](#apidoc.element.blessed.Tput.prototype.readTermcap)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>readTerminfo (term)](#apidoc.element.blessed.Tput.prototype.readTerminfo)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>setup ()](#apidoc.element.blessed.Tput.prototype.setup)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>term (is)](#apidoc.element.blessed.Tput.prototype.term)
1.  [function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>translateTermcap (info)](#apidoc.element.blessed.Tput.prototype.translateTermcap)
1.  object <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>utoa

#### [module blessed.ansiimage](#apidoc.module.blessed.ansiimage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>ansiimage (options)](#apidoc.element.blessed.ansiimage.ansiimage)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.</span>curl (url)](#apidoc.element.blessed.ansiimage.curl)

#### [module blessed.ansiimage.prototype](#apidoc.module.blessed.ansiimage.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>clearImage ()](#apidoc.element.blessed.ansiimage.prototype.clearImage)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>pause ()](#apidoc.element.blessed.ansiimage.prototype.pause)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>play ()](#apidoc.element.blessed.ansiimage.prototype.play)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>render ()](#apidoc.element.blessed.ansiimage.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>setImage (file)](#apidoc.element.blessed.ansiimage.prototype.setImage)
1.  [function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>stop ()](#apidoc.element.blessed.ansiimage.prototype.stop)
1.  string <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>type

#### [module blessed.bigtext](#apidoc.module.blessed.bigtext)
1.  [function <span class="apidocSignatureSpan">blessed.</span>bigtext (options)](#apidoc.element.blessed.bigtext.bigtext)

#### [module blessed.bigtext.prototype](#apidoc.module.blessed.bigtext.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>loadFont (filename)](#apidoc.element.blessed.bigtext.prototype.loadFont)
1.  [function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>render ()](#apidoc.element.blessed.bigtext.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>setContent (content)](#apidoc.element.blessed.bigtext.prototype.setContent)
1.  string <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>type

#### [module blessed.button](#apidoc.module.blessed.button)
1.  [function <span class="apidocSignatureSpan">blessed.</span>button (options)](#apidoc.element.blessed.button.button)

#### [module blessed.button.prototype](#apidoc.module.blessed.button.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.button.prototype.</span>press ()](#apidoc.element.blessed.button.prototype.press)
1.  string <span class="apidocSignatureSpan">blessed.button.prototype.</span>type

#### [module blessed.checkbox](#apidoc.module.blessed.checkbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>checkbox (options)](#apidoc.element.blessed.checkbox.checkbox)

#### [module blessed.checkbox.prototype](#apidoc.module.blessed.checkbox.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>check ()](#apidoc.element.blessed.checkbox.prototype.check)
1.  [function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>render ()](#apidoc.element.blessed.checkbox.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>toggle ()](#apidoc.element.blessed.checkbox.prototype.toggle)
1.  [function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>uncheck ()](#apidoc.element.blessed.checkbox.prototype.uncheck)
1.  string <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>type

#### [module blessed.colors](#apidoc.module.blessed.colors)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>RGBToHex (r, g, b)](#apidoc.element.blessed.colors.RGBToHex)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>blend (attr, attr2, alpha)](#apidoc.element.blessed.colors.blend)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>convert (color)](#apidoc.element.blessed.colors.convert)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>hexToRGB (hex)](#apidoc.element.blessed.colors.hexToRGB)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>match (r1, g1, b1)](#apidoc.element.blessed.colors.match)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>mixColors (c1, c2, alpha)](#apidoc.element.blessed.colors.mixColors)
1.  [function <span class="apidocSignatureSpan">blessed.colors.</span>reduce (color, total)](#apidoc.element.blessed.colors.reduce)
1.  object <span class="apidocSignatureSpan">blessed.</span>colors
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>_cache
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>ccolors
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>colorNames
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>ncolors
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>vcolors
1.  object <span class="apidocSignatureSpan">blessed.colors.</span>xterm

#### [module blessed.filemanager](#apidoc.module.blessed.filemanager)
1.  [function <span class="apidocSignatureSpan">blessed.</span>filemanager (options)](#apidoc.element.blessed.filemanager.filemanager)

#### [module blessed.filemanager.prototype](#apidoc.module.blessed.filemanager.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>pick (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.pick)
1.  [function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>refresh (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.refresh)
1.  [function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>reset (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.reset)
1.  string <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>type

#### [module blessed.form](#apidoc.module.blessed.form)
1.  [function <span class="apidocSignatureSpan">blessed.</span>form (options)](#apidoc.element.blessed.form.form)

#### [module blessed.form.prototype](#apidoc.module.blessed.form.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>_refresh ()](#apidoc.element.blessed.form.prototype._refresh)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>_visible ()](#apidoc.element.blessed.form.prototype._visible)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>cancel ()](#apidoc.element.blessed.form.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusFirst ()](#apidoc.element.blessed.form.prototype.focusFirst)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusLast ()](#apidoc.element.blessed.form.prototype.focusLast)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusNext ()](#apidoc.element.blessed.form.prototype.focusNext)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusPrevious ()](#apidoc.element.blessed.form.prototype.focusPrevious)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>next ()](#apidoc.element.blessed.form.prototype.next)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>previous ()](#apidoc.element.blessed.form.prototype.previous)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>reset ()](#apidoc.element.blessed.form.prototype.reset)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>resetSelected ()](#apidoc.element.blessed.form.prototype.resetSelected)
1.  [function <span class="apidocSignatureSpan">blessed.form.prototype.</span>submit ()](#apidoc.element.blessed.form.prototype.submit)
1.  string <span class="apidocSignatureSpan">blessed.form.prototype.</span>type

#### [module blessed.helpers](#apidoc.module.blessed.helpers)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>Element (options)](#apidoc.element.blessed.helpers.Element)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>Screen (options)](#apidoc.element.blessed.helpers.Screen)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>_element (options)](#apidoc.element.blessed.helpers._element)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>_screen (options)](#apidoc.element.blessed.helpers._screen)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>asort (obj)](#apidoc.element.blessed.helpers.asort)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>attrToBinary (style, element)](#apidoc.element.blessed.helpers.attrToBinary)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>cleanTags (text)](#apidoc.element.blessed.helpers.cleanTags)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>dropUnicode (text)](#apidoc.element.blessed.helpers.dropUnicode)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>escape (text)](#apidoc.element.blessed.helpers.escape)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>findFile (start, target)](#apidoc.element.blessed.helpers.findFile)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>generateTags (style, text)](#apidoc.element.blessed.helpers.generateTags)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>hsort (obj)](#apidoc.element.blessed.helpers.hsort)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>merge (a, b)](#apidoc.element.blessed.helpers.merge)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>parseTags (text, screen)](#apidoc.element.blessed.helpers.parseTags)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>sprintf (src)](#apidoc.element.blessed.helpers.sprintf)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>stripTags (text)](#apidoc.element.blessed.helpers.stripTags)
1.  [function <span class="apidocSignatureSpan">blessed.helpers.</span>tryRead (file)](#apidoc.element.blessed.helpers.tryRead)

#### [module blessed.layout](#apidoc.module.blessed.layout)
1.  [function <span class="apidocSignatureSpan">blessed.</span>layout (options)](#apidoc.element.blessed.layout.layout)

#### [module blessed.layout.prototype](#apidoc.module.blessed.layout.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>_renderCoords ()](#apidoc.element.blessed.layout.prototype._renderCoords)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>getLast (i)](#apidoc.element.blessed.layout.prototype.getLast)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>getLastCoords (i)](#apidoc.element.blessed.layout.prototype.getLastCoords)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>isRendered (el)](#apidoc.element.blessed.layout.prototype.isRendered)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>render ()](#apidoc.element.blessed.layout.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>renderer (coords)](#apidoc.element.blessed.layout.prototype.renderer)
1.  string <span class="apidocSignatureSpan">blessed.layout.prototype.</span>type

#### [module blessed.list](#apidoc.module.blessed.list)
1.  [function <span class="apidocSignatureSpan">blessed.</span>list (options)](#apidoc.element.blessed.list.list)

#### [module blessed.list.prototype](#apidoc.module.blessed.list.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>add (content)](#apidoc.element.blessed.list.prototype.add)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>addItem (content)](#apidoc.element.blessed.list.prototype.addItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>appendItem (content)](#apidoc.element.blessed.list.prototype.appendItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>cancelSelected (i)](#apidoc.element.blessed.list.prototype.cancelSelected)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>clearItems ()](#apidoc.element.blessed.list.prototype.clearItems)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>createItem (content)](#apidoc.element.blessed.list.prototype.createItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>down (offset)](#apidoc.element.blessed.list.prototype.down)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>enterSelected (i)](#apidoc.element.blessed.list.prototype.enterSelected)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>find (search, back)](#apidoc.element.blessed.list.prototype.find)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>fuzzyFind (search, back)](#apidoc.element.blessed.list.prototype.fuzzyFind)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>getItem (child)](#apidoc.element.blessed.list.prototype.getItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>getItemIndex (child)](#apidoc.element.blessed.list.prototype.getItemIndex)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>insertItem (child, content)](#apidoc.element.blessed.list.prototype.insertItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>move (offset)](#apidoc.element.blessed.list.prototype.move)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>pick (label, callback)](#apidoc.element.blessed.list.prototype.pick)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>popItem ()](#apidoc.element.blessed.list.prototype.popItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>pushItem (content)](#apidoc.element.blessed.list.prototype.pushItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>removeItem (child)](#apidoc.element.blessed.list.prototype.removeItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>select (index)](#apidoc.element.blessed.list.prototype.select)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>setItem (child, content)](#apidoc.element.blessed.list.prototype.setItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>setItems (items)](#apidoc.element.blessed.list.prototype.setItems)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>shiftItem ()](#apidoc.element.blessed.list.prototype.shiftItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>spliceItem (child, n)](#apidoc.element.blessed.list.prototype.spliceItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>unshiftItem (content)](#apidoc.element.blessed.list.prototype.unshiftItem)
1.  [function <span class="apidocSignatureSpan">blessed.list.prototype.</span>up (offset)](#apidoc.element.blessed.list.prototype.up)
1.  string <span class="apidocSignatureSpan">blessed.list.prototype.</span>type

#### [module blessed.listbar](#apidoc.module.blessed.listbar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>listbar (options)](#apidoc.element.blessed.listbar.listbar)

#### [module blessed.listbar.prototype](#apidoc.module.blessed.listbar.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>add (item, callback)](#apidoc.element.blessed.listbar.prototype.add)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>addItem (item, callback)](#apidoc.element.blessed.listbar.prototype.addItem)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>appendItem (item, callback)](#apidoc.element.blessed.listbar.prototype.appendItem)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>move (offset)](#apidoc.element.blessed.listbar.prototype.move)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>moveLeft (offset)](#apidoc.element.blessed.listbar.prototype.moveLeft)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>moveRight (offset)](#apidoc.element.blessed.listbar.prototype.moveRight)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>removeItem (child)](#apidoc.element.blessed.listbar.prototype.removeItem)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>render ()](#apidoc.element.blessed.listbar.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>select (offset)](#apidoc.element.blessed.listbar.prototype.select)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>selectTab (index)](#apidoc.element.blessed.listbar.prototype.selectTab)
1.  [function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>setItems (commands)](#apidoc.element.blessed.listbar.prototype.setItems)
1.  number <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>selected
1.  string <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>type

#### [module blessed.listtable](#apidoc.module.blessed.listtable)
1.  [function <span class="apidocSignatureSpan">blessed.</span>listtable (options)](#apidoc.element.blessed.listtable.listtable)

#### [module blessed.listtable.prototype](#apidoc.module.blessed.listtable.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>_calculateMaxes ()](#apidoc.element.blessed.listtable.prototype._calculateMaxes)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>_select (index)](#apidoc.element.blessed.listtable.prototype._select)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>render ()](#apidoc.element.blessed.listtable.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>select (i)](#apidoc.element.blessed.listtable.prototype.select)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>setData (rows)](#apidoc.element.blessed.listtable.prototype.setData)
1.  [function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>setRows (rows)](#apidoc.element.blessed.listtable.prototype.setRows)
1.  string <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>type

#### [module blessed.loading](#apidoc.module.blessed.loading)
1.  [function <span class="apidocSignatureSpan">blessed.</span>loading (options)](#apidoc.element.blessed.loading.loading)

#### [module blessed.loading.prototype](#apidoc.module.blessed.loading.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.loading.prototype.</span>load (text)](#apidoc.element.blessed.loading.prototype.load)
1.  [function <span class="apidocSignatureSpan">blessed.loading.prototype.</span>stop ()](#apidoc.element.blessed.loading.prototype.stop)
1.  string <span class="apidocSignatureSpan">blessed.loading.prototype.</span>type

#### [module blessed.log](#apidoc.module.blessed.log)
1.  [function <span class="apidocSignatureSpan">blessed.</span>log (options)](#apidoc.element.blessed.log.log)

#### [module blessed.log.prototype](#apidoc.module.blessed.log.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.log.prototype.</span>_scroll (offset, always)](#apidoc.element.blessed.log.prototype._scroll)
1.  [function <span class="apidocSignatureSpan">blessed.log.prototype.</span>add ()](#apidoc.element.blessed.log.prototype.add)
1.  [function <span class="apidocSignatureSpan">blessed.log.prototype.</span>log ()](#apidoc.element.blessed.log.prototype.log)
1.  [function <span class="apidocSignatureSpan">blessed.log.prototype.</span>scroll (offset, always)](#apidoc.element.blessed.log.prototype.scroll)
1.  string <span class="apidocSignatureSpan">blessed.log.prototype.</span>type

#### [module blessed.message](#apidoc.module.blessed.message)
1.  [function <span class="apidocSignatureSpan">blessed.</span>message (options)](#apidoc.element.blessed.message.message)

#### [module blessed.message.prototype](#apidoc.module.blessed.message.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.message.prototype.</span>display (text, time, callback)](#apidoc.element.blessed.message.prototype.display)
1.  [function <span class="apidocSignatureSpan">blessed.message.prototype.</span>error (text, time, callback)](#apidoc.element.blessed.message.prototype.error)
1.  [function <span class="apidocSignatureSpan">blessed.message.prototype.</span>log (text, time, callback)](#apidoc.element.blessed.message.prototype.log)
1.  string <span class="apidocSignatureSpan">blessed.message.prototype.</span>type

#### [module blessed.node](#apidoc.module.blessed.node)
1.  [function <span class="apidocSignatureSpan">blessed.</span>node (options)](#apidoc.element.blessed.node.node)
1.  number <span class="apidocSignatureSpan">blessed.node.</span>uid

#### [module blessed.node.prototype](#apidoc.module.blessed.node.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>append (element)](#apidoc.element.blessed.node.prototype.append)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>collectAncestors (s)](#apidoc.element.blessed.node.prototype.collectAncestors)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>collectDescendants (s)](#apidoc.element.blessed.node.prototype.collectDescendants)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>destroy ()](#apidoc.element.blessed.node.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>detach ()](#apidoc.element.blessed.node.prototype.detach)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>emitAncestors ()](#apidoc.element.blessed.node.prototype.emitAncestors)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>emitDescendants ()](#apidoc.element.blessed.node.prototype.emitDescendants)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>forAncestors (iter, s)](#apidoc.element.blessed.node.prototype.forAncestors)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>forDescendants (iter, s)](#apidoc.element.blessed.node.prototype.forDescendants)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>free ()](#apidoc.element.blessed.node.prototype.free)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>get (name, value)](#apidoc.element.blessed.node.prototype.get)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>hasAncestor (target)](#apidoc.element.blessed.node.prototype.hasAncestor)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>hasDescendant (target)](#apidoc.element.blessed.node.prototype.hasDescendant)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insert (element, i)](#apidoc.element.blessed.node.prototype.insert)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insertAfter (element, other)](#apidoc.element.blessed.node.prototype.insertAfter)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insertBefore (element, other)](#apidoc.element.blessed.node.prototype.insertBefore)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>prepend (element)](#apidoc.element.blessed.node.prototype.prepend)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>remove (element)](#apidoc.element.blessed.node.prototype.remove)
1.  [function <span class="apidocSignatureSpan">blessed.node.prototype.</span>set (name, value)](#apidoc.element.blessed.node.prototype.set)
1.  string <span class="apidocSignatureSpan">blessed.node.prototype.</span>type

#### [module blessed.overlayimage](#apidoc.module.blessed.overlayimage)
1.  [function <span class="apidocSignatureSpan">blessed.</span>overlayimage (options)](#apidoc.element.blessed.overlayimage.overlayimage)
1.  string <span class="apidocSignatureSpan">blessed.overlayimage.</span>w3mdisplay

#### [module blessed.overlayimage.prototype](#apidoc.module.blessed.overlayimage.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>clearImage (callback)](#apidoc.element.blessed.overlayimage.prototype.clearImage)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>clearImageSync ()](#apidoc.element.blessed.overlayimage.prototype.clearImageSync)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>displayImage (callback)](#apidoc.element.blessed.overlayimage.prototype.displayImage)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>getPixelRatio (callback)](#apidoc.element.blessed.overlayimage.prototype.getPixelRatio)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>getPixelRatioSync ()](#apidoc.element.blessed.overlayimage.prototype.getPixelRatioSync)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>imageSize (callback)](#apidoc.element.blessed.overlayimage.prototype.imageSize)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>imageSizeSync ()](#apidoc.element.blessed.overlayimage.prototype.imageSizeSync)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>renderImage (img, ratio, callback)](#apidoc.element.blessed.overlayimage.prototype.renderImage)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>renderImageSync (img, ratio)](#apidoc.element.blessed.overlayimage.prototype.renderImageSync)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>setImage (img, callback)](#apidoc.element.blessed.overlayimage.prototype.setImage)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>spawn (file, args, opt, callback)](#apidoc.element.blessed.overlayimage.prototype.spawn)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>termSize (callback)](#apidoc.element.blessed.overlayimage.prototype.termSize)
1.  [function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>termSizeSync (_, recurse)](#apidoc.element.blessed.overlayimage.prototype.termSizeSync)
1.  string <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>type

#### [module blessed.progressbar](#apidoc.module.blessed.progressbar)
1.  [function <span class="apidocSignatureSpan">blessed.</span>progressbar (options)](#apidoc.element.blessed.progressbar.progressbar)

#### [module blessed.progressbar.prototype](#apidoc.module.blessed.progressbar.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>progress (filled)](#apidoc.element.blessed.progressbar.prototype.progress)
1.  [function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>render ()](#apidoc.element.blessed.progressbar.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>reset ()](#apidoc.element.blessed.progressbar.prototype.reset)
1.  [function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>setProgress (filled)](#apidoc.element.blessed.progressbar.prototype.setProgress)
1.  string <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>type

#### [module blessed.prompt](#apidoc.module.blessed.prompt)
1.  [function <span class="apidocSignatureSpan">blessed.</span>prompt (options)](#apidoc.element.blessed.prompt.prompt)

#### [module blessed.prompt.prototype](#apidoc.module.blessed.prompt.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>input (text, value, callback)](#apidoc.element.blessed.prompt.prototype.input)
1.  [function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>readInput (text, value, callback)](#apidoc.element.blessed.prompt.prototype.readInput)
1.  [function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>setInput (text, value, callback)](#apidoc.element.blessed.prompt.prototype.setInput)
1.  string <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>type

#### [module blessed.question](#apidoc.module.blessed.question)
1.  [function <span class="apidocSignatureSpan">blessed.</span>question (options)](#apidoc.element.blessed.question.question)

#### [module blessed.question.prototype](#apidoc.module.blessed.question.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.question.prototype.</span>ask (text, callback)](#apidoc.element.blessed.question.prototype.ask)
1.  string <span class="apidocSignatureSpan">blessed.question.prototype.</span>type

#### [module blessed.radiobutton](#apidoc.module.blessed.radiobutton)
1.  [function <span class="apidocSignatureSpan">blessed.</span>radiobutton (options)](#apidoc.element.blessed.radiobutton.radiobutton)

#### [module blessed.radiobutton.prototype](#apidoc.module.blessed.radiobutton.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.radiobutton.prototype.</span>render ()](#apidoc.element.blessed.radiobutton.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.radiobutton.prototype.</span>toggle ()](#apidoc.element.blessed.radiobutton.prototype.toggle)
1.  string <span class="apidocSignatureSpan">blessed.radiobutton.prototype.</span>type

#### [module blessed.scrollablebox](#apidoc.module.blessed.scrollablebox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>scrollablebox (options)](#apidoc.element.blessed.scrollablebox.scrollablebox)

#### [module blessed.scrollablebox.prototype](#apidoc.module.blessed.scrollablebox.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>_recalculateIndex ()](#apidoc.element.blessed.scrollablebox.prototype._recalculateIndex)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>_scrollBottom ()](#apidoc.element.blessed.scrollablebox.prototype._scrollBottom)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScroll ()](#apidoc.element.blessed.scrollablebox.prototype.getScroll)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScrollHeight ()](#apidoc.element.blessed.scrollablebox.prototype.getScrollHeight)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScrollPerc (s)](#apidoc.element.blessed.scrollablebox.prototype.getScrollPerc)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>resetScroll ()](#apidoc.element.blessed.scrollablebox.prototype.resetScroll)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>scroll (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.scroll)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>scrollTo (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.scrollTo)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>setScroll (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.setScroll)
1.  [function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>setScrollPerc (i)](#apidoc.element.blessed.scrollablebox.prototype.setScrollPerc)
1.  string <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>type

#### [module blessed.table](#apidoc.module.blessed.table)
1.  [function <span class="apidocSignatureSpan">blessed.</span>table (options)](#apidoc.element.blessed.table.table)

#### [module blessed.table.prototype](#apidoc.module.blessed.table.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.table.prototype.</span>_calculateMaxes ()](#apidoc.element.blessed.table.prototype._calculateMaxes)
1.  [function <span class="apidocSignatureSpan">blessed.table.prototype.</span>render ()](#apidoc.element.blessed.table.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.table.prototype.</span>setData (rows)](#apidoc.element.blessed.table.prototype.setData)
1.  [function <span class="apidocSignatureSpan">blessed.table.prototype.</span>setRows (rows)](#apidoc.element.blessed.table.prototype.setRows)
1.  string <span class="apidocSignatureSpan">blessed.table.prototype.</span>type

#### [module blessed.terminal](#apidoc.module.blessed.terminal)
1.  [function <span class="apidocSignatureSpan">blessed.</span>terminal (options)](#apidoc.element.blessed.terminal.terminal)

#### [module blessed.terminal.prototype](#apidoc.module.blessed.terminal.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>_isMouse (buf)](#apidoc.element.blessed.terminal.prototype._isMouse)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>bootstrap ()](#apidoc.element.blessed.terminal.prototype.bootstrap)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScroll ()](#apidoc.element.blessed.terminal.prototype.getScroll)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScrollHeight ()](#apidoc.element.blessed.terminal.prototype.getScrollHeight)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScrollPerc ()](#apidoc.element.blessed.terminal.prototype.getScrollPerc)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>kill ()](#apidoc.element.blessed.terminal.prototype.kill)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>render ()](#apidoc.element.blessed.terminal.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>resetScroll ()](#apidoc.element.blessed.terminal.prototype.resetScroll)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>screenshot (xi, xl, yi, yl)](#apidoc.element.blessed.terminal.prototype.screenshot)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>scroll (offset)](#apidoc.element.blessed.terminal.prototype.scroll)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>scrollTo (offset)](#apidoc.element.blessed.terminal.prototype.scrollTo)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>setScroll (offset)](#apidoc.element.blessed.terminal.prototype.setScroll)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>setScrollPerc (i)](#apidoc.element.blessed.terminal.prototype.setScrollPerc)
1.  [function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>write (data)](#apidoc.element.blessed.terminal.prototype.write)
1.  string <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>type

#### [module blessed.textarea](#apidoc.module.blessed.textarea)
1.  [function <span class="apidocSignatureSpan">blessed.</span>textarea (options)](#apidoc.element.blessed.textarea.textarea)

#### [module blessed.textarea.prototype](#apidoc.module.blessed.textarea.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_listener (ch, key)](#apidoc.element.blessed.textarea.prototype._listener)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_typeScroll ()](#apidoc.element.blessed.textarea.prototype._typeScroll)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_updateCursor (get)](#apidoc.element.blessed.textarea.prototype._updateCursor)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>cancel ()](#apidoc.element.blessed.textarea.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>clearInput ()](#apidoc.element.blessed.textarea.prototype.clearInput)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>clearValue ()](#apidoc.element.blessed.textarea.prototype.clearValue)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>editor (callback)](#apidoc.element.blessed.textarea.prototype.editor)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>getValue ()](#apidoc.element.blessed.textarea.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>input (callback)](#apidoc.element.blessed.textarea.prototype.input)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>readEditor (callback)](#apidoc.element.blessed.textarea.prototype.readEditor)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>readInput (callback)](#apidoc.element.blessed.textarea.prototype.readInput)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>render ()](#apidoc.element.blessed.textarea.prototype.render)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setEditor (callback)](#apidoc.element.blessed.textarea.prototype.setEditor)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setInput (callback)](#apidoc.element.blessed.textarea.prototype.setInput)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setValue (value)](#apidoc.element.blessed.textarea.prototype.setValue)
1.  [function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>submit ()](#apidoc.element.blessed.textarea.prototype.submit)
1.  string <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>type

#### [module blessed.textbox](#apidoc.module.blessed.textbox)
1.  [function <span class="apidocSignatureSpan">blessed.</span>textbox (options)](#apidoc.element.blessed.textbox.textbox)

#### [module blessed.textbox.prototype](#apidoc.module.blessed.textbox.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>__olistener (ch, key)](#apidoc.element.blessed.textbox.prototype.__olistener)
1.  [function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>_listener (ch, key)](#apidoc.element.blessed.textbox.prototype._listener)
1.  [function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>setValue (value)](#apidoc.element.blessed.textbox.prototype.setValue)
1.  [function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>submit ()](#apidoc.element.blessed.textbox.prototype.submit)
1.  string <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>type

#### [module blessed.unicode](#apidoc.module.blessed.unicode)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>charWidth (str, i)](#apidoc.element.blessed.unicode.charWidth)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>codePointAt (str, position)](#apidoc.element.blessed.unicode.codePointAt)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>fromCodePoint ()](#apidoc.element.blessed.unicode.fromCodePoint)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>isCombining (str, i)](#apidoc.element.blessed.unicode.isCombining)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>isSurrogate (str, i)](#apidoc.element.blessed.unicode.isSurrogate)
1.  [function <span class="apidocSignatureSpan">blessed.unicode.</span>strWidth (str)](#apidoc.element.blessed.unicode.strWidth)
1.  object <span class="apidocSignatureSpan">blessed.unicode.</span>chars
1.  object <span class="apidocSignatureSpan">blessed.unicode.</span>combining
1.  object <span class="apidocSignatureSpan">blessed.unicode.</span>combiningTable

#### [module blessed.video](#apidoc.module.blessed.video)
1.  [function <span class="apidocSignatureSpan">blessed.</span>video (options)](#apidoc.element.blessed.video.video)

#### [module blessed.video.prototype](#apidoc.module.blessed.video.prototype)
1.  [function <span class="apidocSignatureSpan">blessed.video.prototype.</span>exists (program)](#apidoc.element.blessed.video.prototype.exists)
1.  string <span class="apidocSignatureSpan">blessed.video.prototype.</span>type

#### [module blessed.widget](#apidoc.module.blessed.widget)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ANSIImage (options)](#apidoc.element.blessed.widget.ANSIImage)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>BigText (options)](#apidoc.element.blessed.widget.BigText)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Box (options)](#apidoc.element.blessed.widget.Box)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Button (options)](#apidoc.element.blessed.widget.Button)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Checkbox (options)](#apidoc.element.blessed.widget.Checkbox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Element (options)](#apidoc.element.blessed.widget.Element)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>FileManager (options)](#apidoc.element.blessed.widget.FileManager)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Form (options)](#apidoc.element.blessed.widget.Form)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Image (options)](#apidoc.element.blessed.widget.Image)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Input (options)](#apidoc.element.blessed.widget.Input)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Layout (options)](#apidoc.element.blessed.widget.Layout)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Line (options)](#apidoc.element.blessed.widget.Line)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>List (options)](#apidoc.element.blessed.widget.List)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ListBar (options)](#apidoc.element.blessed.widget.ListBar)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ListTable (options)](#apidoc.element.blessed.widget.ListTable)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Listbar (options)](#apidoc.element.blessed.widget.Listbar)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Loading (options)](#apidoc.element.blessed.widget.Loading)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Log (options)](#apidoc.element.blessed.widget.Log)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Message (options)](#apidoc.element.blessed.widget.Message)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Node (options)](#apidoc.element.blessed.widget.Node)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>OverlayImage (options)](#apidoc.element.blessed.widget.OverlayImage)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>PNG (options)](#apidoc.element.blessed.widget.PNG)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ProgressBar (options)](#apidoc.element.blessed.widget.ProgressBar)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Prompt (options)](#apidoc.element.blessed.widget.Prompt)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Question (options)](#apidoc.element.blessed.widget.Question)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>RadioButton (options)](#apidoc.element.blessed.widget.RadioButton)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>RadioSet (options)](#apidoc.element.blessed.widget.RadioSet)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Screen (options)](#apidoc.element.blessed.widget.Screen)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ScrollableBox (options)](#apidoc.element.blessed.widget.ScrollableBox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ScrollableText (options)](#apidoc.element.blessed.widget.ScrollableText)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Table (options)](#apidoc.element.blessed.widget.Table)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Terminal (options)](#apidoc.element.blessed.widget.Terminal)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Text (options)](#apidoc.element.blessed.widget.Text)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Textarea (options)](#apidoc.element.blessed.widget.Textarea)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Textbox (options)](#apidoc.element.blessed.widget.Textbox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>Video (options)](#apidoc.element.blessed.widget.Video)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>ansiimage (options)](#apidoc.element.blessed.widget.ansiimage)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>bigtext (options)](#apidoc.element.blessed.widget.bigtext)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>box (options)](#apidoc.element.blessed.widget.box)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>button (options)](#apidoc.element.blessed.widget.button)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>checkbox (options)](#apidoc.element.blessed.widget.checkbox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>element (options)](#apidoc.element.blessed.widget.element)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>filemanager (options)](#apidoc.element.blessed.widget.filemanager)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>form (options)](#apidoc.element.blessed.widget.form)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>image (options)](#apidoc.element.blessed.widget.image)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>input (options)](#apidoc.element.blessed.widget.input)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>layout (options)](#apidoc.element.blessed.widget.layout)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>line (options)](#apidoc.element.blessed.widget.line)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>list (options)](#apidoc.element.blessed.widget.list)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>listbar (options)](#apidoc.element.blessed.widget.listbar)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>listtable (options)](#apidoc.element.blessed.widget.listtable)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>loading (options)](#apidoc.element.blessed.widget.loading)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>log (options)](#apidoc.element.blessed.widget.log)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>message (options)](#apidoc.element.blessed.widget.message)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>node (options)](#apidoc.element.blessed.widget.node)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>overlayimage (options)](#apidoc.element.blessed.widget.overlayimage)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>png (options)](#apidoc.element.blessed.widget.png)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>progressbar (options)](#apidoc.element.blessed.widget.progressbar)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>prompt (options)](#apidoc.element.blessed.widget.prompt)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>question (options)](#apidoc.element.blessed.widget.question)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>radiobutton (options)](#apidoc.element.blessed.widget.radiobutton)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>radioset (options)](#apidoc.element.blessed.widget.radioset)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>screen (options)](#apidoc.element.blessed.widget.screen)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>scrollablebox (options)](#apidoc.element.blessed.widget.scrollablebox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>scrollabletext (options)](#apidoc.element.blessed.widget.scrollabletext)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>table (options)](#apidoc.element.blessed.widget.table)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>terminal (options)](#apidoc.element.blessed.widget.terminal)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>text (options)](#apidoc.element.blessed.widget.text)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>textarea (options)](#apidoc.element.blessed.widget.textarea)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>textbox (options)](#apidoc.element.blessed.widget.textbox)
1.  [function <span class="apidocSignatureSpan">blessed.widget.</span>video (options)](#apidoc.element.blessed.widget.video)
1.  object <span class="apidocSignatureSpan">blessed.widget.</span>aliases
1.  object <span class="apidocSignatureSpan">blessed.widget.</span>classes



# <a name="apidoc.module.blessed"></a>[module blessed](#apidoc.module.blessed)

#### <a name="apidoc.element.blessed.blessed"></a>[function <span class="apidocSignatureSpan"></span>blessed ()](#apidoc.element.blessed.blessed)
- description and source-code
```javascript
function blessed() {
  return blessed.program.apply(null, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ANSIImage"></a>[function <span class="apidocSignatureSpan">blessed.</span>ANSIImage (options)](#apidoc.element.blessed.ANSIImage)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.BigText"></a>[function <span class="apidocSignatureSpan">blessed.</span>BigText (options)](#apidoc.element.blessed.BigText)
- description and source-code
```javascript
function BigText(options) {
  if (!(this instanceof Node)) {
    return new BigText(options);
  }
  options = options || {};
  options.font = options.font
    || __dirname + '/../../usr/fonts/ter-u14n.json';
  options.fontBold = options.font
    || __dirname + '/../../usr/fonts/ter-u14b.json';
  this.fch = options.fch;
  this.ratio = {};
  this.font = this.loadFont(options.font);
  this.fontBold = this.loadFont(options.font);
  Box.call(this, options);
  if (this.style.bold) {
    this.font = this.fontBold;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Box"></a>[function <span class="apidocSignatureSpan">blessed.</span>Box (options)](#apidoc.element.blessed.Box)
- description and source-code
```javascript
function Box(options) {
  if (!(this instanceof Node)) {
    return new Box(options);
  }
  options = options || {};
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Button"></a>[function <span class="apidocSignatureSpan">blessed.</span>Button (options)](#apidoc.element.blessed.Button)
- description and source-code
```javascript
function Button(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Button(options);
  }

  options = options || {};

  if (options.autoFocus == null) {
    options.autoFocus = false;
  }

  Input.call(this, options);

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      return self.press();
    }
  });

  if (this.options.mouse) {
    this.on('click', function() {
      return self.press();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Checkbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>Checkbox (options)](#apidoc.element.blessed.Checkbox)
- description and source-code
```javascript
function Checkbox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Checkbox(options);
  }

  options = options || {};

  Input.call(this, options);

  this.text = options.content || options.text || '';
  this.checked = this.value = options.checked || false;

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      self.toggle();
      self.screen.render();
    }
  });

  if (options.mouse) {
    this.on('click', function() {
      self.toggle();
      self.screen.render();
    });
  }

  this.on('focus', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    self.screen.program.lsaveCursor('checkbox');
    self.screen.program.cup(lpos.yi, lpos.xi + 1);
    self.screen.program.showCursor();
  });

  this.on('blur', function() {
    self.screen.program.lrestoreCursor('checkbox', true);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element"></a>[function <span class="apidocSignatureSpan">blessed.</span>Element (options)](#apidoc.element.blessed.Element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.FileManager"></a>[function <span class="apidocSignatureSpan">blessed.</span>FileManager (options)](#apidoc.element.blessed.FileManager)
- description and source-code
```javascript
function FileManager(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new FileManager(options);
  }

  options = options || {};
  options.parseTags = true;
  // options.label = ' {blue-fg}%path{/blue-fg} ';

  List.call(this, options);

  this.cwd = options.cwd || process.cwd();
  this.file = this.cwd;
  this.value = this.cwd;

  if (options.label && ~options.label.indexOf('%path')) {
    this._label.setContent(options.label.replace('%path', this.cwd));
  }

  this.on('select', function(item) {
    var value = item.content.replace(/\{[^{}]+\}/g, '').replace(/@$/, '')
      , file = path.resolve(self.cwd, value);

    return fs.stat(file, function(err, stat) {
      if (err) {
        return self.emit('error', err, file);
      }
      self.file = file;
      self.value = file;
      if (stat.isDirectory()) {
        self.emit('cd', file, self.cwd);
        self.cwd = file;
        if (options.label && ~options.label.indexOf('%path')) {
          self._label.setContent(options.label.replace('%path', file));
        }
        self.refresh();
      } else {
        self.emit('file', file);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Form"></a>[function <span class="apidocSignatureSpan">blessed.</span>Form (options)](#apidoc.element.blessed.Form)
- description and source-code
```javascript
function Form(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Form(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  Box.call(this, options);

  if (options.keys) {
    this.screen._listenKeys(this);
    this.on('element keypress', function(el, ch, key) {
      if ((key.name === 'tab' && !key.shift)
          || (el.type === 'textbox' && options.autoNext && key.name === 'enter')
          || key.name === 'down'
          || (options.vi && key.name === 'j')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'j') return;
          if (key.name === 'tab') {
            // Workaround, since we can't stop the tab from being added.
            el.emit('keypress', null, { name: 'backspace' });
          }
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusNext();
        return;
      }

      if ((key.name === 'tab' && key.shift)
          || key.name === 'up'
          || (options.vi && key.name === 'k')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'k') return;
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusPrevious();
        return;
      }

      if (key.name === 'escape') {
        self.focus();
        return;
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Image"></a>[function <span class="apidocSignatureSpan">blessed.</span>Image (options)](#apidoc.element.blessed.Image)
- description and source-code
```javascript
function Image(options) {
  if (!(this instanceof Node)) {
    return new Image(options);
  }

  options = options || {};
  options.type = options.itype || options.type || 'ansi';

  Box.call(this, options);

  if (options.type === 'ansi' && this.type !== 'ansiimage') {
    var ANSIImage = require('./ansiimage');
    Object.getOwnPropertyNames(ANSIImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ANSIImage.prototype, key));
    }, this);
    ANSIImage.call(this, options);
    return this;
  }

  if (options.type === 'overlay' && this.type !== 'overlayimage') {
    var OverlayImage = require('./overlayimage');
    Object.getOwnPropertyNames(OverlayImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(OverlayImage.prototype, key));
    }, this);
    OverlayImage.call(this, options);
    return this;
  }

  throw new Error(''type' must either be 'ansi' or 'overlay'.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Input"></a>[function <span class="apidocSignatureSpan">blessed.</span>Input (options)](#apidoc.element.blessed.Input)
- description and source-code
```javascript
function Input(options) {
  if (!(this instanceof Node)) {
    return new Input(options);
  }
  options = options || {};
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Layout"></a>[function <span class="apidocSignatureSpan">blessed.</span>Layout (options)](#apidoc.element.blessed.Layout)
- description and source-code
```javascript
function Layout(options) {
  if (!(this instanceof Node)) {
    return new Layout(options);
  }

  options = options || {};

  if ((options.width == null
      && (options.left == null && options.right == null))
      || (options.height == null
      && (options.top == null && options.bottom == null))) {
    throw new Error(''Layout' must have a width and height!');
  }

  options.layout = options.layout || 'inline';

  Element.call(this, options);

  if (options.renderer) {
    this.renderer = options.renderer;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Line"></a>[function <span class="apidocSignatureSpan">blessed.</span>Line (options)](#apidoc.element.blessed.Line)
- description and source-code
```javascript
function Line(options) {
  if (!(this instanceof Node)) {
    return new Line(options);
  }

  options = options || {};

  var orientation = options.orientation || 'vertical';
  delete options.orientation;

  if (orientation === 'vertical') {
    options.width = 1;
  } else {
    options.height = 1;
  }

  Box.call(this, options);

  this.ch = !options.type || options.type === 'line'
    ? orientation === 'horizontal' ? '─' : '│'
    : options.ch || ' ';

  this.border = {
    type: 'bg',
    __proto__: this
  };

  this.style.border = this.style;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.List"></a>[function <span class="apidocSignatureSpan">blessed.</span>List (options)](#apidoc.element.blessed.List)
- description and source-code
```javascript
function List(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new List(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  // Possibly put this here: this.items = [];
  options.scrollable = true;
  Box.call(this, options);

  this.value = '';
  this.items = [];
  this.ritems = [];
  this.selected = 0;
  this._isList = true;

  if (!this.style.selected) {
    this.style.selected = {};
    this.style.selected.bg = options.selectedBg;
    this.style.selected.fg = options.selectedFg;
    this.style.selected.bold = options.selectedBold;
    this.style.selected.underline = options.selectedUnderline;
    this.style.selected.blink = options.selectedBlink;
    this.style.selected.inverse = options.selectedInverse;
    this.style.selected.invisible = options.selectedInvisible;
  }

  if (!this.style.item) {
    this.style.item = {};
    this.style.item.bg = options.itemBg;
    this.style.item.fg = options.itemFg;
    this.style.item.bold = options.itemBold;
    this.style.item.underline = options.itemUnderline;
    this.style.item.blink = options.itemBlink;
    this.style.item.inverse = options.itemInverse;
    this.style.item.invisible = options.itemInvisible;
  }

  // Legacy: for apps written before the addition of item attributes.
  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    if (self.style[name] != null && self.style.item[name] == null) {
      self.style.item[name] = self.style[name];
    }
  });

  if (this.options.itemHoverBg) {
    this.options.itemHoverEffects = { bg: this.options.itemHoverBg };
  }

  if (this.options.itemHoverEffects) {
    this.style.item.hover = this.options.itemHoverEffects;
  }

  if (this.options.itemFocusEffects) {
    this.style.item.focus = this.options.itemFocusEffects;
  }

  this.interactive = options.interactive !== false;

  this.mouse = options.mouse || false;

  if (options.items) {
    this.ritems = options.items;
    options.items.forEach(this.add.bind(this));
  }

  this.select(0);

  if (options.mouse) {
    this.screen._listenMouse(this);
    this.on('element wheeldown', function() {
      self.select(self.selected + 2);
      self.screen.render();
    });
    this.on('element wheelup', function() {
      self.select(self.selected - 2);
      self.screen.render();
    });
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.up();
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.down();
        self.screen.render();
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'l' && !key.shift)) {
        self.enterSelected();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.cancelSelected();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.move(-((self.height - self.iheight) / 2) | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.move((self.height - self.iheight) / 2 | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'b' && key.ctrl) {
        self.move(-(self.height - self.iheight));
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'f' && key.ctrl) {
        self.move(self.height - self.iheight);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'h' && key.shift) {
        self.move(self.childBase - self.selected);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'm' && key.shift) {
        // TODO: Maybe use Math.min(this.items.length,
        // ... for calculating visible items elsewhere.
        var visible = Math.min(
          self.height - self.iheight,
          self.items.length) / 2 | 0;
        self.move(sel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ListBar"></a>[function <span class="apidocSignatureSpan">blessed.</span>ListBar (options)](#apidoc.element.blessed.ListBar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ListTable"></a>[function <span class="apidocSignatureSpan">blessed.</span>ListTable (options)](#apidoc.element.blessed.ListTable)
- description and source-code
```javascript
function ListTable(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ListTable(options);
  }

  options = options || {};
  options.shrink = true;
  options.normalShrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  this.__align = options.align || 'center';
  delete options.align;

  options.style.selected = options.style.cell.selected;
  options.style.item = options.style.cell;

  List.call(this, options);

  this._header = new Box({
    parent: this,
    left: this.screen.autoPadding ? 0 : this.ileft,
    top: 0,
    width: 'shrink',
    height: 1,
    style: options.style.header,
    tags: options.parseTags || options.tags
  });

  this.on('scroll', function() {
    self._header.setFront();
    self._header.rtop = self.childBase;
    if (!self.screen.autoPadding) {
      self._header.rtop = self.childBase + (self.border ? 1 : 0);
    }
  });

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setData(self.rows);
  });

  this.on('resize', function() {
    var selected = self.selected;
    self.setData(self.rows);
    self.select(selected);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Listbar"></a>[function <span class="apidocSignatureSpan">blessed.</span>Listbar (options)](#apidoc.element.blessed.Listbar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Loading"></a>[function <span class="apidocSignatureSpan">blessed.</span>Loading (options)](#apidoc.element.blessed.Loading)
- description and source-code
```javascript
function Loading(options) {
  if (!(this instanceof Node)) {
    return new Loading(options);
  }

  options = options || {};

  Box.call(this, options);

  this._.icon = new Text({
    parent: this,
    align: 'center',
    top: 2,
    left: 1,
    right: 1,
    height: 1,
    content: '|'
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Log"></a>[function <span class="apidocSignatureSpan">blessed.</span>Log (options)](#apidoc.element.blessed.Log)
- description and source-code
```javascript
function Log(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Log(options);
  }

  options = options || {};

  ScrollableText.call(this, options);

  this.scrollback = options.scrollback != null
    ? options.scrollback
    : Infinity;
  this.scrollOnInput = options.scrollOnInput;

  this.on('set content', function() {
    if (!self._userScrolled || self.scrollOnInput) {
      nextTick(function() {
        self.setScrollPerc(100);
        self._userScrolled = false;
        self.screen.render();
      });
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Message"></a>[function <span class="apidocSignatureSpan">blessed.</span>Message (options)](#apidoc.element.blessed.Message)
- description and source-code
```javascript
function Message(options) {
  if (!(this instanceof Node)) {
    return new Message(options);
  }

  options = options || {};
  options.tags = true;

  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Node"></a>[function <span class="apidocSignatureSpan">blessed.</span>Node (options)](#apidoc.element.blessed.Node)
- description and source-code
```javascript
function Node(options) {
  var self = this;
  var Screen = require('./screen');

  if (!(this instanceof Node)) {
    return new Node(options);
  }

  EventEmitter.call(this);

  options = options || {};
  this.options = options;

  this.screen = this.screen || options.screen;

  if (!this.screen) {
    if (this.type === 'screen') {
      this.screen = this;
    } else if (Screen.total === 1) {
      this.screen = Screen.global;
    } else if (options.parent) {
      this.screen = options.parent;
      while (this.screen && this.screen.type !== 'screen') {
        this.screen = this.screen.parent;
      }
    } else if (Screen.total) {
      // This _should_ work in most cases as long as the element is appended
      // synchronously after the screen's creation. Throw error if not.
      this.screen = Screen.instances[Screen.instances.length - 1];
      process.nextTick(function() {
        if (!self.parent) {
          throw new Error('Element (' + self.type + ')'
            + ' was not appended synchronously after the'
            + ' screen\'s creation. Please set a 'parent''
            + ' or 'screen' option in the element\'s constructor'
            + ' if you are going to use multiple screens and'
            + ' append the element later.');
        }
      });
    } else {
      throw new Error('No active screen.');
    }
  }

  this.parent = options.parent || null;
  this.children = [];
  this.$ = this._ = this.data = {};
  this.uid = Node.uid++;
  this.index = this.index != null ? this.index : -1;

  if (this.type !== 'screen') {
    this.detached = true;
  }

  if (this.parent) {
    this.parent.append(this);
  }

  (options.children || []).forEach(this.append.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.OverlayImage"></a>[function <span class="apidocSignatureSpan">blessed.</span>OverlayImage (options)](#apidoc.element.blessed.OverlayImage)
- description and source-code
```javascript
function OverlayImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new OverlayImage(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.w3m) {
    OverlayImage.w3mdisplay = options.w3m;
  }

  if (OverlayImage.hasW3MDisplay == null) {
    if (fs.existsSync(OverlayImage.w3mdisplay)) {
      OverlayImage.hasW3MDisplay = true;
    } else if (options.search !== false) {
      var file = helpers.findFile('/usr', 'w3mimgdisplay')
              || helpers.findFile('/lib', 'w3mimgdisplay')
              || helpers.findFile('/bin', 'w3mimgdisplay');
      if (file) {
        OverlayImage.hasW3MDisplay = true;
        OverlayImage.w3mdisplay = file;
      } else {
        OverlayImage.hasW3MDisplay = false;
      }
    }
  }

  this.on('hide', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('show', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.on('detach', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('attach', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.onScreenEvent('resize', function() {
    self._needsRatio = true;
  });

  // Get images to overlap properly. Maybe not worth it:
  // this.onScreenEvent('render', function() {
  //   self.screen.program.flush();
  //   if (!self._noImage) return;
  //   function display(el, next) {
  //     if (el.type === 'w3mimage' && el.file) {
  //       el.setImage(el.file, next);
  //     } else {
  //       next();
  //     }
  //   }
  //   function done(el) {
  //     el.children.forEach(recurse);
  //   }
  //   function recurse(el) {
  //     display(el, function() {
  //       var pending = el.children.length;
  //       el.children.forEach(function(el) {
  //         display(el, function() {
  //           if (!--pending) done(el);
  //         });
  //       });
  //     });
  //   }
  //   recurse(self.screen);
  // });

  this.onScreenEvent('render', function() {
    self.screen.program.flush();
    if (!self._noImage) {
      self.setImage(self.file);
    }
  });

  if (this.options.file || this.options.img) {
    this.setImage(this.options.file || this.options.img);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.PNG"></a>[function <span class="apidocSignatureSpan">blessed.</span>PNG (options)](#apidoc.element.blessed.PNG)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program"></a>[function <span class="apidocSignatureSpan">blessed.</span>Program (options)](#apidoc.element.blessed.Program)
- description and source-code
```javascript
function Program(options) {
  var self = this;

  if (!(this instanceof Program)) {
    return new Program(options);
  }

  Program.bind(this);

  EventEmitter.call(this);

  if (!options || options.__proto__ !== Object.prototype) {
    options = {
      input: arguments[0],
      output: arguments[1]
    };
  }

  this.options = options;
  this.input = options.input || process.stdin;
  this.output = options.output || process.stdout;

  options.log = options.log || options.dump;
  if (options.log) {
    this._logger = fs.createWriteStream(options.log);
    if (options.dump) this.setupDump();
  }

  this.zero = options.zero !== false;
  this.useBuffer = options.buffer;

  this.x = 0;
  this.y = 0;
  this.savedX = 0;
  this.savedY = 0;

  this.cols = this.output.columns || 1;
  this.rows = this.output.rows || 1;

  this.scrollTop = 0;
  this.scrollBottom = this.rows - 1;

  this._terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this._terminal = this._terminal.toLowerCase();

  // OSX
  this.isOSXTerm = process.env.TERM_PROGRAM === 'Apple_Terminal';
  this.isiTerm2 = process.env.TERM_PROGRAM === 'iTerm.app'
    || !!process.env.ITERM_SESSION_ID;

  // VTE
  // NOTE: lxterminal does not provide an env variable to check for.
  // NOTE: gnome-terminal and sakura use a later version of VTE
  // which provides VTE_VERSION as well as supports SGR events.
  this.isXFCE = /xfce/i.test(process.env.COLORTERM);
  this.isTerminator = !!process.env.TERMINATOR_UUID;
  this.isLXDE = false;
  this.isVTE = !!process.env.VTE_VERSION
    || this.isXFCE
    || this.isTerminator
    || this.isLXDE;

  // xterm and rxvt - not accurate
  this.isRxvt = /rxvt/i.test(process.env.COLORTERM);
  this.isXterm = false;

  this.tmux = !!process.env.TMUX;
  this.tmuxVersion = (function() {
    if (!self.tmux) return 2;
    try {
      var version = cp.execFileSync('tmux', ['-V'], { encoding: 'utf8' });
      return +/^tmux ([\d.]+)/i.exec(version.trim().split('\n')[0])[1];
    } catch (e) {
      return 2;
    }
  })();

  this._buf = '';
  this._flush = this.flush.bind(this);

  if (options.tput !== false) {
    this.setupTput();
  }

  this.listen();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ProgressBar"></a>[function <span class="apidocSignatureSpan">blessed.</span>ProgressBar (options)](#apidoc.element.blessed.ProgressBar)
- description and source-code
```javascript
function ProgressBar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ProgressBar(options);
  }

  options = options || {};

  Input.call(this, options);

  this.filled = options.filled || 0;
  if (typeof this.filled === 'string') {
    this.filled = +this.filled.slice(0, -1);
  }
  this.value = this.filled;

  this.pch = options.pch || ' ';

  // XXX Workaround that predates the usage of 'el.ch'.
  if (options.ch) {
    this.pch = options.ch;
    this.ch = ' ';
  }
  if (options.bch) {
    this.ch = options.bch;
  }

  if (!this.style.bar) {
    this.style.bar = {};
    this.style.bar.fg = options.barFg;
    this.style.bar.bg = options.barBg;
  }

  this.orientation = options.orientation || 'horizontal';

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      var back, forward;
      if (self.orientation === 'horizontal') {
        back = ['left', 'h'];
        forward = ['right', 'l'];
      } else if (self.orientation === 'vertical') {
        back = ['down', 'j'];
        forward = ['up', 'k'];
      }
      if (key.name === back[0] || (options.vi && key.name === back[1])) {
        self.progress(-5);
        self.screen.render();
        return;
      }
      if (key.name === forward[0] || (options.vi && key.name === forward[1])) {
        self.progress(5);
        self.screen.render();
        return;
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      var x, y, m, p;
      if (!self.lpos) return;
      if (self.orientation === 'horizontal') {
        x = data.x - self.lpos.xi;
        m = (self.lpos.xl - self.lpos.xi) - self.iwidth;
        p = x / m * 100 | 0;
      } else if (self.orientation === 'vertical') {
        y = data.y - self.lpos.yi;
        m = (self.lpos.yl - self.lpos.yi) - self.iheight;
        p = y / m * 100 | 0;
      }
      self.setProgress(p);
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Prompt"></a>[function <span class="apidocSignatureSpan">blessed.</span>Prompt (options)](#apidoc.element.blessed.Prompt)
- description and source-code
```javascript
function Prompt(options) {
  if (!(this instanceof Node)) {
    return new Prompt(options);
  }

  options = options || {};

  options.hidden = true;

  Box.call(this, options);

  this._.input = new Textbox({
    parent: this,
    top: 3,
    height: 1,
    left: 2,
    right: 2,
    bg: 'black'
  });

  this._.okay = new Button({
    parent: this,
    top: 5,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    parent: this,
    top: 5,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Question"></a>[function <span class="apidocSignatureSpan">blessed.</span>Question (options)](#apidoc.element.blessed.Question)
- description and source-code
```javascript
function Question(options) {
  if (!(this instanceof Node)) {
    return new Question(options);
  }

  options = options || {};
  options.hidden = true;

  Box.call(this, options);

  this._.okay = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.RadioButton"></a>[function <span class="apidocSignatureSpan">blessed.</span>RadioButton (options)](#apidoc.element.blessed.RadioButton)
- description and source-code
```javascript
function RadioButton(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new RadioButton(options);
  }

  options = options || {};

  Checkbox.call(this, options);

  this.on('check', function() {
    var el = self;
    while (el = el.parent) {
      if (el.type === 'radio-set'
          || el.type === 'form') break;
    }
    el = el || self.parent;
    el.forDescendants(function(el) {
      if (el.type !== 'radio-button' || el === self) {
        return;
      }
      el.uncheck();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.RadioSet"></a>[function <span class="apidocSignatureSpan">blessed.</span>RadioSet (options)](#apidoc.element.blessed.RadioSet)
- description and source-code
```javascript
function RadioSet(options) {
  if (!(this instanceof Node)) {
    return new RadioSet(options);
  }
  options = options || {};
  // Possibly inherit parent's style.
  // options.style = this.parent.style;
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen"></a>[function <span class="apidocSignatureSpan">blessed.</span>Screen (options)](#apidoc.element.blessed.Screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ScrollableBox"></a>[function <span class="apidocSignatureSpan">blessed.</span>ScrollableBox (options)](#apidoc.element.blessed.ScrollableBox)
- description and source-code
```javascript
function ScrollableBox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ScrollableBox(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.scrollable === false) {
    return this;
  }

  this.scrollable = true;
  this.childOffset = 0;
  this.childBase = 0;
  this.baseLimit = options.baseLimit || Infinity;
  this.alwaysScroll = options.alwaysScroll;

  this.scrollbar = options.scrollbar;
  if (this.scrollbar) {
    this.scrollbar.ch = this.scrollbar.ch || ' ';
    this.style.scrollbar = this.style.scrollbar || this.scrollbar.style;
    if (!this.style.scrollbar) {
      this.style.scrollbar = {};
      this.style.scrollbar.fg = this.scrollbar.fg;
      this.style.scrollbar.bg = this.scrollbar.bg;
      this.style.scrollbar.bold = this.scrollbar.bold;
      this.style.scrollbar.underline = this.scrollbar.underline;
      this.style.scrollbar.inverse = this.scrollbar.inverse;
      this.style.scrollbar.invisible = this.scrollbar.invisible;
    }
    //this.scrollbar.style = this.style.scrollbar;
    if (this.track || this.scrollbar.track) {
      this.track = this.scrollbar.track || this.track;
      this.style.track = this.style.scrollbar.track || this.style.track;
      this.track.ch = this.track.ch || ' ';
      this.style.track = this.style.track || this.track.style;
      if (!this.style.track) {
        this.style.track = {};
        this.style.track.fg = this.track.fg;
        this.style.track.bg = this.track.bg;
        this.style.track.bold = this.track.bold;
        this.style.track.underline = this.track.underline;
        this.style.track.inverse = this.track.inverse;
        this.style.track.invisible = this.track.invisible;
      }
      this.track.style = this.style.track;
    }
    // Allow controlling of the scrollbar via the mouse:
    if (options.mouse) {
      this.on('mousedown', function(data) {
        if (self._scrollingBar) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          return;
        }
        var x = data.x - self.aleft;
        var y = data.y - self.atop;
        if (x === self.width - self.iright - 1) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          var perc = (y - self.itop) / (self.height - self.iheight);
          self.setScrollPerc(perc * 100 | 0);
          self.screen.render();
          var smd, smu;
          self._scrollingBar = true;
          self.onScreenEvent('mousedown', smd = function(data) {
            var y = data.y - self.atop;
            var perc = y / self.height;
            self.setScrollPerc(perc * 100 | 0);
            self.screen.render();
          });
          // If mouseup occurs out of the window, no mouseup event fires, and
          // scrollbar will drag again on mousedown until another mouseup
          // occurs.
          self.onScreenEvent('mouseup', smu = function() {
            self._scrollingBar = false;
            self.removeScreenEvent('mousedown', smd);
            self.removeScreenEvent('mouseup', smu);
          });
        }
      });
    }
  }

  if (options.mouse) {
    this.on('wheeldown', function() {
      self.scroll(self.height / 2 | 0 || 1);
      self.screen.render();
    });
    this.on('wheelup', function() {
      self.scroll(-(self.height / 2 | 0) || -1);
      self.screen.render();
    });
  }

  if (options.keys && !options.ignoreKeys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.scroll(-1);
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.scroll(1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.scroll(-(self.height / 2 | 0) || -1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.scroll( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ScrollableText"></a>[function <span class="apidocSignatureSpan">blessed.</span>ScrollableText (options)](#apidoc.element.blessed.ScrollableText)
- description and source-code
```javascript
function ScrollableText(options) {
  if (!(this instanceof Node)) {
    return new ScrollableText(options);
  }
  options = options || {};
  options.alwaysScroll = true;
  ScrollableBox.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Table"></a>[function <span class="apidocSignatureSpan">blessed.</span>Table (options)](#apidoc.element.blessed.Table)
- description and source-code
```javascript
function Table(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Table(options);
  }

  options = options || {};
  options.shrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  options.align = options.align || 'center';

  // Regular tables do not get custom height (this would
  // require extra padding). Maybe add in the future.
  delete options.height;

  Box.call(this, options);

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setContent('');
    self.setData(self.rows);
  });

  this.on('resize', function() {
    self.setContent('');
    self.setData(self.rows);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Terminal"></a>[function <span class="apidocSignatureSpan">blessed.</span>Terminal (options)](#apidoc.element.blessed.Terminal)
- description and source-code
```javascript
function Terminal(options) {
  if (!(this instanceof Node)) {
    return new Terminal(options);
  }

  options = options || {};
  options.scrollable = false;

  Box.call(this, options);

  // XXX Workaround for all motion
  if (this.screen.program.tmux && this.screen.program.tmuxVersion >= 2) {
    this.screen.program.enableMouse();
  }

  this.handler = options.handler;
  this.shell = options.shell || process.env.SHELL || 'sh';
  this.args = options.args || [];

  this.cursor = this.options.cursor;
  this.cursorBlink = this.options.cursorBlink;
  this.screenKeys = this.options.screenKeys;

  this.style = this.style || {};
  this.style.bg = this.style.bg || 'default';
  this.style.fg = this.style.fg || 'default';

  this.termName = options.terminal
    || options.term
    || process.env.TERM
    || 'xterm';

  this.bootstrap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Text"></a>[function <span class="apidocSignatureSpan">blessed.</span>Text (options)](#apidoc.element.blessed.Text)
- description and source-code
```javascript
function Text(options) {
  if (!(this instanceof Node)) {
    return new Text(options);
  }
  options = options || {};
  options.shrink = true;
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Textarea"></a>[function <span class="apidocSignatureSpan">blessed.</span>Textarea (options)](#apidoc.element.blessed.Textarea)
- description and source-code
```javascript
function Textarea(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Textarea(options);
  }

  options = options || {};

  options.scrollable = options.scrollable !== false;

  Input.call(this, options);

  this.screen._listenKeys(this);

  this.value = options.value || '';

  this.__updateCursor = this._updateCursor.bind(this);
  this.on('resize', this.__updateCursor);
  this.on('move', this.__updateCursor);

  if (options.inputOnFocus) {
    this.on('focus', this.readInput.bind(this, null));
  }

  if (!options.inputOnFocus && options.keys) {
    this.on('keypress', function(ch, key) {
      if (self._reading) return;
      if (key.name === 'enter' || (options.vi && key.name === 'i')) {
        return self.readInput();
      }
      if (key.name === 'e') {
        return self.readEditor();
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      if (self._reading) return;
      if (data.button !== 'right') return;
      self.readEditor();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Textbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>Textbox (options)](#apidoc.element.blessed.Textbox)
- description and source-code
```javascript
function Textbox(options) {
  if (!(this instanceof Node)) {
    return new Textbox(options);
  }

  options = options || {};

  options.scrollable = false;

  Textarea.call(this, options);

  this.secret = options.secret;
  this.censor = options.censor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput"></a>[function <span class="apidocSignatureSpan">blessed.</span>Tput (options)](#apidoc.element.blessed.Tput)
- description and source-code
```javascript
function Tput(options) {
  if (!(this instanceof Tput)) {
    return new Tput(options);
  }

  options = options || {};
  if (typeof options === 'string') {
    options = { terminal: options };
  }

  this.options = options;
  this.terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this.terminal = this.terminal.toLowerCase();

  this.debug = options.debug;
  this.padding = options.padding;
  this.extended = options.extended;
  this.printf = options.printf;
  this.termcap = options.termcap;
  this.error = null;

  this.terminfoPrefix = options.terminfoPrefix;
  this.terminfoFile = options.terminfoFile;
  this.termcapFile = options.termcapFile;

  if (options.terminal || options.term) {
    this.setup();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Video"></a>[function <span class="apidocSignatureSpan">blessed.</span>Video (options)](#apidoc.element.blessed.Video)
- description and source-code
```javascript
function Video(options) {
  var self = this
    , shell
    , args;

  if (!(this instanceof Node)) {
    return new Video(options);
  }

  options = options || {};

  Box.call(this, options);

  if (this.exists('mplayer')) {
    shell = 'mplayer';
    args = ['-vo', 'caca', '-quiet', options.file];
  } else if (this.exists('mpv')) {
    shell = 'mpv';
    args = ['--vo', 'caca', '--really-quiet', options.file];
  } else {
    this.parseTags = true;
    this.setContent('{red-fg}{bold}Error:{/bold}'
      + ' mplayer or mpv not installed.{/red-fg}');
    return this;
  }

  var opts = {
    parent: this,
    left: 0,
    top: 0,
    width: this.width - this.iwidth,
    height: this.height - this.iheight,
    shell: shell,
    args: args.slice()
  };

  this.now = Date.now() / 1000 | 0;
  this.start = opts.start || 0;
  if (this.start) {
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', this.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', this.start + '');
    }
  }

  var DISPLAY = process.env.DISPLAY;
  delete process.env.DISPLAY;
  this.tty = new Terminal(opts);
  process.env.DISPLAY = DISPLAY;

  this.on('click', function() {
    self.tty.pty.write('p');
  });

  // mplayer/mpv cannot resize itself in the terminal, so we have
  // to restart it at the correct start time.
  this.on('resize', function() {
    self.tty.destroy();

    var opts = {
      parent: self,
      left: 0,
      top: 0,
      width: self.width - self.iwidth,
      height: self.height - self.iheight,
      shell: shell,
      args: args.slice()
    };

    var watched = (Date.now() / 1000 | 0) - self.now;
    self.now = Date.now() / 1000 | 0;
    self.start += watched;
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', self.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', self.start + '');
    }

    var DISPLAY = process.env.DISPLAY;
    delete process.env.DISPLAY;
    self.tty = new Terminal(opts);
    process.env.DISPLAY = DISPLAY;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage"></a>[function <span class="apidocSignatureSpan">blessed.</span>ansiimage (options)](#apidoc.element.blessed.ansiimage)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.asort"></a>[function <span class="apidocSignatureSpan">blessed.</span>asort (obj)](#apidoc.element.blessed.asort)
- description and source-code
```javascript
asort = function (obj) {
  return obj.sort(function(a, b) {
    a = a.name.toLowerCase();
    b = b.name.toLowerCase();

    if (a[0] === '.' && b[0] === '.') {
      a = a[1];
      b = b[1];
    } else {
      a = a[0];
      b = b[0];
    }

    return a > b ? 1 : (a < b ? -1 : 0);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.attrToBinary"></a>[function <span class="apidocSignatureSpan">blessed.</span>attrToBinary (style, element)](#apidoc.element.blessed.attrToBinary)
- description and source-code
```javascript
attrToBinary = function (style, element) {
  return helpers.Element.prototype.sattr.call(element || {}, style);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.bigtext"></a>[function <span class="apidocSignatureSpan">blessed.</span>bigtext (options)](#apidoc.element.blessed.bigtext)
- description and source-code
```javascript
function BigText(options) {
  if (!(this instanceof Node)) {
    return new BigText(options);
  }
  options = options || {};
  options.font = options.font
    || __dirname + '/../../usr/fonts/ter-u14n.json';
  options.fontBold = options.font
    || __dirname + '/../../usr/fonts/ter-u14b.json';
  this.fch = options.fch;
  this.ratio = {};
  this.font = this.loadFont(options.font);
  this.fontBold = this.loadFont(options.font);
  Box.call(this, options);
  if (this.style.bold) {
    this.font = this.fontBold;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.box"></a>[function <span class="apidocSignatureSpan">blessed.</span>box (options)](#apidoc.element.blessed.box)
- description and source-code
```javascript
function Box(options) {
  if (!(this instanceof Node)) {
    return new Box(options);
  }
  options = options || {};
  Element.call(this, options);
}
```
- example usage
```shell
...
var screen = blessed.screen({
smartCSR: true
});

screen.title = 'my window title';

// Create a box perfectly centered horizontally and vertically.
var box = blessed.box({
top: 'center',
left: 'center',
width: '50%',
height: '50%',
content: 'Hello {bold}world{/bold}!',
tags: true,
border: {
...
```

#### <a name="apidoc.element.blessed.button"></a>[function <span class="apidocSignatureSpan">blessed.</span>button (options)](#apidoc.element.blessed.button)
- description and source-code
```javascript
function Button(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Button(options);
  }

  options = options || {};

  if (options.autoFocus == null) {
    options.autoFocus = false;
  }

  Input.call(this, options);

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      return self.press();
    }
  });

  if (this.options.mouse) {
    this.on('click', function() {
      return self.press();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.checkbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>checkbox (options)](#apidoc.element.blessed.checkbox)
- description and source-code
```javascript
function Checkbox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Checkbox(options);
  }

  options = options || {};

  Input.call(this, options);

  this.text = options.content || options.text || '';
  this.checked = this.value = options.checked || false;

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      self.toggle();
      self.screen.render();
    }
  });

  if (options.mouse) {
    this.on('click', function() {
      self.toggle();
      self.screen.render();
    });
  }

  this.on('focus', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    self.screen.program.lsaveCursor('checkbox');
    self.screen.program.cup(lpos.yi, lpos.xi + 1);
    self.screen.program.showCursor();
  });

  this.on('blur', function() {
    self.screen.program.lrestoreCursor('checkbox', true);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.cleanTags"></a>[function <span class="apidocSignatureSpan">blessed.</span>cleanTags (text)](#apidoc.element.blessed.cleanTags)
- description and source-code
```javascript
cleanTags = function (text) {
  return helpers.stripTags(text).trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.dropUnicode"></a>[function <span class="apidocSignatureSpan">blessed.</span>dropUnicode (text)](#apidoc.element.blessed.dropUnicode)
- description and source-code
```javascript
dropUnicode = function (text) {
  if (!text) return '';
  return text
    .replace(unicode.chars.all, '??')
    .replace(unicode.chars.combining, '')
    .replace(unicode.chars.surrogate, '?');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.element"></a>[function <span class="apidocSignatureSpan">blessed.</span>element (options)](#apidoc.element.blessed.element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.escape"></a>[function <span class="apidocSignatureSpan">blessed.</span>escape (text)](#apidoc.element.blessed.escape)
- description and source-code
```javascript
escape = function (text) {
  return text.replace(/[{}]/g, function(ch) {
    return ch === '{' ? '{open}' : '{close}';
  });
}
```
- example usage
```shell
...

- __merge(a, b)__ - Merge objects 'a' and 'b' into object 'a'.
- __asort(obj)__ - Sort array alphabetically by 'name' prop.
- __hsort(obj)__ - Sort array numerically by 'index' prop.
- __findFile(start, target)__ - Find a file at 'start' directory with name
'target'.
- __escape(text)__ - Escape content's tags to be passed into 'el.setContent()'.
Example: 'box.setContent('escaped tag: ' + blessed.escape('{bold}{/bold}'));'
- __parseTags(text)__ - Parse tags into SGR escape codes.
- __generateTags(style, text)__ - Generate text tags based on 'style' object.
- __attrToBinary(style, element)__ - Convert 'style' attributes to binary
format.
- __stripTags(text)__ - Strip text of tags and SGR sequences.
- __cleanTags(text)__ - Strip text of tags, SGR escape code, and
leading/trailing whitespace.
...
```

#### <a name="apidoc.element.blessed.filemanager"></a>[function <span class="apidocSignatureSpan">blessed.</span>filemanager (options)](#apidoc.element.blessed.filemanager)
- description and source-code
```javascript
function FileManager(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new FileManager(options);
  }

  options = options || {};
  options.parseTags = true;
  // options.label = ' {blue-fg}%path{/blue-fg} ';

  List.call(this, options);

  this.cwd = options.cwd || process.cwd();
  this.file = this.cwd;
  this.value = this.cwd;

  if (options.label && ~options.label.indexOf('%path')) {
    this._label.setContent(options.label.replace('%path', this.cwd));
  }

  this.on('select', function(item) {
    var value = item.content.replace(/\{[^{}]+\}/g, '').replace(/@$/, '')
      , file = path.resolve(self.cwd, value);

    return fs.stat(file, function(err, stat) {
      if (err) {
        return self.emit('error', err, file);
      }
      self.file = file;
      self.value = file;
      if (stat.isDirectory()) {
        self.emit('cd', file, self.cwd);
        self.cwd = file;
        if (options.label && ~options.label.indexOf('%path')) {
          self._label.setContent(options.label.replace('%path', file));
        }
        self.refresh();
      } else {
        self.emit('file', file);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.findFile"></a>[function <span class="apidocSignatureSpan">blessed.</span>findFile (start, target)](#apidoc.element.blessed.findFile)
- description and source-code
```javascript
findFile = function (start, target) {
  return (function read(dir) {
    var files, file, stat, out;

    if (dir === '/dev' || dir === '/sys'
        || dir === '/proc' || dir === '/net') {
      return null;
    }

    try {
      files = fs.readdirSync(dir);
    } catch (e) {
      files = [];
    }

    for (var i = 0; i < files.length; i++) {
      file = files[i];

      if (file === target) {
        return (dir === '/' ? '' : dir) + '/' + file;
      }

      try {
        stat = fs.lstatSync((dir === '/' ? '' : dir) + '/' + file);
      } catch (e) {
        stat = null;
      }

      if (stat && stat.isDirectory() && !stat.isSymbolicLink()) {
        out = read((dir === '/' ? '' : dir) + '/' + file);
        if (out) return out;
      }
    }

    return null;
  })(start);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form"></a>[function <span class="apidocSignatureSpan">blessed.</span>form (options)](#apidoc.element.blessed.form)
- description and source-code
```javascript
function Form(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Form(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  Box.call(this, options);

  if (options.keys) {
    this.screen._listenKeys(this);
    this.on('element keypress', function(el, ch, key) {
      if ((key.name === 'tab' && !key.shift)
          || (el.type === 'textbox' && options.autoNext && key.name === 'enter')
          || key.name === 'down'
          || (options.vi && key.name === 'j')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'j') return;
          if (key.name === 'tab') {
            // Workaround, since we can't stop the tab from being added.
            el.emit('keypress', null, { name: 'backspace' });
          }
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusNext();
        return;
      }

      if ((key.name === 'tab' && key.shift)
          || key.name === 'up'
          || (options.vi && key.name === 'k')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'k') return;
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusPrevious();
        return;
      }

      if (key.name === 'escape') {
        self.focus();
        return;
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.generateTags"></a>[function <span class="apidocSignatureSpan">blessed.</span>generateTags (style, text)](#apidoc.element.blessed.generateTags)
- description and source-code
```javascript
generateTags = function (style, text) {
  var open = ''
    , close = '';

  Object.keys(style || {}).forEach(function(key) {
    var val = style[key];
    if (typeof val === 'string') {
      val = val.replace(/^light(?!-)/, 'light-');
      val = val.replace(/^bright(?!-)/, 'bright-');
      open = '{' + val + '-' + key + '}' + open;
      close += '{/' + val + '-' + key + '}';
    } else {
      if (val === true) {
        open = '{' + key + '}' + open;
        close += '{/' + key + '}';
      }
    }
  });

  if (text != null) {
    return open + text + close;
  }

  return {
    open: open,
    close: close
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.hsort"></a>[function <span class="apidocSignatureSpan">blessed.</span>hsort (obj)](#apidoc.element.blessed.hsort)
- description and source-code
```javascript
hsort = function (obj) {
  return obj.sort(function(a, b) {
    return b.index - a.index;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.image"></a>[function <span class="apidocSignatureSpan">blessed.</span>image (options)](#apidoc.element.blessed.image)
- description and source-code
```javascript
function Image(options) {
  if (!(this instanceof Node)) {
    return new Image(options);
  }

  options = options || {};
  options.type = options.itype || options.type || 'ansi';

  Box.call(this, options);

  if (options.type === 'ansi' && this.type !== 'ansiimage') {
    var ANSIImage = require('./ansiimage');
    Object.getOwnPropertyNames(ANSIImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ANSIImage.prototype, key));
    }, this);
    ANSIImage.call(this, options);
    return this;
  }

  if (options.type === 'overlay' && this.type !== 'overlayimage') {
    var OverlayImage = require('./overlayimage');
    Object.getOwnPropertyNames(OverlayImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(OverlayImage.prototype, key));
    }, this);
    OverlayImage.call(this, options);
    return this;
  }

  throw new Error(''type' must either be 'ansi' or 'overlay'.');
}
```
- example usage
```shell
...
}
});

// Append our box to the screen.
screen.append(box);

// Add a png icon to the box
var icon = blessed.image({
parent: box,
top: 0,
left: 0,
type: 'overlay',
width: 'shrink',
height: 'shrink',
file: __dirname + '/my-program-icon.png',
...
```

#### <a name="apidoc.element.blessed.input"></a>[function <span class="apidocSignatureSpan">blessed.</span>input (options)](#apidoc.element.blessed.input)
- description and source-code
```javascript
function Input(options) {
  if (!(this instanceof Node)) {
    return new Input(options);
  }
  options = options || {};
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.layout"></a>[function <span class="apidocSignatureSpan">blessed.</span>layout (options)](#apidoc.element.blessed.layout)
- description and source-code
```javascript
function Layout(options) {
  if (!(this instanceof Node)) {
    return new Layout(options);
  }

  options = options || {};

  if ((options.width == null
      && (options.left == null && options.right == null))
      || (options.height == null
      && (options.top == null && options.bottom == null))) {
    throw new Error(''Layout' must have a width and height!');
  }

  options.layout = options.layout || 'inline';

  Element.call(this, options);

  if (options.renderer) {
    this.renderer = options.renderer;
  }
}
```
- example usage
```shell
...

Here is an example of how to provide a renderer. Note that this is also the
default renderer if none is provided. This renderer will render each child as
though they were 'display: inline-block;' in CSS, as if there were a
dynamically sized horizontal grid from left to right.

''' js
var layout = blessed.layout({
parent: screen,
top: 'center',
left: 'center',
width: '50%',
height: '50%',
border: 'line',
style: {
...
```

#### <a name="apidoc.element.blessed.line"></a>[function <span class="apidocSignatureSpan">blessed.</span>line (options)](#apidoc.element.blessed.line)
- description and source-code
```javascript
function Line(options) {
  if (!(this instanceof Node)) {
    return new Line(options);
  }

  options = options || {};

  var orientation = options.orientation || 'vertical';
  delete options.orientation;

  if (orientation === 'vertical') {
    options.width = 1;
  } else {
    options.height = 1;
  }

  Box.call(this, options);

  this.ch = !options.type || options.type === 'line'
    ? orientation === 'horizontal' ? '─' : '│'
    : options.ch || ' ';

  this.border = {
    type: 'bg',
    __proto__: this
  };

  this.style.border = this.style;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list"></a>[function <span class="apidocSignatureSpan">blessed.</span>list (options)](#apidoc.element.blessed.list)
- description and source-code
```javascript
function List(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new List(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  // Possibly put this here: this.items = [];
  options.scrollable = true;
  Box.call(this, options);

  this.value = '';
  this.items = [];
  this.ritems = [];
  this.selected = 0;
  this._isList = true;

  if (!this.style.selected) {
    this.style.selected = {};
    this.style.selected.bg = options.selectedBg;
    this.style.selected.fg = options.selectedFg;
    this.style.selected.bold = options.selectedBold;
    this.style.selected.underline = options.selectedUnderline;
    this.style.selected.blink = options.selectedBlink;
    this.style.selected.inverse = options.selectedInverse;
    this.style.selected.invisible = options.selectedInvisible;
  }

  if (!this.style.item) {
    this.style.item = {};
    this.style.item.bg = options.itemBg;
    this.style.item.fg = options.itemFg;
    this.style.item.bold = options.itemBold;
    this.style.item.underline = options.itemUnderline;
    this.style.item.blink = options.itemBlink;
    this.style.item.inverse = options.itemInverse;
    this.style.item.invisible = options.itemInvisible;
  }

  // Legacy: for apps written before the addition of item attributes.
  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    if (self.style[name] != null && self.style.item[name] == null) {
      self.style.item[name] = self.style[name];
    }
  });

  if (this.options.itemHoverBg) {
    this.options.itemHoverEffects = { bg: this.options.itemHoverBg };
  }

  if (this.options.itemHoverEffects) {
    this.style.item.hover = this.options.itemHoverEffects;
  }

  if (this.options.itemFocusEffects) {
    this.style.item.focus = this.options.itemFocusEffects;
  }

  this.interactive = options.interactive !== false;

  this.mouse = options.mouse || false;

  if (options.items) {
    this.ritems = options.items;
    options.items.forEach(this.add.bind(this));
  }

  this.select(0);

  if (options.mouse) {
    this.screen._listenMouse(this);
    this.on('element wheeldown', function() {
      self.select(self.selected + 2);
      self.screen.render();
    });
    this.on('element wheelup', function() {
      self.select(self.selected - 2);
      self.screen.render();
    });
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.up();
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.down();
        self.screen.render();
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'l' && !key.shift)) {
        self.enterSelected();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.cancelSelected();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.move(-((self.height - self.iheight) / 2) | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.move((self.height - self.iheight) / 2 | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'b' && key.ctrl) {
        self.move(-(self.height - self.iheight));
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'f' && key.ctrl) {
        self.move(self.height - self.iheight);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'h' && key.shift) {
        self.move(self.childBase - self.selected);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'm' && key.shift) {
        // TODO: Maybe use Math.min(this.items.length,
        // ... for calculating visible items elsewhere.
        var visible = Math.min(
          self.height - self.iheight,
          self.items.length) / 2 | 0;
        self.move(sel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar"></a>[function <span class="apidocSignatureSpan">blessed.</span>listbar (options)](#apidoc.element.blessed.listbar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listtable"></a>[function <span class="apidocSignatureSpan">blessed.</span>listtable (options)](#apidoc.element.blessed.listtable)
- description and source-code
```javascript
function ListTable(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ListTable(options);
  }

  options = options || {};
  options.shrink = true;
  options.normalShrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  this.__align = options.align || 'center';
  delete options.align;

  options.style.selected = options.style.cell.selected;
  options.style.item = options.style.cell;

  List.call(this, options);

  this._header = new Box({
    parent: this,
    left: this.screen.autoPadding ? 0 : this.ileft,
    top: 0,
    width: 'shrink',
    height: 1,
    style: options.style.header,
    tags: options.parseTags || options.tags
  });

  this.on('scroll', function() {
    self._header.setFront();
    self._header.rtop = self.childBase;
    if (!self.screen.autoPadding) {
      self._header.rtop = self.childBase + (self.border ? 1 : 0);
    }
  });

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setData(self.rows);
  });

  this.on('resize', function() {
    var selected = self.selected;
    self.setData(self.rows);
    self.select(selected);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.loading"></a>[function <span class="apidocSignatureSpan">blessed.</span>loading (options)](#apidoc.element.blessed.loading)
- description and source-code
```javascript
function Loading(options) {
  if (!(this instanceof Node)) {
    return new Loading(options);
  }

  options = options || {};

  Box.call(this, options);

  this._.icon = new Text({
    parent: this,
    align: 'center',
    top: 2,
    left: 1,
    right: 1,
    height: 1,
    content: '|'
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.log"></a>[function <span class="apidocSignatureSpan">blessed.</span>log (options)](#apidoc.element.blessed.log)
- description and source-code
```javascript
function Log(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Log(options);
  }

  options = options || {};

  ScrollableText.call(this, options);

  this.scrollback = options.scrollback != null
    ? options.scrollback
    : Infinity;
  this.scrollOnInput = options.scrollOnInput;

  this.on('set content', function() {
    if (!self._userScrolled || self.scrollOnInput) {
      nextTick(function() {
        self.setScrollPerc(100);
        self._userScrolled = false;
        self.screen.render();
      });
    }
  });
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```

#### <a name="apidoc.element.blessed.merge"></a>[function <span class="apidocSignatureSpan">blessed.</span>merge (a, b)](#apidoc.element.blessed.merge)
- description and source-code
```javascript
merge = function (a, b) {
  Object.keys(b).forEach(function(key) {
    a[key] = b[key];
  });
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.message"></a>[function <span class="apidocSignatureSpan">blessed.</span>message (options)](#apidoc.element.blessed.message)
- description and source-code
```javascript
function Message(options) {
  if (!(this instanceof Node)) {
    return new Message(options);
  }

  options = options || {};
  options.tags = true;

  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node"></a>[function <span class="apidocSignatureSpan">blessed.</span>node (options)](#apidoc.element.blessed.node)
- description and source-code
```javascript
function Node(options) {
  var self = this;
  var Screen = require('./screen');

  if (!(this instanceof Node)) {
    return new Node(options);
  }

  EventEmitter.call(this);

  options = options || {};
  this.options = options;

  this.screen = this.screen || options.screen;

  if (!this.screen) {
    if (this.type === 'screen') {
      this.screen = this;
    } else if (Screen.total === 1) {
      this.screen = Screen.global;
    } else if (options.parent) {
      this.screen = options.parent;
      while (this.screen && this.screen.type !== 'screen') {
        this.screen = this.screen.parent;
      }
    } else if (Screen.total) {
      // This _should_ work in most cases as long as the element is appended
      // synchronously after the screen's creation. Throw error if not.
      this.screen = Screen.instances[Screen.instances.length - 1];
      process.nextTick(function() {
        if (!self.parent) {
          throw new Error('Element (' + self.type + ')'
            + ' was not appended synchronously after the'
            + ' screen\'s creation. Please set a 'parent''
            + ' or 'screen' option in the element\'s constructor'
            + ' if you are going to use multiple screens and'
            + ' append the element later.');
        }
      });
    } else {
      throw new Error('No active screen.');
    }
  }

  this.parent = options.parent || null;
  this.children = [];
  this.$ = this._ = this.data = {};
  this.uid = Node.uid++;
  this.index = this.index != null ? this.index : -1;

  if (this.type !== 'screen') {
    this.detached = true;
  }

  if (this.parent) {
    this.parent.append(this);
  }

  (options.children || []).forEach(this.append.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage"></a>[function <span class="apidocSignatureSpan">blessed.</span>overlayimage (options)](#apidoc.element.blessed.overlayimage)
- description and source-code
```javascript
function OverlayImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new OverlayImage(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.w3m) {
    OverlayImage.w3mdisplay = options.w3m;
  }

  if (OverlayImage.hasW3MDisplay == null) {
    if (fs.existsSync(OverlayImage.w3mdisplay)) {
      OverlayImage.hasW3MDisplay = true;
    } else if (options.search !== false) {
      var file = helpers.findFile('/usr', 'w3mimgdisplay')
              || helpers.findFile('/lib', 'w3mimgdisplay')
              || helpers.findFile('/bin', 'w3mimgdisplay');
      if (file) {
        OverlayImage.hasW3MDisplay = true;
        OverlayImage.w3mdisplay = file;
      } else {
        OverlayImage.hasW3MDisplay = false;
      }
    }
  }

  this.on('hide', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('show', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.on('detach', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('attach', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.onScreenEvent('resize', function() {
    self._needsRatio = true;
  });

  // Get images to overlap properly. Maybe not worth it:
  // this.onScreenEvent('render', function() {
  //   self.screen.program.flush();
  //   if (!self._noImage) return;
  //   function display(el, next) {
  //     if (el.type === 'w3mimage' && el.file) {
  //       el.setImage(el.file, next);
  //     } else {
  //       next();
  //     }
  //   }
  //   function done(el) {
  //     el.children.forEach(recurse);
  //   }
  //   function recurse(el) {
  //     display(el, function() {
  //       var pending = el.children.length;
  //       el.children.forEach(function(el) {
  //         display(el, function() {
  //           if (!--pending) done(el);
  //         });
  //       });
  //     });
  //   }
  //   recurse(self.screen);
  // });

  this.onScreenEvent('render', function() {
    self.screen.program.flush();
    if (!self._noImage) {
      self.setImage(self.file);
    }
  });

  if (this.options.file || this.options.img) {
    this.setImage(this.options.file || this.options.img);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.parseTags"></a>[function <span class="apidocSignatureSpan">blessed.</span>parseTags (text, screen)](#apidoc.element.blessed.parseTags)
- description and source-code
```javascript
parseTags = function (text, screen) {
  return helpers.Element.prototype._parseTags.call(
    { parseTags: true, screen: screen || helpers.Screen.global }, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.png"></a>[function <span class="apidocSignatureSpan">blessed.</span>png (options)](#apidoc.element.blessed.png)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.program"></a>[function <span class="apidocSignatureSpan">blessed.</span>program (options)](#apidoc.element.blessed.program)
- description and source-code
```javascript
function Program(options) {
  var self = this;

  if (!(this instanceof Program)) {
    return new Program(options);
  }

  Program.bind(this);

  EventEmitter.call(this);

  if (!options || options.__proto__ !== Object.prototype) {
    options = {
      input: arguments[0],
      output: arguments[1]
    };
  }

  this.options = options;
  this.input = options.input || process.stdin;
  this.output = options.output || process.stdout;

  options.log = options.log || options.dump;
  if (options.log) {
    this._logger = fs.createWriteStream(options.log);
    if (options.dump) this.setupDump();
  }

  this.zero = options.zero !== false;
  this.useBuffer = options.buffer;

  this.x = 0;
  this.y = 0;
  this.savedX = 0;
  this.savedY = 0;

  this.cols = this.output.columns || 1;
  this.rows = this.output.rows || 1;

  this.scrollTop = 0;
  this.scrollBottom = this.rows - 1;

  this._terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this._terminal = this._terminal.toLowerCase();

  // OSX
  this.isOSXTerm = process.env.TERM_PROGRAM === 'Apple_Terminal';
  this.isiTerm2 = process.env.TERM_PROGRAM === 'iTerm.app'
    || !!process.env.ITERM_SESSION_ID;

  // VTE
  // NOTE: lxterminal does not provide an env variable to check for.
  // NOTE: gnome-terminal and sakura use a later version of VTE
  // which provides VTE_VERSION as well as supports SGR events.
  this.isXFCE = /xfce/i.test(process.env.COLORTERM);
  this.isTerminator = !!process.env.TERMINATOR_UUID;
  this.isLXDE = false;
  this.isVTE = !!process.env.VTE_VERSION
    || this.isXFCE
    || this.isTerminator
    || this.isLXDE;

  // xterm and rxvt - not accurate
  this.isRxvt = /rxvt/i.test(process.env.COLORTERM);
  this.isXterm = false;

  this.tmux = !!process.env.TMUX;
  this.tmuxVersion = (function() {
    if (!self.tmux) return 2;
    try {
      var version = cp.execFileSync('tmux', ['-V'], { encoding: 'utf8' });
      return +/^tmux ([\d.]+)/i.exec(version.trim().split('\n')[0])[1];
    } catch (e) {
      return 2;
    }
  })();

  this._buf = '';
  this._flush = this.flush.bind(this);

  if (options.tput !== false) {
    this.setupTput();
  }

  this.listen();
}
```
- example usage
```shell
...
$ echo "$(tput.js setaf 2)Hello World$(tput.js sgr0)"
'''

The main functionality is exposed in the main 'blessed' module:

''' js
var blessed = require('blessed')
, program = blessed.program();

program.key('q', function(ch, key) {
program.clear();
program.disableMouse();
program.showCursor();
program.normalBuffer();
process.exit(0);
...
```

#### <a name="apidoc.element.blessed.progressbar"></a>[function <span class="apidocSignatureSpan">blessed.</span>progressbar (options)](#apidoc.element.blessed.progressbar)
- description and source-code
```javascript
function ProgressBar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ProgressBar(options);
  }

  options = options || {};

  Input.call(this, options);

  this.filled = options.filled || 0;
  if (typeof this.filled === 'string') {
    this.filled = +this.filled.slice(0, -1);
  }
  this.value = this.filled;

  this.pch = options.pch || ' ';

  // XXX Workaround that predates the usage of 'el.ch'.
  if (options.ch) {
    this.pch = options.ch;
    this.ch = ' ';
  }
  if (options.bch) {
    this.ch = options.bch;
  }

  if (!this.style.bar) {
    this.style.bar = {};
    this.style.bar.fg = options.barFg;
    this.style.bar.bg = options.barBg;
  }

  this.orientation = options.orientation || 'horizontal';

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      var back, forward;
      if (self.orientation === 'horizontal') {
        back = ['left', 'h'];
        forward = ['right', 'l'];
      } else if (self.orientation === 'vertical') {
        back = ['down', 'j'];
        forward = ['up', 'k'];
      }
      if (key.name === back[0] || (options.vi && key.name === back[1])) {
        self.progress(-5);
        self.screen.render();
        return;
      }
      if (key.name === forward[0] || (options.vi && key.name === forward[1])) {
        self.progress(5);
        self.screen.render();
        return;
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      var x, y, m, p;
      if (!self.lpos) return;
      if (self.orientation === 'horizontal') {
        x = data.x - self.lpos.xi;
        m = (self.lpos.xl - self.lpos.xi) - self.iwidth;
        p = x / m * 100 | 0;
      } else if (self.orientation === 'vertical') {
        y = data.y - self.lpos.yi;
        m = (self.lpos.yl - self.lpos.yi) - self.iheight;
        p = y / m * 100 | 0;
      }
      self.setProgress(p);
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.prompt"></a>[function <span class="apidocSignatureSpan">blessed.</span>prompt (options)](#apidoc.element.blessed.prompt)
- description and source-code
```javascript
function Prompt(options) {
  if (!(this instanceof Node)) {
    return new Prompt(options);
  }

  options = options || {};

  options.hidden = true;

  Box.call(this, options);

  this._.input = new Textbox({
    parent: this,
    top: 3,
    height: 1,
    left: 2,
    right: 2,
    bg: 'black'
  });

  this._.okay = new Button({
    parent: this,
    top: 5,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    parent: this,
    top: 5,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.question"></a>[function <span class="apidocSignatureSpan">blessed.</span>question (options)](#apidoc.element.blessed.question)
- description and source-code
```javascript
function Question(options) {
  if (!(this instanceof Node)) {
    return new Question(options);
  }

  options = options || {};
  options.hidden = true;

  Box.call(this, options);

  this._.okay = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.radiobutton"></a>[function <span class="apidocSignatureSpan">blessed.</span>radiobutton (options)](#apidoc.element.blessed.radiobutton)
- description and source-code
```javascript
function RadioButton(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new RadioButton(options);
  }

  options = options || {};

  Checkbox.call(this, options);

  this.on('check', function() {
    var el = self;
    while (el = el.parent) {
      if (el.type === 'radio-set'
          || el.type === 'form') break;
    }
    el = el || self.parent;
    el.forDescendants(function(el) {
      if (el.type !== 'radio-button' || el === self) {
        return;
      }
      el.uncheck();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.radioset"></a>[function <span class="apidocSignatureSpan">blessed.</span>radioset (options)](#apidoc.element.blessed.radioset)
- description and source-code
```javascript
function RadioSet(options) {
  if (!(this instanceof Node)) {
    return new RadioSet(options);
  }
  options = options || {};
  // Possibly inherit parent's style.
  // options.style = this.parent.style;
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.screen"></a>[function <span class="apidocSignatureSpan">blessed.</span>screen (options)](#apidoc.element.blessed.screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
...
'blessed.screen' option. This will enable CSR when scrolling text in elements
or when manipulating lines.

''' js
var blessed = require('blessed');

// Create a screen object.
var screen = blessed.screen({
  smartCSR: true
});

screen.title = 'my window title';

// Create a box perfectly centered horizontally and vertically.
var box = blessed.box({
...
```

#### <a name="apidoc.element.blessed.scrollablebox"></a>[function <span class="apidocSignatureSpan">blessed.</span>scrollablebox (options)](#apidoc.element.blessed.scrollablebox)
- description and source-code
```javascript
function ScrollableBox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ScrollableBox(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.scrollable === false) {
    return this;
  }

  this.scrollable = true;
  this.childOffset = 0;
  this.childBase = 0;
  this.baseLimit = options.baseLimit || Infinity;
  this.alwaysScroll = options.alwaysScroll;

  this.scrollbar = options.scrollbar;
  if (this.scrollbar) {
    this.scrollbar.ch = this.scrollbar.ch || ' ';
    this.style.scrollbar = this.style.scrollbar || this.scrollbar.style;
    if (!this.style.scrollbar) {
      this.style.scrollbar = {};
      this.style.scrollbar.fg = this.scrollbar.fg;
      this.style.scrollbar.bg = this.scrollbar.bg;
      this.style.scrollbar.bold = this.scrollbar.bold;
      this.style.scrollbar.underline = this.scrollbar.underline;
      this.style.scrollbar.inverse = this.scrollbar.inverse;
      this.style.scrollbar.invisible = this.scrollbar.invisible;
    }
    //this.scrollbar.style = this.style.scrollbar;
    if (this.track || this.scrollbar.track) {
      this.track = this.scrollbar.track || this.track;
      this.style.track = this.style.scrollbar.track || this.style.track;
      this.track.ch = this.track.ch || ' ';
      this.style.track = this.style.track || this.track.style;
      if (!this.style.track) {
        this.style.track = {};
        this.style.track.fg = this.track.fg;
        this.style.track.bg = this.track.bg;
        this.style.track.bold = this.track.bold;
        this.style.track.underline = this.track.underline;
        this.style.track.inverse = this.track.inverse;
        this.style.track.invisible = this.track.invisible;
      }
      this.track.style = this.style.track;
    }
    // Allow controlling of the scrollbar via the mouse:
    if (options.mouse) {
      this.on('mousedown', function(data) {
        if (self._scrollingBar) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          return;
        }
        var x = data.x - self.aleft;
        var y = data.y - self.atop;
        if (x === self.width - self.iright - 1) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          var perc = (y - self.itop) / (self.height - self.iheight);
          self.setScrollPerc(perc * 100 | 0);
          self.screen.render();
          var smd, smu;
          self._scrollingBar = true;
          self.onScreenEvent('mousedown', smd = function(data) {
            var y = data.y - self.atop;
            var perc = y / self.height;
            self.setScrollPerc(perc * 100 | 0);
            self.screen.render();
          });
          // If mouseup occurs out of the window, no mouseup event fires, and
          // scrollbar will drag again on mousedown until another mouseup
          // occurs.
          self.onScreenEvent('mouseup', smu = function() {
            self._scrollingBar = false;
            self.removeScreenEvent('mousedown', smd);
            self.removeScreenEvent('mouseup', smu);
          });
        }
      });
    }
  }

  if (options.mouse) {
    this.on('wheeldown', function() {
      self.scroll(self.height / 2 | 0 || 1);
      self.screen.render();
    });
    this.on('wheelup', function() {
      self.scroll(-(self.height / 2 | 0) || -1);
      self.screen.render();
    });
  }

  if (options.keys && !options.ignoreKeys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.scroll(-1);
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.scroll(1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.scroll(-(self.height / 2 | 0) || -1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.scroll( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollabletext"></a>[function <span class="apidocSignatureSpan">blessed.</span>scrollabletext (options)](#apidoc.element.blessed.scrollabletext)
- description and source-code
```javascript
function ScrollableText(options) {
  if (!(this instanceof Node)) {
    return new ScrollableText(options);
  }
  options = options || {};
  options.alwaysScroll = true;
  ScrollableBox.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.sprintf"></a>[function <span class="apidocSignatureSpan">blessed.</span>sprintf (src)](#apidoc.element.blessed.sprintf)
- description and source-code
```javascript
function sprintf(src) {
  var params = Array.prototype.slice.call(arguments, 1)
    , rule = /%([\-+# ]{1,4})?(\d+(?:\.\d+)?)?([doxXsc])/g
    , i = 0;

  return src.replace(rule, function(_, flag, width, type) {
    var flags = (flag || '').split('')
      , param = params[i] != null ? params[i] : ''
      , initial = param
      // , width = +width
      , opt = {}
      , pre = '';

    i++;

    switch (type) {
      case 'd': // signed int
        param = (+param).toString(10);
        break;
      case 'o': // unsigned octal
        param = (+param).toString(8);
        break;
      case 'x': // unsigned hex int
        param = (+param).toString(16);
        break;
      case 'X': // unsigned hex int uppercase
        param = (+param).toString(16).toUppercase();
        break;
      case 's': // string
        break;
      case 'c': // char
        param = isFinite(param)
          ? String.fromCharCode(param || 0200)
          : '';
        break;
    }

    flags.forEach(function(flag) {
      switch (flag) {
        // left-justify by width
        case '-':
          opt.left = true;
          break;
        // always precede numbers with their signs
        case '+':
          opt.signs = true;
          break;
        // used with o, x, X - value is preceded with 0, 0x, or 0X respectively.
        // used with a, A, e, E, f, F, g, G - forces written output to contain
        // a decimal point even if no more digits follow
        case '#':
          opt.hexpoint = true;
          break;
        // if no sign is going to be written, black space in front of the value
        case ' ':
          opt.space = true;
          break;
      }
    });

    width = +width.split('.')[0];

    // Should this be for opt.left too?
    // Example: %2.2X - turns 0 into 00
    if (width && !opt.left) {
      param = param + '';
      while (param.length < width) {
        param = '0' + param;
      }
    }

    if (opt.signs) {
      if (+initial >= 0) {
        pre += '+';
      }
    }

    if (opt.space) {
      if (!opt.signs && +initial >= 0) {
        pre += ' ';
      }
    }

    if (opt.hexpoint) {
      switch (type) {
        case 'o': // unsigned octal
          pre += '0';
          break;
        case 'x': // unsigned hex int
          pre += '0x';
          break;
        case 'X': // unsigned hex int uppercase
          pre += '0X';
          break;
      }
    }

    if (opt.left) {
      if (width > (pre.length + param.length)) {
        width -= pre.length + param.length;
        pre = Array(width + 1).join(' ') + pre;
      }
    }

    return pre + param;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.stripTags"></a>[function <span class="apidocSignatureSpan">blessed.</span>stripTags (text)](#apidoc.element.blessed.stripTags)
- description and source-code
```javascript
stripTags = function (text) {
  if (!text) return '';
  return text
    .replace(/{(\/?)([\w\-,;!#]*)}/g, '')
    .replace(/\x1b\[[\d;]*m/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.table"></a>[function <span class="apidocSignatureSpan">blessed.</span>table (options)](#apidoc.element.blessed.table)
- description and source-code
```javascript
function Table(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Table(options);
  }

  options = options || {};
  options.shrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  options.align = options.align || 'center';

  // Regular tables do not get custom height (this would
  // require extra padding). Maybe add in the future.
  delete options.height;

  Box.call(this, options);

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setContent('');
    self.setData(self.rows);
  });

  this.on('resize', function() {
    self.setContent('');
    self.setData(self.rows);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal"></a>[function <span class="apidocSignatureSpan">blessed.</span>terminal (options)](#apidoc.element.blessed.terminal)
- description and source-code
```javascript
function Terminal(options) {
  if (!(this instanceof Node)) {
    return new Terminal(options);
  }

  options = options || {};
  options.scrollable = false;

  Box.call(this, options);

  // XXX Workaround for all motion
  if (this.screen.program.tmux && this.screen.program.tmuxVersion >= 2) {
    this.screen.program.enableMouse();
  }

  this.handler = options.handler;
  this.shell = options.shell || process.env.SHELL || 'sh';
  this.args = options.args || [];

  this.cursor = this.options.cursor;
  this.cursorBlink = this.options.cursorBlink;
  this.screenKeys = this.options.screenKeys;

  this.style = this.style || {};
  this.style.bg = this.style.bg || 'default';
  this.style.fg = this.style.fg || 'default';

  this.termName = options.terminal
    || options.term
    || process.env.TERM
    || 'xterm';

  this.bootstrap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.text"></a>[function <span class="apidocSignatureSpan">blessed.</span>text (options)](#apidoc.element.blessed.text)
- description and source-code
```javascript
function Text(options) {
  if (!(this instanceof Node)) {
    return new Text(options);
  }
  options = options || {};
  options.shrink = true;
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea"></a>[function <span class="apidocSignatureSpan">blessed.</span>textarea (options)](#apidoc.element.blessed.textarea)
- description and source-code
```javascript
function Textarea(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Textarea(options);
  }

  options = options || {};

  options.scrollable = options.scrollable !== false;

  Input.call(this, options);

  this.screen._listenKeys(this);

  this.value = options.value || '';

  this.__updateCursor = this._updateCursor.bind(this);
  this.on('resize', this.__updateCursor);
  this.on('move', this.__updateCursor);

  if (options.inputOnFocus) {
    this.on('focus', this.readInput.bind(this, null));
  }

  if (!options.inputOnFocus && options.keys) {
    this.on('keypress', function(ch, key) {
      if (self._reading) return;
      if (key.name === 'enter' || (options.vi && key.name === 'i')) {
        return self.readInput();
      }
      if (key.name === 'e') {
        return self.readEditor();
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      if (self._reading) return;
      if (data.button !== 'right') return;
      self.readEditor();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>textbox (options)](#apidoc.element.blessed.textbox)
- description and source-code
```javascript
function Textbox(options) {
  if (!(this instanceof Node)) {
    return new Textbox(options);
  }

  options = options || {};

  options.scrollable = false;

  Textarea.call(this, options);

  this.secret = options.secret;
  this.censor = options.censor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.toString"></a>[function <span class="apidocSignatureSpan">blessed.</span>toString ()](#apidoc.element.blessed.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.tput"></a>[function <span class="apidocSignatureSpan">blessed.</span>tput (options)](#apidoc.element.blessed.tput)
- description and source-code
```javascript
function Tput(options) {
  if (!(this instanceof Tput)) {
    return new Tput(options);
  }

  options = options || {};
  if (typeof options === 'string') {
    options = { terminal: options };
  }

  this.options = options;
  this.terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this.terminal = this.terminal.toLowerCase();

  this.debug = options.debug;
  this.padding = options.padding;
  this.extended = options.extended;
  this.printf = options.printf;
  this.termcap = options.termcap;
  this.error = null;

  this.terminfoPrefix = options.terminfoPrefix;
  this.terminfoFile = options.terminfoFile;
  this.termcapFile = options.termcapFile;

  if (options.terminal || options.term) {
    this.setup();
  }
}
```
- example usage
```shell
...

This will actually parse the xterm terminfo and compile every
string capability to a javascript function:

''' js
var blessed = require('blessed');

var tput = blessed.tput({
  terminal: 'xterm-256color',
  extended: true
});

process.stdout.write(tput.setaf(4) + 'Hello' + tput.sgr0() + '\n');
'''
...
```

#### <a name="apidoc.element.blessed.tryRead"></a>[function <span class="apidocSignatureSpan">blessed.</span>tryRead (file)](#apidoc.element.blessed.tryRead)
- description and source-code
```javascript
function tryRead(file) {
  if (Array.isArray(file)) {
    for (var i = 0; i < file.length; i++) {
      var data = tryRead(file[i]);
      if (data) return data;
    }
    return '';
  }
  if (!file) return '';
  file = path.resolve.apply(path, arguments);
  try {
    return fs.readFileSync(file, 'utf8');
  } catch (e) {
    return '';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.video"></a>[function <span class="apidocSignatureSpan">blessed.</span>video (options)](#apidoc.element.blessed.video)
- description and source-code
```javascript
function Video(options) {
  var self = this
    , shell
    , args;

  if (!(this instanceof Node)) {
    return new Video(options);
  }

  options = options || {};

  Box.call(this, options);

  if (this.exists('mplayer')) {
    shell = 'mplayer';
    args = ['-vo', 'caca', '-quiet', options.file];
  } else if (this.exists('mpv')) {
    shell = 'mpv';
    args = ['--vo', 'caca', '--really-quiet', options.file];
  } else {
    this.parseTags = true;
    this.setContent('{red-fg}{bold}Error:{/bold}'
      + ' mplayer or mpv not installed.{/red-fg}');
    return this;
  }

  var opts = {
    parent: this,
    left: 0,
    top: 0,
    width: this.width - this.iwidth,
    height: this.height - this.iheight,
    shell: shell,
    args: args.slice()
  };

  this.now = Date.now() / 1000 | 0;
  this.start = opts.start || 0;
  if (this.start) {
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', this.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', this.start + '');
    }
  }

  var DISPLAY = process.env.DISPLAY;
  delete process.env.DISPLAY;
  this.tty = new Terminal(opts);
  process.env.DISPLAY = DISPLAY;

  this.on('click', function() {
    self.tty.pty.write('p');
  });

  // mplayer/mpv cannot resize itself in the terminal, so we have
  // to restart it at the correct start time.
  this.on('resize', function() {
    self.tty.destroy();

    var opts = {
      parent: self,
      left: 0,
      top: 0,
      width: self.width - self.iwidth,
      height: self.height - self.iheight,
      shell: shell,
      args: args.slice()
    };

    var watched = (Date.now() / 1000 | 0) - self.now;
    self.now = Date.now() / 1000 | 0;
    self.start += watched;
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', self.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', self.start + '');
    }

    var DISPLAY = process.env.DISPLAY;
    delete process.env.DISPLAY;
    self.tty = new Terminal(opts);
    process.env.DISPLAY = DISPLAY;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Element"></a>[module blessed.Element](#apidoc.module.blessed.Element)

#### <a name="apidoc.element.blessed.Element.Element"></a>[function <span class="apidocSignatureSpan">blessed.</span>Element (options)](#apidoc.element.blessed.Element.Element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Element.prototype"></a>[module blessed.Element.prototype](#apidoc.module.blessed.Element.prototype)

#### <a name="apidoc.element.blessed.Element.prototype._align"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_align (line, width, align)](#apidoc.element.blessed.Element.prototype._align)
- description and source-code
```javascript
_align = function (line, width, align) {
  if (!align) return line;
  //if (!align && !~line.indexOf('{|}')) return line;

  var cline = line.replace(/\x1b\[[\d;]*m/g, '')
    , len = cline.length
    , s = width - len;

  if (this.shrink) {
    s = 0;
  }

  if (len === 0) return line;
  if (s < 0) return line;

  if (align === 'center') {
    s = Array(((s / 2) | 0) + 1).join(' ');
    return s + line + s;
  } else if (align === 'right') {
    s = Array(s + 1).join(' ');
    return s + line;
  } else if (this.parseTags && ~line.indexOf('{|}')) {
    var parts = line.split('{|}');
    var cparts = cline.split('{|}');
    s = Math.max(width - cparts[0].length - cparts[1].length, 0);
    s = Array(s + 1).join(' ');
    return parts[0] + s + parts[1];
  }

  return line;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getBottom"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getBottom (get)](#apidoc.element.blessed.Element.prototype._getBottom)
- description and source-code
```javascript
_getBottom = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , bottom;

  if (this.position.bottom == null && this.position.top != null) {
    bottom = this.screen.rows - (this._getTop(get) + this._getHeight(get));
    if (this.screen.autoPadding) {
      bottom += this.parent.ibottom;
    }
    return bottom;
  }

  bottom = (parent.abottom || 0) + (this.position.bottom || 0);

  if (this.screen.autoPadding) {
    bottom += this.parent.ibottom;
  }

  return bottom;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getCoords"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getCoords (get, noscroll)](#apidoc.element.blessed.Element.prototype._getCoords)
- description and source-code
```javascript
_getCoords = function (get, noscroll) {
  if (this.hidden) return;

  // if (this.parent._rendering) {
  //   get = true;
  // }

  var xi = this._getLeft(get)
    , xl = xi + this._getWidth(get)
    , yi = this._getTop(get)
    , yl = yi + this._getHeight(get)
    , base = this.childBase || 0
    , el = this
    , fixed = this.fixed
    , coords
    , v
    , noleft
    , noright
    , notop
    , nobot
    , ppos
    , b;

  // Attempt to shrink the element base on the
  // size of the content and child elements.
  if (this.shrink) {
    coords = this._getShrink(xi, xl, yi, yl, get);
    xi = coords.xi, xl = coords.xl;
    yi = coords.yi, yl = coords.yl;
  }

  // Find a scrollable ancestor if we have one.
  while (el = el.parent) {
    if (el.scrollable) {
      if (fixed) {
        fixed = false;
        continue;
      }
      break;
    }
  }

  // Check to make sure we're visible and
  // inside of the visible scroll area.
  // NOTE: Lists have a property where only
  // the list items are obfuscated.

  // Old way of doing things, this would not render right if a shrunken element
  // with lots of boxes in it was within a scrollable element.
  // See: $ node test/widget-shrink-fail.js
  // var thisparent = this.parent;

  var thisparent = el;
  if (el && !noscroll) {
    ppos = thisparent.lpos;

    // The shrink option can cause a stack overflow
    // by calling _getCoords on the child again.
    // if (!get && !thisparent.shrink) {
    //   ppos = thisparent._getCoords();
    // }

    if (!ppos) return;

    // TODO: Figure out how to fix base (and cbase to only
    // take into account the *parent's* padding.

    yi -= ppos.base;
    yl -= ppos.base;

    b = thisparent.border ? 1 : 0;

    // XXX
    // Fixes non-'fixed' labels to work with scrolling (they're ON the border):
    // if (this.position.left < 0
    //     || this.position.right < 0
    //     || this.position.top < 0
    //     || this.position.bottom < 0) {
    if (this._isLabel) {
      b = 0;
    }

    if (yi < ppos.yi + b) {
      if (yl - 1 < ppos.yi + b) {
        // Is above.
        return;
      } else {
        // Is partially covered above.
        notop = true;
        v = ppos.yi - yi;
        if (this.border) v--;
        if (thisparent.border) v++;
        base += v;
        yi += v;
      }
    } else if (yl > ppos.yl - b) {
      if (yi > ppos.yl - 1 - b) {
        // Is below.
        return;
      } else {
        // Is partially covered below.
        nobot = true;
        v = yl - ppos.yl;
        if (this.border) v--;
        if (thisparent.border) v++;
        yl -= v;
      }
    }

    // Shouldn't be necessary.
    // assert.ok(yi < yl);
    if (yi >= yl) return;

    // Could allow overlapping stuff in scrolling elements
    // if we cleared the pending buffer before every draw.
    if (xi < el.lpos.xi) {
      xi = el.lpos.xi;
      noleft = true;
      if (this.border) xi--;
      if (thisparent.border) xi++;
    }
    if (xl > el.lpos.xl) {
      xl = el.lpos.xl;
      noright = true;
      if (this.border) xl++;
      if (thisparent.border) xl--;
    }
    //if (xi > xl) return;
    if (xi >= xl) return;
  }

  if (this.noOverflow && this.parent.lpos) {
    if (xi < this.parent.lpos.xi + this.parent.ileft) {
      xi = this.parent.lpos.xi + this.parent.ileft;
    }
    if (xl > this.parent.lpos.xl - this.parent.iright) {
      xl = this.parent.lpos.xl - this.parent.iright;
    }
    if (yi < this.parent.lpos.yi + this.parent.itop) {
      yi = this.parent.lpos.yi + this.parent.itop;
    }
    if (yl > this.parent.lpos.yl - this.parent.ibottom) {
      yl = this.parent.lpos.yl - this.parent.ibottom;
    }
  }

  // if (this.parent.lpos) {
  //   this.parent.lpos._scrollBottom = Math.max(
  //     this.parent.lpos._scrollBottom, yl);
  // }

  return {
    xi: xi,
    xl: xl,
    yi: yi,
    yl: yl,
    base: base,
    noleft: noleft,
    noright: noright,
    notop: notop,
    nobot: nobot,
    renders: this.screen.renders
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getHeight"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getHeight (get)](#apidoc.element.blessed.Element.prototype._getHeight)
- description and source-code
```javascript
_getHeight = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , height = this.position.height
    , top
    , expr;

  if (typeof height === 'string') {
    if (height === 'half') height = '50%';
    expr = height.split(/(?=\+|-)/);
    height = expr[0];
    height = +height.slice(0, -1) / 100;
    height = parent.height * height | 0;
    height += +(expr[1] || 0);
    return height;
  }

  // This is for if the element is being streched or shrunken.
  // Although the width for shrunken elements is calculated
  // in the render function, it may be calculated based on
  // the content width, and the content width is initially
  // decided by the width the element, so it needs to be
  // calculated here.
  if (height == null) {
    top = this.position.top || 0;
    if (typeof top === 'string') {
      if (top === 'center') top = '50%';
      expr = top.split(/(?=\+|-)/);
      top = expr[0];
      top = +top.slice(0, -1) / 100;
      top = parent.height * top | 0;
      top += +(expr[1] || 0);
    }
    height = parent.height - (this.position.bottom || 0) - top;
    if (this.screen.autoPadding) {
      if ((this.position.top != null
          || this.position.bottom == null)
          && this.position.top !== 'center') {
        height -= this.parent.itop;
      }
      height -= this.parent.ibottom;
    }
  }

  return height;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getLeft"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getLeft (get)](#apidoc.element.blessed.Element.prototype._getLeft)
- description and source-code
```javascript
_getLeft = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , left = this.position.left || 0
    , expr;

  if (typeof left === 'string') {
    if (left === 'center') left = '50%';
    expr = left.split(/(?=\+|-)/);
    left = expr[0];
    left = +left.slice(0, -1) / 100;
    left = parent.width * left | 0;
    left += +(expr[1] || 0);
    if (this.position.left === 'center') {
      left -= this._getWidth(get) / 2 | 0;
    }
  }

  if (this.position.left == null && this.position.right != null) {
    return this.screen.cols - this._getWidth(get) - this._getRight(get);
  }

  if (this.screen.autoPadding) {
    if ((this.position.left != null
        || this.position.right == null)
        && this.position.left !== 'center') {
      left += this.parent.ileft;
    }
  }

  return (parent.aleft || 0) + left;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getPos"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getPos ()](#apidoc.element.blessed.Element.prototype._getPos)
- description and source-code
```javascript
_getPos = function () {
  var pos = this.lpos;

  assert.ok(pos);

  if (pos.aleft != null) return pos;

  pos.aleft = pos.xi;
  pos.atop = pos.yi;
  pos.aright = this.screen.cols - pos.xl;
  pos.abottom = this.screen.rows - pos.yl;
  pos.width = pos.xl - pos.xi;
  pos.height = pos.yl - pos.yi;

  return pos;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getRight"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getRight (get)](#apidoc.element.blessed.Element.prototype._getRight)
- description and source-code
```javascript
_getRight = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , right;

  if (this.position.right == null && this.position.left != null) {
    right = this.screen.cols - (this._getLeft(get) + this._getWidth(get));
    if (this.screen.autoPadding) {
      right += this.parent.iright;
    }
    return right;
  }

  right = (parent.aright || 0) + (this.position.right || 0);

  if (this.screen.autoPadding) {
    right += this.parent.iright;
  }

  return right;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getShrink"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrink (xi, xl, yi, yl, get)](#apidoc.element.blessed.Element.prototype._getShrink)
- description and source-code
```javascript
_getShrink = function (xi, xl, yi, yl, get) {
  var shrinkBox = this._getShrinkBox(xi, xl, yi, yl, get)
    , shrinkContent = this._getShrinkContent(xi, xl, yi, yl, get)
    , xll = xl
    , yll = yl;

  // Figure out which one is bigger and use it.
  if (shrinkBox.xl - shrinkBox.xi > shrinkContent.xl - shrinkContent.xi) {
    xi = shrinkBox.xi;
    xl = shrinkBox.xl;
  } else {
    xi = shrinkContent.xi;
    xl = shrinkContent.xl;
  }

  if (shrinkBox.yl - shrinkBox.yi > shrinkContent.yl - shrinkContent.yi) {
    yi = shrinkBox.yi;
    yl = shrinkBox.yl;
  } else {
    yi = shrinkContent.yi;
    yl = shrinkContent.yl;
  }

  // Recenter shrunken elements.
  if (xl < xll && this.position.left === 'center') {
    xll = (xll - xl) / 2 | 0;
    xi += xll;
    xl += xll;
  }

  if (yl < yll && this.position.top === 'center') {
    yll = (yll - yl) / 2 | 0;
    yi += yll;
    yl += yll;
  }

  return { xi: xi, xl: xl, yi: yi, yl: yl };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getShrinkBox"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrinkBox (xi, xl, yi, yl, get)](#apidoc.element.blessed.Element.prototype._getShrinkBox)
- description and source-code
```javascript
_getShrinkBox = function (xi, xl, yi, yl, get) {
  if (!this.children.length) {
    return { xi: xi, xl: xi + 1, yi: yi, yl: yi + 1 };
  }

  var i, el, ret, mxi = xi, mxl = xi + 1, myi = yi, myl = yi + 1;

  // This is a chicken and egg problem. We need to determine how the children
  // will render in order to determine how this element renders, but it in
  // order to figure out how the children will render, they need to know
  // exactly how their parent renders, so, we can give them what we have so
  // far.
  var _lpos;
  if (get) {
    _lpos = this.lpos;
    this.lpos = { xi: xi, xl: xl, yi: yi, yl: yl };
    //this.shrink = false;
  }

  for (i = 0; i < this.children.length; i++) {
    el = this.children[i];

    ret = el._getCoords(get);

    // Or just (seemed to work, but probably not good):
    // ret = el.lpos || this.lpos;

    if (!ret) continue;

    // Since the parent element is shrunk, and the child elements think it's
    // going to take up as much space as possible, an element anchored to the
    // right or bottom will inadvertantly make the parent's shrunken size as
    // large as possible. So, we can just use the height and/or width the of
    // element.
    // if (get) {
    if (el.position.left == null && el.position.right != null) {
      ret.xl = xi + (ret.xl - ret.xi);
      ret.xi = xi;
      if (this.screen.autoPadding) {
        // Maybe just do this no matter what.
        ret.xl += this.ileft;
        ret.xi += this.ileft;
      }
    }
    if (el.position.top == null && el.position.bottom != null) {
      ret.yl = yi + (ret.yl - ret.yi);
      ret.yi = yi;
      if (this.screen.autoPadding) {
        // Maybe just do this no matter what.
        ret.yl += this.itop;
        ret.yi += this.itop;
      }
    }

    if (ret.xi < mxi) mxi = ret.xi;
    if (ret.xl > mxl) mxl = ret.xl;
    if (ret.yi < myi) myi = ret.yi;
    if (ret.yl > myl) myl = ret.yl;
  }

  if (get) {
    this.lpos = _lpos;
    //this.shrink = true;
  }

  if (this.position.width == null
      && (this.position.left == null
      || this.position.right == null)) {
    if (this.position.left == null && this.position.right != null) {
      xi = xl - (mxl - mxi);
      if (!this.screen.autoPadding) {
        xi -= this.padding.left + this.padding.right;
      } else {
        xi -= this.ileft;
      }
    } else {
      xl = mxl;
      if (!this.screen.autoPadding) {
        xl += this.padding.left + this.padding.right;
        // XXX Temporary workaround until we decide to make autoPadding default.
        // See widget-listtable.js for an example of why this is necessary.
        // XXX Maybe just to this for all this being that this would affect
        // width shrunken normal shrunken lists as well.
        // if (this._isList) {
        if (this.type === 'list-table') {
          xl -= this.padding.left + this.padding.right;
          xl += this.iright;
        }
      } else {
        //xl += this.padding.right;
        xl += this.iright;
      }
    }
  }

  if (this.position.height == null
      && (this.position.top == null
      || this.position.bottom == null)
      && (!this.scrollable || this._isList)) {
    // NOTE: Lists get special treatment if they are shrunken - assume they
    // want all list items showing. This is one case we can calculate the
    // height based on items/boxes.
    if (this._isList) {
      myi = 0 - this.itop;
      myl = this.items.length + this.ibottom;
    }
    if (this.position.top == null && this.position.bottom != null) {
      yi = yl - (myl - myi);
      if (!this.screen.autoPadding) {
        yi -= this.padding.top + this.padding.bottom;
      } else {
        yi -= this.itop;
      }
    } else {
      yl = myl;
      if (!this.screen.autoPadding) {
        yl += this.padding.top + this.padding.bottom;
      } else {
        yl += this.ibottom;
      }
    }
  }

  return { xi: xi, xl: xl, yi: yi, yl: yl };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getShrinkContent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getShrinkContent (xi, xl, yi, yl)](#apidoc.element.blessed.Element.prototype._getShrinkContent)
- description and source-code
```javascript
_getShrinkContent = function (xi, xl, yi, yl) {
  var h = this._clines.length
    , w = this._clines.mwidth || 1;

  if (this.position.width == null
      && (this.position.left == null
      || this.position.right == null)) {
    if (this.position.left == null && this.position.right != null) {
      xi = xl - w - this.iwidth;
    } else {
      xl = xi + w + this.iwidth;
    }
  }

  if (this.position.height == null
      && (this.position.top == null
      || this.position.bottom == null)
      && (!this.scrollable || this._isList)) {
    if (this.position.top == null && this.position.bottom != null) {
      yi = yl - h - this.iheight;
    } else {
      yl = yi + h + this.iheight;
    }
  }

  return { xi: xi, xl: xl, yi: yi, yl: yl };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getTop"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getTop (get)](#apidoc.element.blessed.Element.prototype._getTop)
- description and source-code
```javascript
_getTop = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , top = this.position.top || 0
    , expr;

  if (typeof top === 'string') {
    if (top === 'center') top = '50%';
    expr = top.split(/(?=\+|-)/);
    top = expr[0];
    top = +top.slice(0, -1) / 100;
    top = parent.height * top | 0;
    top += +(expr[1] || 0);
    if (this.position.top === 'center') {
      top -= this._getHeight(get) / 2 | 0;
    }
  }

  if (this.position.top == null && this.position.bottom != null) {
    return this.screen.rows - this._getHeight(get) - this._getBottom(get);
  }

  if (this.screen.autoPadding) {
    if ((this.position.top != null
        || this.position.bottom == null)
        && this.position.top !== 'center') {
      top += this.parent.itop;
    }
  }

  return (parent.atop || 0) + top;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._getWidth"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_getWidth (get)](#apidoc.element.blessed.Element.prototype._getWidth)
- description and source-code
```javascript
_getWidth = function (get) {
  var parent = get ? this.parent._getPos() : this.parent
    , width = this.position.width
    , left
    , expr;

  if (typeof width === 'string') {
    if (width === 'half') width = '50%';
    expr = width.split(/(?=\+|-)/);
    width = expr[0];
    width = +width.slice(0, -1) / 100;
    width = parent.width * width | 0;
    width += +(expr[1] || 0);
    return width;
  }

  // This is for if the element is being streched or shrunken.
  // Although the width for shrunken elements is calculated
  // in the render function, it may be calculated based on
  // the content width, and the content width is initially
  // decided by the width the element, so it needs to be
  // calculated here.
  if (width == null) {
    left = this.position.left || 0;
    if (typeof left === 'string') {
      if (left === 'center') left = '50%';
      expr = left.split(/(?=\+|-)/);
      left = expr[0];
      left = +left.slice(0, -1) / 100;
      left = parent.width * left | 0;
      left += +(expr[1] || 0);
    }
    width = parent.width - (this.position.right || 0) - left;
    if (this.screen.autoPadding) {
      if ((this.position.left != null || this.position.right == null)
          && this.position.left !== 'center') {
        width -= this.parent.ileft;
      }
      width -= this.parent.iright;
    }
  }

  return width;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._parseAttr"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_parseAttr (lines)](#apidoc.element.blessed.Element.prototype._parseAttr)
- description and source-code
```javascript
_parseAttr = function (lines) {
  var dattr = this.sattr(this.style)
    , attr = dattr
    , attrs = []
    , line
    , i
    , j
    , c;

  if (lines[0].attr === attr) {
    return;
  }

  for (j = 0; j < lines.length; j++) {
    line = lines[j];
    attrs[j] = attr;
    for (i = 0; i < line.length; i++) {
      if (line[i] === '\x1b') {
        if (c = /^\x1b\[[\d;]*m/.exec(line.substring(i))) {
          attr = this.screen.attrCode(c[0], attr, dattr);
          i += c[0].length - 1;
        }
      }
    }
  }

  return attrs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._parseTags"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_parseTags (text)](#apidoc.element.blessed.Element.prototype._parseTags)
- description and source-code
```javascript
_parseTags = function (text) {
  if (!this.parseTags) return text;
  if (!/{\/?[\w\-,;!#]*}/.test(text)) return text;

  var program = this.screen.program
    , out = ''
    , state
    , bg = []
    , fg = []
    , flag = []
    , cap
    , slash
    , param
    , attr
    , esc;

  for (;;) {
    if (!esc && (cap = /^{escape}/.exec(text))) {
      text = text.substring(cap[0].length);
      esc = true;
      continue;
    }

    if (esc && (cap = /^([\s\S]+?){\/escape}/.exec(text))) {
      text = text.substring(cap[0].length);
      out += cap[1];
      esc = false;
      continue;
    }

    if (esc) {
      // throw new Error('Unterminated escape tag.');
      out += text;
      break;
    }

    if (cap = /^{(\/?)([\w\-,;!#]*)}/.exec(text)) {
      text = text.substring(cap[0].length);
      slash = cap[1] === '/';
      param = cap[2].replace(/-/g, ' ');

      if (param === 'open') {
        out += '{';
        continue;
      } else if (param === 'close') {
        out += '}';
        continue;
      }

      if (param.slice(-3) === ' bg') state = bg;
      else if (param.slice(-3) === ' fg') state = fg;
      else state = flag;

      if (slash) {
        if (!param) {
          out += program._attr('normal');
          bg.length = 0;
          fg.length = 0;
          flag.length = 0;
        } else {
          attr = program._attr(param, false);
          if (attr == null) {
            out += cap[0];
          } else {
            // if (param !== state[state.length - 1]) {
            //   throw new Error('Misnested tags.');
            // }
            state.pop();
            if (state.length) {
              out += program._attr(state[state.length - 1]);
            } else {
              out += attr;
            }
          }
        }
      } else {
        if (!param) {
          out += cap[0];
        } else {
          attr = program._attr(param);
          if (attr == null) {
            out += cap[0];
          } else {
            state.push(param);
            out += attr;
          }
        }
      }

      continue;
    }

    if (cap = /^[\s\S]+?(?={\/?[\w\-,;!#]*})/.exec(text)) {
      text = text.substring(cap[0].length);
      out += cap[0];
      continue;
    }

    out += text;
    break;
  }

  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._render"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_render ()](#apidoc.element.blessed.Element.prototype._render)
- description and source-code
```javascript
_render = function () {
  this._emit('prerender');

  this.parseContent();

  var coords = this._getCoords(true);
  if (!coords) {
    delete this.lpos;
    return;
  }

  if (coords.xl - coords.xi <= 0) {
    coords.xl = Math.max(coords.xl, coords.xi);
    return;
  }

  if (coords.yl - coords.yi <= 0) {
    coords.yl = Math.max(coords.yl, coords.yi);
    return;
  }

  var lines = this.screen.lines
    , xi = coords.xi
    , xl = coords.xl
    , yi = coords.yi
    , yl = coords.yl
    , x
    , y
    , cell
    , attr
    , ch
    , content = this._pcontent
    , ci = this._clines.ci[coords.base]
    , battr
    , dattr
    , c
    , visible
    , i
    , bch = this.ch;

  // Clip content if it's off the edge of the screen
  // if (xi + this.ileft < 0 || yi + this.itop < 0) {
  //   var clines = this._clines.slice();
  //   if (xi + this.ileft < 0) {
  //     for (var i = 0; i < clines.length; i++) {
  //       var t = 0;
  //       var csi = '';
  //       var csis = '';
  //       for (var j = 0; j < clines[i].length; j++) {
  //         while (clines[i][j] === '\x1b') {
  //           csi = '\x1b';
  //           while (clines[i][j++] !== 'm') csi += clines[i][j];
  //           csis += csi;
  //         }
  //         if (++t === -(xi + this.ileft) + 1) break;
  //       }
  //       clines[i] = csis + clines[i].substring(j);
  //     }
  //   }
  //   if (yi + this.itop < 0) {
  //     clines = clines.slice(-(yi + this.itop));
  //   }
  //   content = clines.join('\n');
  // }

  if (coords.base >= this._clines.ci.length) {
    ci = this._pcontent.length;
  }

  this.lpos = coords;

  if (this.border && this.border.type === 'line') {
    this.screen._borderStops[coords.yi] = true;
    this.screen._borderStops[coords.yl - 1] = true;
    // if (!this.screen._borderStops[coords.yi]) {
    //   this.screen._borderStops[coords.yi] = { xi: coords.xi, xl: coords.xl };
    // } else {
    //   if (this.screen._borderStops[coords.yi].xi > coords.xi) {
    //     this.screen._borderStops[coords.yi].xi = coords.xi;
    //   }
    //   if (this.screen._borderStops[coords.yi].xl < coords.xl) {
    //     this.screen._borderStops[coords.yi].xl = coords.xl;
    //   }
    // }
    // this.screen._borderStops[coords.yl - 1] = this.screen._borderStops[coords.yi];
  }

  dattr = this.sattr(this.style);
  attr = dattr;

  // If we're in a scrollable text box, check to
  // see which attributes this line starts with.
  if (ci > 0) {
    attr = this._clines.attr[Math.min(coords.base, this._clines.length - 1)];
  }

  if (this.border) xi++, xl--, yi++, yl--;

  // If we have padding/valign, that means the
  // content-drawing loop will skip a few cells/lines.
  // To deal with this, we can just fill the whole thing
  // ahead of time. This could be optimized.
  if (this.tpadding || (this.valign && this.valign !== 'top')) {
    if (this.style.transparent) {
      for (y = Math.max(yi, 0); y < yl; y++) {
        if (!lines[y]) break;
        for (x = Math.max(xi, 0); x < xl; x++) {
          if (!lines[y][x]) break;
          lines[y][x][0] = colors.blend(attr, lines[y][x][0]);
          // lines[y][x][1] = bch;
          lines[y].dirty = true;
        }
      }
    } else {
      this.screen.fillRegion(dattr, bch, xi, xl, yi, yl);
    }
  }

  if (this.tpadding) {
    xi += this.padding.left, xl -= this.padding.right;
    yi += this.padding.top, yl -= this.padding.bottom;
  }

  // Determine where to place the text if it's vertically aligned.
  if (this.valign === 'middle' || this.valign === 'bottom') {
    visible = yl - yi;
    if (this._clines.length < visible) {
      if (this.valign === 'middle') {
        visible = visible / 2 | 0;
        visible -= this._clines.length / 2 | 0;
      } else if (this.valign === 'bottom') {
        visible -= this._clines.length;
      }
      ci -= visible * (xl - xi);
    }
  }

  // Draw the content and background.
  for (y = yi; y < yl; y++) {
    if (!lines[y]) {
      if (y >= this.screen.height || yl < this.ibottom) {
        break;
      } else {
        continue;
      }
    }
    for (x = xi; x < ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype._wrapContent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>_wrapContent (content, width)](#apidoc.element.blessed.Element.prototype._wrapContent)
- description and source-code
```javascript
_wrapContent = function (content, width) {
  var tags = this.parseTags
    , state = this.align
    , wrap = this.wrap
    , margin = 0
    , rtof = []
    , ftor = []
    , out = []
    , no = 0
    , line
    , align
    , cap
    , total
    , i
    , part
    , j
    , lines
    , rest;

  lines = content.split('\n');

  if (!content) {
    out.push(content);
    out.rtof = [0];
    out.ftor = [[0]];
    out.fake = lines;
    out.real = out;
    out.mwidth = 0;
    return out;
  }

  if (this.scrollbar) margin++;
  if (this.type === 'textarea') margin++;
  if (width > margin) width -= margin;

main:
  for (; no < lines.length; no++) {
    line = lines[no];
    align = state;

    ftor.push([]);

    // Handle alignment tags.
    if (tags) {
      if (cap = /^{(left|center|right)}/.exec(line)) {
        line = line.substring(cap[0].length);
        align = state = cap[1] !== 'left'
          ? cap[1]
          : null;
      }
      if (cap = /{\/(left|center|right)}$/.exec(line)) {
        line = line.slice(0, -cap[0].length);
        //state = null;
        state = this.align;
      }
    }

    // If the string is apparently too long, wrap it.
    while (line.length > width) {
      // Measure the real width of the string.
      for (i = 0, total = 0; i < line.length; i++) {
        while (line[i] === '\x1b') {
          while (line[i] && line[i++] !== 'm');
        }
        if (!line[i]) break;
        if (++total === width) {
          // If we're not wrapping the text, we have to finish up the rest of
          // the control sequences before cutting off the line.
          i++;
          if (!wrap) {
            rest = line.substring(i).match(/\x1b\[[^m]*m/g);
            rest = rest ? rest.join('') : '';
            out.push(this._align(line.substring(0, i) + rest, width, align));
            ftor[no].push(out.length - 1);
            rtof.push(no);
            continue main;
          }
          if (!this.screen.fullUnicode) {
            // Try to find a space to break on.
            if (i !== line.length) {
              j = i;
              while (j > i - 10 && j > 0 && line[--j] !== ' ');
              if (line[j] === ' ') i = j + 1;
            }
          } else {
            // Try to find a character to break on.
            if (i !== line.length) {
              // <XXX>
              // Compensate for surrogate length
              // counts on wrapping (experimental):
              // NOTE: Could optimize this by putting
              // it in the parent for loop.
              if (unicode.isSurrogate(line, i)) i--;
              for (var s = 0, n = 0; n < i; n++) {
                if (unicode.isSurrogate(line, n)) s++, n++;
              }
              i += s;
              // </XXX>
              j = i;
              // Break _past_ space.
              // Break _past_ double-width chars.
              // Break _past_ surrogate pairs.
              // Break _past_ combining chars.
              while (j > i - 10 && j > 0) {
                j--;
                if (line[j] === ' '
                    || line[j] === '\x03'
                    || (unicode.isSurrogate(line, j - 1) && line[j + 1] !== '\x03')
                    || unicode.isCombining(line, j)) {
                  break;
                }
              }
              if (line[j] === ' '
                  || line[j] === '\x03'
                  || (unicode.isSurrogate(line, j - 1) && line[j + 1] !== '\x03')
                  || unicode.isCombining(line, j)) {
                i = j + 1;
              }
            }
          }
          break;
        }
      }

      part = line.substring(0, i);
      line = line.substring(i);

      out.push(this._align(part, width, align));
      ftor[no].push(out.length - 1);
      rtof.push(no);

      // Make sure we didn't wrap the line to the very end, otherwise
      // we get a pointless empty line after a newline.
      if (line === '') continue main;

      // If only an escape code got cut off, at it to 'part'.
      if (/^(?:\x1b[\[\d;]*m)+$/.test(line)) {
        out[out.length - 1] += line; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.clearBaseLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearBaseLine (i)](#apidoc.element.blessed.Element.prototype.clearBaseLine)
- description and source-code
```javascript
clearBaseLine = function (i) {
  var fake = this._clines.rtof[this.childBase || 0];
  return this.clearLine(fake + i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.clearLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearLine (i)](#apidoc.element.blessed.Element.prototype.clearLine)
- description and source-code
```javascript
clearLine = function (i) {
  i = Math.min(i, this._clines.fake.length - 1);
  return this.setLine(i, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.clearPos"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>clearPos (get, override)](#apidoc.element.blessed.Element.prototype.clearPos)
- description and source-code
```javascript
clearPos = function (get, override) {
  if (this.detached) return;
  var lpos = this._getCoords(get);
  if (!lpos) return;
  this.screen.clearRegion(
    lpos.xi, lpos.xl,
    lpos.yi, lpos.yl,
    override);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.deleteBottom"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteBottom (n)](#apidoc.element.blessed.Element.prototype.deleteBottom)
- description and source-code
```javascript
deleteBottom = function (n) {
  var h = (this.childBase || 0) + this.height - 1 - this.iheight
    , i = Math.min(h, this._clines.length - 1)
    , fake = this._clines.rtof[i];

  n = n || 1;

  return this.deleteLine(fake - (n - 1), n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.deleteLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteLine (i, n)](#apidoc.element.blessed.Element.prototype.deleteLine)
- description and source-code
```javascript
deleteLine = function (i, n) {
  n = n || 1;

  if (i !== i || i == null) {
    i = this._clines.ftor.length - 1;
  }

  i = Math.max(i, 0);
  i = Math.min(i, this._clines.ftor.length - 1);

  // NOTE: Could possibly compare the first and last ftor line numbers to see
  // if they're the same, or if they fit in the visible region entirely.
  var start = this._clines.length
    , diff
    , real = this._clines.ftor[i][0];

  while (n--) {
    this._clines.fake.splice(i, 1);
  }

  this.setContent(this._clines.fake.join('\n'), true);

  diff = start - this._clines.length;

  // XXX clearPos() without diff statement?
  var height = 0;

  if (diff > 0) {
    var pos = this._getCoords();
    if (!pos) return;

    height = pos.yl - pos.yi - this.iheight;

    var base = this.childBase || 0
      , visible = real >= base && real - base < height;

    if (pos && visible && this.screen.cleanSides(this)) {
      this.screen.deleteLine(diff,
        pos.yi + this.itop + real - base,
        pos.yi,
        pos.yl - this.ibottom - 1);
    }
  }

  if (this._clines.length < height) {
    this.clearPos();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.deleteTop"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>deleteTop (n)](#apidoc.element.blessed.Element.prototype.deleteTop)
- description and source-code
```javascript
deleteTop = function (n) {
  var fake = this._clines.rtof[this.childBase || 0];
  return this.deleteLine(fake, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.disableDrag"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>disableDrag ()](#apidoc.element.blessed.Element.prototype.disableDrag)
- description and source-code
```javascript
disableDrag = function () {
  if (!this._draggable) return false;
  delete this.screen._dragging;
  delete this._drag;
  this.removeListener('mousedown', this._dragMD);
  this.removeScreenEvent('mouse', this._dragM);
  return this._draggable = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.enableDrag"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableDrag (verify)](#apidoc.element.blessed.Element.prototype.enableDrag)
- description and source-code
```javascript
enableDrag = function (verify) {
  var self = this;

  if (this._draggable) return true;

  if (typeof verify !== 'function') {
    verify = function() { return true; };
  }

  this.enableMouse();

  this.on('mousedown', this._dragMD = function(data) {
    if (self.screen._dragging) return;
    if (!verify(data)) return;
    self.screen._dragging = self;
    self._drag = {
      x: data.x - self.aleft,
      y: data.y - self.atop
    };
    self.setFront();
  });

  this.onScreenEvent('mouse', this._dragM = function(data) {
    if (self.screen._dragging !== self) return;

    if (data.action !== 'mousedown' && data.action !== 'mousemove') {
      delete self.screen._dragging;
      delete self._drag;
      return;
    }

    // This can happen in edge cases where the user is
    // already dragging and element when it is detached.
    if (!self.parent) return;

    var ox = self._drag.x
      , oy = self._drag.y
      , px = self.parent.aleft
      , py = self.parent.atop
      , x = data.x - px - ox
      , y = data.y - py - oy;

    if (self.position.right != null) {
      if (self.position.left != null) {
        self.width = '100%-' + (self.parent.width - self.width);
      }
      self.position.right = null;
    }

    if (self.position.bottom != null) {
      if (self.position.top != null) {
        self.height = '100%-' + (self.parent.height - self.height);
      }
      self.position.bottom = null;
    }

    self.rleft = x;
    self.rtop = y;

    self.screen.render();
  });

  return this._draggable = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.enableInput"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableInput ()](#apidoc.element.blessed.Element.prototype.enableInput)
- description and source-code
```javascript
enableInput = function () {
  this.screen._listenMouse(this);
  this.screen._listenKeys(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.enableKeys"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableKeys ()](#apidoc.element.blessed.Element.prototype.enableKeys)
- description and source-code
```javascript
enableKeys = function () {
  this.screen._listenKeys(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.enableMouse"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>enableMouse ()](#apidoc.element.blessed.Element.prototype.enableMouse)
- description and source-code
```javascript
enableMouse = function () {
  this.screen._listenMouse(this);
}
```
- example usage
```shell
...
- __resize__ - Received on screen resize.
- __mouse__ - Received on mouse events.
- __keypress__ - Received on key events.
- __element [name]__ - Global events received for all elements.
- __key [name]__ - Received on key event for [name].
- __focus, blur__ - Received when the terminal window focuses/blurs. Requires a
terminal supporting the focus protocol and focus needs to be passed to
program.enableMouse().
- __prerender__ - Received before render.
- __render__ - Received on render.
- __warning__ - Received when blessed notices something untoward (output is not
a tty, terminfo not found, etc).
- __destroy__ - Received when the screen is destroyed (only useful when using
multiple screens).
...
```

#### <a name="apidoc.element.blessed.Element.prototype.focus"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>focus ()](#apidoc.element.blessed.Element.prototype.focus)
- description and source-code
```javascript
focus = function () {
  return this.screen.focused = this;
}
```
- example usage
```shell
...

// Quit on Escape, q, or Control-C.
screen.key(['escape', 'q', 'C-c'], function(ch, key) {
  return process.exit(0);
});

// Focus our element.
box.focus();

// Render the screen.
screen.render();
'''

## Documentation
...
```

#### <a name="apidoc.element.blessed.Element.prototype.free"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>free ()](#apidoc.element.blessed.Element.prototype.free)
- description and source-code
```javascript
free = function () {
  var listeners = this._slisteners = this._slisteners || [];
  for (var i = 0; i < listeners.length; i++) {
    var listener = listeners[i];
    this.screen.removeListener(listener.type, listener.handler);
  }
  delete this._slisteners;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getBaseLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getBaseLine (i)](#apidoc.element.blessed.Element.prototype.getBaseLine)
- description and source-code
```javascript
getBaseLine = function (i) {
  var fake = this._clines.rtof[this.childBase || 0];
  return this.getLine(fake + i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getContent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getContent ()](#apidoc.element.blessed.Element.prototype.getContent)
- description and source-code
```javascript
getContent = function () {
  if (!this._clines) return '';
  return this._clines.fake.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getLine (i)](#apidoc.element.blessed.Element.prototype.getLine)
- description and source-code
```javascript
getLine = function (i) {
  i = Math.max(i, 0);
  i = Math.min(i, this._clines.fake.length - 1);
  return this._clines.fake[i];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getLines"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getLines ()](#apidoc.element.blessed.Element.prototype.getLines)
- description and source-code
```javascript
getLines = function () {
  return this._clines.fake.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getScreenLines"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getScreenLines ()](#apidoc.element.blessed.Element.prototype.getScreenLines)
- description and source-code
```javascript
getScreenLines = function () {
  return this._clines.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.getText"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>getText ()](#apidoc.element.blessed.Element.prototype.getText)
- description and source-code
```javascript
getText = function () {
  return this.getContent().replace(/\x1b\[[\d;]*m/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.hide"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>hide ()](#apidoc.element.blessed.Element.prototype.hide)
- description and source-code
```javascript
hide = function () {
  if (this.hidden) return;
  this.clearPos();
  this.hidden = true;
  this.emit('hide');
  if (this.screen.focused === this) {
    this.screen.rewindFocus();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.insertBottom"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertBottom (line)](#apidoc.element.blessed.Element.prototype.insertBottom)
- description and source-code
```javascript
insertBottom = function (line) {
  var h = (this.childBase || 0) + this.height - this.iheight
    , i = Math.min(h, this._clines.length)
    , fake = this._clines.rtof[i - 1] + 1;

  return this.insertLine(fake, line);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.insertLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertLine (i, line)](#apidoc.element.blessed.Element.prototype.insertLine)
- description and source-code
```javascript
insertLine = function (i, line) {
  if (typeof line === 'string') line = line.split('\n');

  if (i !== i || i == null) {
    i = this._clines.ftor.length;
  }

  i = Math.max(i, 0);

  while (this._clines.fake.length < i) {
    this._clines.fake.push('');
    this._clines.ftor.push([this._clines.push('') - 1]);
    this._clines.rtof(this._clines.fake.length - 1);
  }

  // NOTE: Could possibly compare the first and last ftor line numbers to see
  // if they're the same, or if they fit in the visible region entirely.
  var start = this._clines.length
    , diff
    , real;

  if (i >= this._clines.ftor.length) {
    real = this._clines.ftor[this._clines.ftor.length - 1];
    real = real[real.length - 1] + 1;
  } else {
    real = this._clines.ftor[i][0];
  }

  for (var j = 0; j < line.length; j++) {
    this._clines.fake.splice(i + j, 0, line[j]);
  }

  this.setContent(this._clines.fake.join('\n'), true);

  diff = this._clines.length - start;

  if (diff > 0) {
    var pos = this._getCoords();
    if (!pos) return;

    var height = pos.yl - pos.yi - this.iheight
      , base = this.childBase || 0
      , visible = real >= base && real - base < height;

    if (pos && visible && this.screen.cleanSides(this)) {
      this.screen.insertLine(diff,
        pos.yi + this.itop + real - base,
        pos.yi,
        pos.yl - this.ibottom - 1);
    }
  }
}
```
- example usage
```shell
...
  screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
  box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
  box.setLine(1, 'bar');
  box.insertLine(1, 'foo');
  screen.render();
});

// Quit on Escape, q, or Control-C.
screen.key(['escape', 'q', 'C-c'], function(ch, key) {
  return process.exit(0);
});
...
```

#### <a name="apidoc.element.blessed.Element.prototype.insertTop"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>insertTop (line)](#apidoc.element.blessed.Element.prototype.insertTop)
- description and source-code
```javascript
insertTop = function (line) {
  var fake = this._clines.rtof[this.childBase || 0];
  return this.insertLine(fake, line);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.key"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>key ()](#apidoc.element.blessed.Element.prototype.key)
- description and source-code
```javascript
key = function () {
  return this.screen.program.key.apply(this, arguments);
}
```
- example usage
```shell
...
// If our box is clicked, change the content.
box.on('click', function(data) {
  box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
  screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
  box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
  box.setLine(1, 'bar');
  box.insertLine(1, 'foo');
  screen.render();
});

// Quit on Escape, q, or Control-C.
...
```

#### <a name="apidoc.element.blessed.Element.prototype.onScreenEvent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.onScreenEvent)
- description and source-code
```javascript
onScreenEvent = function (type, handler) {
  var listeners = this._slisteners = this._slisteners || [];
  listeners.push({ type: type, handler: handler });
  this.screen.on(type, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.onceKey"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onceKey ()](#apidoc.element.blessed.Element.prototype.onceKey)
- description and source-code
```javascript
onceKey = function () {
  return this.screen.program.onceKey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.onceScreenEvent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>onceScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.onceScreenEvent)
- description and source-code
```javascript
onceScreenEvent = function (type, handler) {
  var listeners = this._slisteners = this._slisteners || [];
  var entry = { type: type, handler: handler };
  listeners.push(entry);
  this.screen.once(type, function() {
    var i = listeners.indexOf(entry);
    if (~i) listeners.splice(i, 1);
    return handler.apply(this, arguments);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.parseContent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>parseContent (noTags)](#apidoc.element.blessed.Element.prototype.parseContent)
- description and source-code
```javascript
parseContent = function (noTags) {
  if (this.detached) return false;

  var width = this.width - this.iwidth;
  if (this._clines == null
      || this._clines.width !== width
      || this._clines.content !== this.content) {
    var content = this.content;

    content = content
      .replace(/[\x00-\x08\x0b-\x0c\x0e-\x1a\x1c-\x1f\x7f]/g, '')
      .replace(/\x1b(?!\[[\d;]*m)/g, '')
      .replace(/\r\n|\r/g, '\n')
      .replace(/\t/g, this.screen.tabc);

    if (this.screen.fullUnicode) {
      // double-width chars will eat the next char after render. create a
      // blank character after it so it doesn't eat the real next char.
      content = content.replace(unicode.chars.all, '$1\x03');
      // iTerm2 cannot render combining characters properly.
      if (this.screen.program.isiTerm2) {
        content = content.replace(unicode.chars.combining, '');
      }
    } else {
      // no double-width: replace them with question-marks.
      content = content.replace(unicode.chars.all, '??');
      // delete combining characters since they're 0-width anyway.
      // NOTE: We could drop this, the non-surrogates would get changed to ? by
      // the unicode filter, and surrogates changed to ? by the surrogate
      // regex. however, the user might expect them to be 0-width.
      // NOTE: Might be better for performance to drop!
      content = content.replace(unicode.chars.combining, '');
      // no surrogate pairs: replace them with question-marks.
      content = content.replace(unicode.chars.surrogate, '?');
      // XXX Deduplicate code here:
      // content = helpers.dropUnicode(content);
    }

    if (!noTags) {
      content = this._parseTags(content);
    }

    this._clines = this._wrapContent(content, width);
    this._clines.width = width;
    this._clines.content = this.content;
    this._clines.attr = this._parseAttr(this._clines);
    this._clines.ci = [];
    this._clines.reduce(function(total, line) {
      this._clines.ci.push(total);
      return total + line.length + 1;
    }.bind(this), 0);

    this._pcontent = this._clines.join('\n');
    this.emit('parsed content');

    return true;
  }

  // Need to calculate this every time because the default fg/bg may change.
  this._clines.attr = this._parseAttr(this._clines) || this._clines.attr;

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.popLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>popLine (n)](#apidoc.element.blessed.Element.prototype.popLine)
- description and source-code
```javascript
popLine = function (n) {
  return this.deleteLine(this._clines.fake.length - 1, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.pushLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>pushLine (line)](#apidoc.element.blessed.Element.prototype.pushLine)
- description and source-code
```javascript
pushLine = function (line) {
  if (!this.content) return this.setLine(0, line);
  return this.insertLine(this._clines.fake.length, line);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.removeHover"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeHover ()](#apidoc.element.blessed.Element.prototype.removeHover)
- description and source-code
```javascript
removeHover = function () {
  delete this._hoverOptions;
  if (!this.screen._hoverText || this.screen._hoverText.detached) return;
  this.screen._hoverText.detach();
  this.screen.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.removeKey"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeKey ()](#apidoc.element.blessed.Element.prototype.removeKey)
- description and source-code
```javascript
removeKey = function () {
  return this.screen.program.unkey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.removeLabel"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeLabel ()](#apidoc.element.blessed.Element.prototype.removeLabel)
- description and source-code
```javascript
removeLabel = function () {
  if (!this._label) return;
  this.removeListener('scroll', this._labelScroll);
  this.removeListener('resize', this._labelResize);
  this._label.detach();
  delete this._labelScroll;
  delete this._labelResize;
  delete this._label;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.removeScreenEvent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>removeScreenEvent (type, handler)](#apidoc.element.blessed.Element.prototype.removeScreenEvent)
- description and source-code
```javascript
removeScreenEvent = function (type, handler) {
  var listeners = this._slisteners = this._slisteners || [];
  for (var i = 0; i < listeners.length; i++) {
    var listener = listeners[i];
    if (listener.type === type && listener.handler === handler) {
      listeners.splice(i, 1);
      if (this._slisteners.length === 0) {
        delete this._slisteners;
      }
      break;
    }
  }
  this.screen.removeListener(type, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>render ()](#apidoc.element.blessed.Element.prototype.render)
- description and source-code
```javascript
render = function () {
  this._emit('prerender');

  this.parseContent();

  var coords = this._getCoords(true);
  if (!coords) {
    delete this.lpos;
    return;
  }

  if (coords.xl - coords.xi <= 0) {
    coords.xl = Math.max(coords.xl, coords.xi);
    return;
  }

  if (coords.yl - coords.yi <= 0) {
    coords.yl = Math.max(coords.yl, coords.yi);
    return;
  }

  var lines = this.screen.lines
    , xi = coords.xi
    , xl = coords.xl
    , yi = coords.yi
    , yl = coords.yl
    , x
    , y
    , cell
    , attr
    , ch
    , content = this._pcontent
    , ci = this._clines.ci[coords.base]
    , battr
    , dattr
    , c
    , visible
    , i
    , bch = this.ch;

  // Clip content if it's off the edge of the screen
  // if (xi + this.ileft < 0 || yi + this.itop < 0) {
  //   var clines = this._clines.slice();
  //   if (xi + this.ileft < 0) {
  //     for (var i = 0; i < clines.length; i++) {
  //       var t = 0;
  //       var csi = '';
  //       var csis = '';
  //       for (var j = 0; j < clines[i].length; j++) {
  //         while (clines[i][j] === '\x1b') {
  //           csi = '\x1b';
  //           while (clines[i][j++] !== 'm') csi += clines[i][j];
  //           csis += csi;
  //         }
  //         if (++t === -(xi + this.ileft) + 1) break;
  //       }
  //       clines[i] = csis + clines[i].substring(j);
  //     }
  //   }
  //   if (yi + this.itop < 0) {
  //     clines = clines.slice(-(yi + this.itop));
  //   }
  //   content = clines.join('\n');
  // }

  if (coords.base >= this._clines.ci.length) {
    ci = this._pcontent.length;
  }

  this.lpos = coords;

  if (this.border && this.border.type === 'line') {
    this.screen._borderStops[coords.yi] = true;
    this.screen._borderStops[coords.yl - 1] = true;
    // if (!this.screen._borderStops[coords.yi]) {
    //   this.screen._borderStops[coords.yi] = { xi: coords.xi, xl: coords.xl };
    // } else {
    //   if (this.screen._borderStops[coords.yi].xi > coords.xi) {
    //     this.screen._borderStops[coords.yi].xi = coords.xi;
    //   }
    //   if (this.screen._borderStops[coords.yi].xl < coords.xl) {
    //     this.screen._borderStops[coords.yi].xl = coords.xl;
    //   }
    // }
    // this.screen._borderStops[coords.yl - 1] = this.screen._borderStops[coords.yi];
  }

  dattr = this.sattr(this.style);
  attr = dattr;

  // If we're in a scrollable text box, check to
  // see which attributes this line starts with.
  if (ci > 0) {
    attr = this._clines.attr[Math.min(coords.base, this._clines.length - 1)];
  }

  if (this.border) xi++, xl--, yi++, yl--;

  // If we have padding/valign, that means the
  // content-drawing loop will skip a few cells/lines.
  // To deal with this, we can just fill the whole thing
  // ahead of time. This could be optimized.
  if (this.tpadding || (this.valign && this.valign !== 'top')) {
    if (this.style.transparent) {
      for (y = Math.max(yi, 0); y < yl; y++) {
        if (!lines[y]) break;
        for (x = Math.max(xi, 0); x < xl; x++) {
          if (!lines[y][x]) break;
          lines[y][x][0] = colors.blend(attr, lines[y][x][0]);
          // lines[y][x][1] = bch;
          lines[y].dirty = true;
        }
      }
    } else {
      this.screen.fillRegion(dattr, bch, xi, xl, yi, yl);
    }
  }

  if (this.tpadding) {
    xi += this.padding.left, xl -= this.padding.right;
    yi += this.padding.top, yl -= this.padding.bottom;
  }

  // Determine where to place the text if it's vertically aligned.
  if (this.valign === 'middle' || this.valign === 'bottom') {
    visible = yl - yi;
    if (this._clines.length < visible) {
      if (this.valign === 'middle') {
        visible = visible / 2 | 0;
        visible -= this._clines.length / 2 | 0;
      } else if (this.valign === 'bottom') {
        visible -= this._clines.length;
      }
      ci -= visible * (xl - xi);
    }
  }

  // Draw the content and background.
  for (y = yi; y < yl; y++) {
    if (!lines[y]) {
      if (y >= this.screen.height || yl < this.ibottom) {
        break;
      } else {
        continue;
      }
    }
    for (x = xi; x < ...
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.Element.prototype.sattr"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>sattr (style, fg, bg)](#apidoc.element.blessed.Element.prototype.sattr)
- description and source-code
```javascript
sattr = function (style, fg, bg) {
  var bold = style.bold
    , underline = style.underline
    , blink = style.blink
    , inverse = style.inverse
    , invisible = style.invisible;

  // if (arguments.length === 1) {
  if (fg == null && bg == null) {
    fg = style.fg;
    bg = style.bg;
  }

  // This used to be a loop, but I decided
  // to unroll it for performance's sake.
  if (typeof bold === 'function') bold = bold(this);
  if (typeof underline === 'function') underline = underline(this);
  if (typeof blink === 'function') blink = blink(this);
  if (typeof inverse === 'function') inverse = inverse(this);
  if (typeof invisible === 'function') invisible = invisible(this);

  if (typeof fg === 'function') fg = fg(this);
  if (typeof bg === 'function') bg = bg(this);

  // return (this.uid << 24)
  //   | ((this.dockBorders ? 32 : 0) << 18)
  return ((invisible ? 16 : 0) << 18)
    | ((inverse ? 8 : 0) << 18)
    | ((blink ? 4 : 0) << 18)
    | ((underline ? 2 : 0) << 18)
    | ((bold ? 1 : 0) << 18)
    | (colors.convert(fg) << 9)
    | colors.convert(bg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.screenshot"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>screenshot (xi, xl, yi, yl)](#apidoc.element.blessed.Element.prototype.screenshot)
- description and source-code
```javascript
screenshot = function (xi, xl, yi, yl) {
  xi = this.lpos.xi + this.ileft + (xi || 0);
  if (xl != null) {
    xl = this.lpos.xi + this.ileft + (xl || 0);
  } else {
    xl = this.lpos.xl - this.iright;
  }
  yi = this.lpos.yi + this.itop + (yi || 0);
  if (yl != null) {
    yl = this.lpos.yi + this.itop + (yl || 0);
  } else {
    yl = this.lpos.yl - this.ibottom;
  }
  return this.screen.screenshot(xi, xl, yi, yl);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setBack"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setBack ()](#apidoc.element.blessed.Element.prototype.setBack)
- description and source-code
```javascript
setBack = function () {
  return this.setIndex(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setBaseLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setBaseLine (i, line)](#apidoc.element.blessed.Element.prototype.setBaseLine)
- description and source-code
```javascript
setBaseLine = function (i, line) {
  var fake = this._clines.rtof[this.childBase || 0];
  return this.setLine(fake + i, line);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setContent"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setContent (content, noClear, noTags)](#apidoc.element.blessed.Element.prototype.setContent)
- description and source-code
```javascript
setContent = function (content, noClear, noTags) {
  if (!noClear) this.clearPos();
  this.content = content || '';
  this.parseContent(noTags);
  this.emit('set content');
}
```
- example usage
```shell
...
height: 'shrink',
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
...
```

#### <a name="apidoc.element.blessed.Element.prototype.setFront"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setFront ()](#apidoc.element.blessed.Element.prototype.setFront)
- description and source-code
```javascript
setFront = function () {
  return this.setIndex(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setHover"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setHover (options)](#apidoc.element.blessed.Element.prototype.setHover)
- description and source-code
```javascript
setHover = function (options) {
  if (typeof options === 'string') {
    options = { text: options };
  }

  this._hoverOptions = options;
  this.enableMouse();
  this.screen._initHover();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setIndex"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setIndex (index)](#apidoc.element.blessed.Element.prototype.setIndex)
- description and source-code
```javascript
setIndex = function (index) {
  if (!this.parent) return;

  if (index < 0) {
    index = this.parent.children.length + index;
  }

  index = Math.max(index, 0);
  index = Math.min(index, this.parent.children.length - 1);

  var i = this.parent.children.indexOf(this);
  if (!~i) return;

  var item = this.parent.children.splice(i, 1)[0];
  this.parent.children.splice(index, 0, item);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setLabel"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setLabel (options)](#apidoc.element.blessed.Element.prototype.setLabel)
- description and source-code
```javascript
setLabel = function (options) {
  var self = this;
  var Box = require('./box');

  if (typeof options === 'string') {
    options = { text: options };
  }

  if (this._label) {
    this._label.setContent(options.text);
    if (options.side !== 'right') {
      this._label.rleft = 2 + (this.border ? -1 : 0);
      this._label.position.right = undefined;
      if (!this.screen.autoPadding) {
        this._label.rleft = 2;
      }
    } else {
      this._label.rright = 2 + (this.border ? -1 : 0);
      this._label.position.left = undefined;
      if (!this.screen.autoPadding) {
        this._label.rright = 2;
      }
    }
    return;
  }

  this._label = new Box({
    screen: this.screen,
    parent: this,
    content: options.text,
    top: -this.itop,
    tags: this.parseTags,
    shrink: true,
    style: this.style.label
  });

  if (options.side !== 'right') {
    this._label.rleft = 2 - this.ileft;
  } else {
    this._label.rright = 2 - this.iright;
  }

  this._label._isLabel = true;

  if (!this.screen.autoPadding) {
    if (options.side !== 'right') {
      this._label.rleft = 2;
    } else {
      this._label.rright = 2;
    }
    this._label.rtop = 0;
  }

  var reposition = function() {
    self._label.rtop = (self.childBase || 0) - self.itop;
    if (!self.screen.autoPadding) {
      self._label.rtop = (self.childBase || 0);
    }
    self.screen.render();
  };

  this.on('scroll', this._labelScroll = function() {
    reposition();
  });

  this.on('resize', this._labelResize = function() {
    nextTick(function() {
      reposition();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.setLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setLine (i, line)](#apidoc.element.blessed.Element.prototype.setLine)
- description and source-code
```javascript
setLine = function (i, line) {
  i = Math.max(i, 0);
  while (this._clines.fake.length < i) {
    this._clines.fake.push('');
  }
  this._clines.fake[i] = line;
  return this.setContent(this._clines.fake.join('\n'), true);
}
```
- example usage
```shell
...
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
screen.render();
});

// Quit on Escape, q, or Control-C.
screen.key(['escape', 'q', 'C-c'], function(ch, key) {
return process.exit(0);
...
```

#### <a name="apidoc.element.blessed.Element.prototype.setText"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>setText (content, noClear)](#apidoc.element.blessed.Element.prototype.setText)
- description and source-code
```javascript
setText = function (content, noClear) {
  content = content || '';
  content = content.replace(/\x1b\[[\d;]*m/g, '');
  return this.setContent(content, noClear, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.shiftLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>shiftLine (n)](#apidoc.element.blessed.Element.prototype.shiftLine)
- description and source-code
```javascript
shiftLine = function (n) {
  return this.deleteLine(0, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.show"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>show ()](#apidoc.element.blessed.Element.prototype.show)
- description and source-code
```javascript
show = function () {
  if (!this.hidden) return;
  this.hidden = false;
  this.emit('show');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.strWidth"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>strWidth (text)](#apidoc.element.blessed.Element.prototype.strWidth)
- description and source-code
```javascript
strWidth = function (text) {
  text = this.parseTags
    ? helpers.stripTags(text)
    : text;
  return this.screen.fullUnicode
    ? unicode.strWidth(text)
    : helpers.dropUnicode(text).length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.toggle"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>toggle ()](#apidoc.element.blessed.Element.prototype.toggle)
- description and source-code
```javascript
toggle = function () {
  return this.hidden ? this.show() : this.hide();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.unkey"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>unkey ()](#apidoc.element.blessed.Element.prototype.unkey)
- description and source-code
```javascript
unkey = function () {
  return this.screen.program.unkey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Element.prototype.unshiftLine"></a>[function <span class="apidocSignatureSpan">blessed.Element.prototype.</span>unshiftLine (line)](#apidoc.element.blessed.Element.prototype.unshiftLine)
- description and source-code
```javascript
unshiftLine = function (line) {
  return this.insertLine(0, line);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Program"></a>[module blessed.Program](#apidoc.module.blessed.Program)

#### <a name="apidoc.element.blessed.Program.Program"></a>[function <span class="apidocSignatureSpan">blessed.</span>Program (options)](#apidoc.element.blessed.Program.Program)
- description and source-code
```javascript
function Program(options) {
  var self = this;

  if (!(this instanceof Program)) {
    return new Program(options);
  }

  Program.bind(this);

  EventEmitter.call(this);

  if (!options || options.__proto__ !== Object.prototype) {
    options = {
      input: arguments[0],
      output: arguments[1]
    };
  }

  this.options = options;
  this.input = options.input || process.stdin;
  this.output = options.output || process.stdout;

  options.log = options.log || options.dump;
  if (options.log) {
    this._logger = fs.createWriteStream(options.log);
    if (options.dump) this.setupDump();
  }

  this.zero = options.zero !== false;
  this.useBuffer = options.buffer;

  this.x = 0;
  this.y = 0;
  this.savedX = 0;
  this.savedY = 0;

  this.cols = this.output.columns || 1;
  this.rows = this.output.rows || 1;

  this.scrollTop = 0;
  this.scrollBottom = this.rows - 1;

  this._terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this._terminal = this._terminal.toLowerCase();

  // OSX
  this.isOSXTerm = process.env.TERM_PROGRAM === 'Apple_Terminal';
  this.isiTerm2 = process.env.TERM_PROGRAM === 'iTerm.app'
    || !!process.env.ITERM_SESSION_ID;

  // VTE
  // NOTE: lxterminal does not provide an env variable to check for.
  // NOTE: gnome-terminal and sakura use a later version of VTE
  // which provides VTE_VERSION as well as supports SGR events.
  this.isXFCE = /xfce/i.test(process.env.COLORTERM);
  this.isTerminator = !!process.env.TERMINATOR_UUID;
  this.isLXDE = false;
  this.isVTE = !!process.env.VTE_VERSION
    || this.isXFCE
    || this.isTerminator
    || this.isLXDE;

  // xterm and rxvt - not accurate
  this.isRxvt = /rxvt/i.test(process.env.COLORTERM);
  this.isXterm = false;

  this.tmux = !!process.env.TMUX;
  this.tmuxVersion = (function() {
    if (!self.tmux) return 2;
    try {
      var version = cp.execFileSync('tmux', ['-V'], { encoding: 'utf8' });
      return +/^tmux ([\d.]+)/i.exec(version.trim().split('\n')[0])[1];
    } catch (e) {
      return 2;
    }
  })();

  this._buf = '';
  this._flush = this.flush.bind(this);

  if (options.tput !== false) {
    this.setupTput();
  }

  this.listen();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.bind"></a>[function <span class="apidocSignatureSpan">blessed.Program.</span>bind (program)](#apidoc.element.blessed.Program.bind)
- description and source-code
```javascript
bind = function (program) {
  if (!Program.global) {
    Program.global = program;
  }

  if (!~Program.instances.indexOf(program)) {
    Program.instances.push(program);
    program.index = Program.total;
    Program.total++;
  }

  if (Program._bound) return;
  Program._bound = true;

  unshiftEvent(process, 'exit', Program._exitHandler = function() {
    Program.instances.forEach(function(program) {
      // Potentially reset window title on exit:
      // if (program._originalTitle) {
      //   program.setTitle(program._originalTitle);
      // }
      // Ensure the buffer is flushed (it should
      // always be at this point, but who knows).
      program.flush();
      // Ensure _exiting is set (could technically
      // use process._exiting).
      program._exiting = true;
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Program.prototype"></a>[module blessed.Program.prototype](#apidoc.module.blessed.Program.prototype)

#### <a name="apidoc.element.blessed.Program.prototype.HPositionRelative"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>HPositionRelative (param)](#apidoc.element.blessed.Program.prototype.HPositionRelative)
- description and source-code
```javascript
HPositionRelative = function (param) {
  if (this.tput) return this.cuf(param);
  this.x += param || 1;
  this._ncoords();
  // Does not exist:
  // if (this.tput) return this.put.hpr(param);
  return this._write('\x1b[' + (param || '') + 'a');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.HVPosition"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>HVPosition (row, col)](#apidoc.element.blessed.Program.prototype.HVPosition)
- description and source-code
```javascript
HVPosition = function (row, col) {
  if (!this.zero) {
    row = (row || 1) - 1;
    col = (col || 1) - 1;
  } else {
    row = row || 0;
    col = col || 0;
  }
  this.y = row;
  this.x = col;
  this._ncoords();
  // Does not exist (?):
  // if (this.tput) return this.put.hvp(row, col);
  if (this.tput) return this.put.cup(row, col);
  return this._write('\x1b[' + (row + 1) + ';' + (col + 1) + 'f');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.VPositionRelative"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>VPositionRelative (param)](#apidoc.element.blessed.Program.prototype.VPositionRelative)
- description and source-code
```javascript
VPositionRelative = function (param) {
  if (this.tput) return this.cud(param);
  this.y += param || 1;
  this._ncoords();
  // Does not exist:
  // if (this.tput) return this.put.vpr(param);
  return this._write('\x1b[' + (param || '') + 'e');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._attr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_attr (param, val)](#apidoc.element.blessed.Program.prototype._attr)
- description and source-code
```javascript
_attr = function (param, val) {
  var self = this
    , parts
    , color
    , m;

  if (Array.isArray(param)) {
    parts = param;
    param = parts[0] || 'normal';
  } else {
    param = param || 'normal';
    parts = param.split(/\s*[,;]\s*/);
  }

  if (parts.length > 1) {
    var used = {}
      , out = [];

    parts.forEach(function(part) {
      part = self._attr(part, val).slice(2, -1);
      if (part === '') return;
      if (used[part]) return;
      used[part] = true;
      out.push(part);
    });

    return '\x1b[' + out.join(';') + 'm';
  }

  if (param.indexOf('no ') === 0) {
    param = param.substring(3);
    val = false;
  } else if (param.indexOf('!') === 0) {
    param = param.substring(1);
    val = false;
  }

  switch (param) {
    // attributes
    case 'normal':
    case 'default':
      if (val === false) return '';
      return '\x1b[m';
    case 'bold':
      return val === false
        ? '\x1b[22m'
        : '\x1b[1m';
    case 'ul':
    case 'underline':
    case 'underlined':
      return val === false
        ? '\x1b[24m'
        : '\x1b[4m';
    case 'blink':
      return val === false
        ? '\x1b[25m'
        : '\x1b[5m';
    case 'inverse':
      return val === false
        ? '\x1b[27m'
        : '\x1b[7m';
    case 'invisible':
      return val === false
        ? '\x1b[28m'
        : '\x1b[8m';

    // 8-color foreground
    case 'black fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[30m';
    case 'red fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[31m';
    case 'green fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[32m';
    case 'yellow fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[33m';
    case 'blue fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[34m';
    case 'magenta fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[35m';
    case 'cyan fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[36m';
    case 'white fg':
    case 'light grey fg':
    case 'light gray fg':
    case 'bright grey fg':
    case 'bright gray fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[37m';
    case 'default fg':
      if (val === false) return '';
      return '\x1b[39m';

    // 8-color background
    case 'black bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[40m';
    case 'red bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[41m';
    case 'green bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[42m';
    case 'yellow bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[43m';
    case 'blue bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[44m';
    case 'magenta bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[45m';
    case 'cyan bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[46m';
    case 'white bg':
    case 'light grey bg':
    case 'light gray bg':
    case 'bright grey bg':
    case 'bright gray bg':
      return val === false
        ? '\x1b[49m'
        : '\x1b[47m';
    case 'default bg':
      if (val === false) return '';
      return '\x1b[49m';

    // 16-color foreground
    case 'light black fg':
    case 'bright black fg':
    case 'grey fg':
    case 'gray fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[90m';
    case 'light red fg':
    case 'bright red fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[91m';
    case 'light green fg':
    case 'bright green fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[92m';
    case 'light yellow fg':
    case 'bright yellow fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[93m';
    case 'light blue fg':
    case 'bright blue fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[94m';
    case 'light magenta fg':
    case 'bright magenta fg':
      return val === false
        ? '\x1b[39m'
        : '\x1b[95m';
    case 'light cyan fg':
    case 'b ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._bindMouse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_bindMouse (s, buf)](#apidoc.element.blessed.Program.prototype._bindMouse)
- description and source-code
```javascript
_bindMouse = function (s, buf) {
  var self = this
    , key
    , parts
    , b
    , x
    , y
    , mod
    , params
    , down
    , page
    , button;

  key = {
    name: undefined,
    ctrl: false,
    meta: false,
    shift: false
  };

  if (Buffer.isBuffer(s)) {
    if (s[0] > 127 && s[1] === undefined) {
      s[0] -= 128;
      s = '\x1b' + s.toString('utf-8');
    } else {
      s = s.toString('utf-8');
    }
  }

  // if (this.8bit) {
  //   s = s.replace(/\233/g, '\x1b[');
  //   buf = new Buffer(s, 'utf8');
  // }

  // XTerm / X10 for buggy VTE
  // VTE can only send unsigned chars and no unicode for coords. This limits
  // them to 0xff. However, normally the x10 protocol does not allow a byte
  // under 0x20, but since VTE can have the bytes overflow, we can consider
  // bytes below 0x20 to be up to 0xff + 0x20. This gives a limit of 287. Since
  // characters ranging from 223 to 248 confuse javascript's utf parser, we
  // need to parse the raw binary. We can detect whether the terminal is using
  // a bugged VTE version by examining the coordinates and seeing whether they
  // are a value they would never otherwise be with a properly implemented x10
  // protocol. This method of detecting VTE is only 99% reliable because we
  // can't check if the coords are 0x00 (255) since that is a valid x10 coord
  // technically.
  var bx = s.charCodeAt(4);
  var by = s.charCodeAt(5);
  if (buf[0] === 0x1b && buf[1] === 0x5b && buf[2] === 0x4d
      && (this.isVTE
      || bx >= 65533 || by >= 65533
      || (bx > 0x00 && bx < 0x20)
      || (by > 0x00 && by < 0x20)
      || (buf[4] > 223 && buf[4] < 248 && buf.length === 6)
      || (buf[5] > 223 && buf[5] < 248 && buf.length === 6))) {
    b = buf[3];
    x = buf[4];
    y = buf[5];

    // unsigned char overflow.
    if (x < 0x20) x += 0xff;
    if (y < 0x20) y += 0xff;

    // Convert the coordinates into a
    // properly formatted x10 utf8 sequence.
    s = '\x1b[M'
      + String.fromCharCode(b)
      + String.fromCharCode(x)
      + String.fromCharCode(y);
  }

  // XTerm / X10
  if (parts = /^\x1b\[M([\x00\u0020-\uffff]{3})/.exec(s)) {
    b = parts[1].charCodeAt(0);
    x = parts[1].charCodeAt(1);
    y = parts[1].charCodeAt(2);

    key.name = 'mouse';
    key.type = 'X10';

    key.raw = [b, x, y, parts[0]];
    key.buf = buf;
    key.x = x - 32;
    key.y = y - 32;

    if (this.zero) key.x--, key.y--;

    if (x === 0) key.x = 255;
    if (y === 0) key.y = 255;

    mod = b >> 2;
    key.shift = !!(mod & 1);
    key.meta = !!((mod >> 1) & 1);
    key.ctrl = !!((mod >> 2) & 1);

    b -= 32;

    if ((b >> 6) & 1) {
      key.action = b & 1 ? 'wheeldown' : 'wheelup';
      key.button = 'middle';
    } else if (b === 3) {
      // NOTE: x10 and urxvt have no way
      // of telling which button mouseup used.
      key.action = 'mouseup';
      key.button = this._lastButton || 'unknown';
      delete this._lastButton;
    } else {
      key.action = 'mousedown';
      button = b & 3;
      key.button =
        button === 0 ? 'left'
        : button === 1 ? 'middle'
        : button === 2 ? 'right'
        : 'unknown';
      this._lastButton = key.button;
    }

    // Probably a movement.
    // The *newer* VTE gets mouse movements comepletely wrong.
    // This presents a problem: older versions of VTE that get it right might
    // be confused by the second conditional in the if statement.
    // NOTE: Possibly just switch back to the if statement below.
    // none, shift, ctrl, alt
    // gnome: 32, 36, 48, 40
    // xterm: 35, _, 51, _
    // urxvt: 35, _, _, _
    // if (key.action === 'mousedown' && key.button === 'unknown') {
    if (b === 35 || b === 39 || b === 51 || b === 43
        || (this.isVTE && (b === 32 || b === 36 || b === 48 || b === 40))) {
      delete key.button;
      key.action = 'mousemove';
    }

    self.emit('mouse', key);

    return;
  }

  // URxvt
  if (parts = /^\x1b\[(\d+;\d+;\d+)M/.exec(s)) {
    params = parts[1].split(';');
    b = +params[0];
    x = +params[1];
    y = +params[2];

    key.name = 'mouse';
    key.type = 'u ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._bindResponse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_bindResponse (s)](#apidoc.element.blessed.Program.prototype._bindResponse)
- description and source-code
```javascript
_bindResponse = function (s) {
  var out = {}
    , parts;

  if (Buffer.isBuffer(s)) {
    if (s[0] > 127 && s[1] === undefined) {
      s[0] -= 128;
      s = '\x1b' + s.toString('utf-8');
    } else {
      s = s.toString('utf-8');
    }
  }

  // CSI P s c
  // Send Device Attributes (Primary DA).
  // CSI > P s c
  // Send Device Attributes (Secondary DA).
  if (parts = /^\x1b\[(\?|>)(\d*(?:;\d*)*)c/.exec(s)) {
    parts = parts[2].split(';').map(function(ch) {
      return +ch || 0;
    });

    out.event = 'device-attributes';
    out.code = 'DA';

    if (parts[1] === '?') {
      out.type = 'primary-attribute';
      // VT100-style params:
      if (parts[0] === 1 && parts[2] === 2) {
        out.term = 'vt100';
        out.advancedVideo = true;
      } else if (parts[0] === 1 && parts[2] === 0) {
        out.term = 'vt101';
      } else if (parts[0] === 6) {
        out.term = 'vt102';
      } else if (parts[0] === 60
        && parts[1] === 1 && parts[2] === 2
        && parts[3] === 6 && parts[4] === 8
        && parts[5] === 9 && parts[6] === 15) {
        out.term = 'vt220';
      } else {
        // VT200-style params:
        parts.forEach(function(attr) {
          switch (attr) {
            case 1:
              out.cols132 = true;
              break;
            case 2:
              out.printer = true;
              break;
            case 6:
              out.selectiveErase = true;
              break;
            case 8:
              out.userDefinedKeys = true;
              break;
            case 9:
              out.nationalReplacementCharsets = true;
              break;
            case 15:
              out.technicalCharacters = true;
              break;
            case 18:
              out.userWindows = true;
              break;
            case 21:
              out.horizontalScrolling = true;
              break;
            case 22:
              out.ansiColor = true;
              break;
            case 29:
              out.ansiTextLocator = true;
              break;
          }
        });
      }
    } else {
      out.type = 'secondary-attribute';
      switch (parts[0]) {
        case 0:
          out.term = 'vt100';
          break;
        case 1:
          out.term = 'vt220';
          break;
        case 2:
          out.term = 'vt240';
          break;
        case 18:
          out.term = 'vt330';
          break;
        case 19:
          out.term = 'vt340';
          break;
        case 24:
          out.term = 'vt320';
          break;
        case 41:
          out.term = 'vt420';
          break;
        case 61:
          out.term = 'vt510';
          break;
        case 64:
          out.term = 'vt520';
          break;
        case 65:
          out.term = 'vt525';
          break;
      }
      out.firmwareVersion = parts[1];
      out.romCartridgeRegistrationNumber = parts[2];
    }

    // LEGACY
    out.deviceAttributes = out;

    this.emit('response', out);
    this.emit('response ' + out.event, out);

    return;
  }

  // CSI Ps n  Device Status Report (DSR).
  //     Ps = 5  -> Status Report.  Result (''OK'') is
  //   CSI 0 n
  // CSI ? Ps n
  //   Device Status Report (DSR, DEC-specific).
  //     Ps = 1 5  -> Report Printer status as CSI ? 1 0  n  (ready).
  //     or CSI ? 1 1  n  (not ready).
  //     Ps = 2 5  -> Report UDK status as CSI ? 2 0  n  (unlocked)
  //     or CSI ? 2 1  n  (locked).
  //     Ps = 2 6  -> Report Keyboard status as
  //   CSI ? 2 7  ;  1  ;  0  ;  0  n  (North American).
  //   The last two parameters apply to VT400 & up, and denote key-
  //   board ready and LK01 respectively.
  //     Ps = 5 3  -> Report Locator status as
  //   CSI ? 5 3  n  Locator available, if compiled-in, or
  //   CSI ? 5 0  n  No Locator, if not.
  if (parts = /^\x1b\[(\?)?(\d+)(?:;(\d+);(\d+);(\d+))?n/.exec(s)) {
    out.event = 'device-status';
    out.code = 'DSR';

    if (!parts[1] && parts[2] === '0' && !parts[3]) {
      out.type = 'device-status';
      out.status = 'OK';

      // LEGACY
      out.deviceStatus = out.status;

      this.emit('response ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._buffer"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_buffer (text)](#apidoc.element.blessed.Program.prototype._buffer)
- description and source-code
```javascript
_buffer = function (text) {
  if (this._exiting) {
    this.flush();
    this._owrite(text);
    return;
  }

  if (this._buf) {
    this._buf += text;
    return;
  }

  this._buf = text;

  nextTick(this._flush);

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._listenInput"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_listenInput ()](#apidoc.element.blessed.Program.prototype._listenInput)
- description and source-code
```javascript
_listenInput = function () {
  var keys = require('./keys')
    , self = this;

  // Input
  this.input.on('keypress', this.input._keypressHandler = function(ch, key) {
    key = key || { ch: ch };

    if (key.name === 'undefined'
        && (key.code === '[M' || key.code === '[I' || key.code === '[O')) {
      // A mouse sequence. The 'keys' module doesn't understand these.
      return;
    }

    if (key.name === 'undefined') {
      // Not sure what this is, but we should probably ignore it.
      return;
    }

    if (key.name === 'enter' && key.sequence === '\n') {
      key.name = 'linefeed';
    }

    if (key.name === 'return' && key.sequence === '\r') {
      self.input.emit('keypress', ch, merge({}, key, { name: 'enter' }));
    }

    var name = (key.ctrl ? 'C-' : '')
      + (key.meta ? 'M-' : '')
      + (key.shift && key.name ? 'S-' : '')
      + (key.name || ch);

    key.full = name;

    Program.instances.forEach(function(program) {
      if (program.input !== self.input) return;
      program.emit('keypress', ch, key);
      program.emit('key ' + name, ch, key);
    });
  });

  this.input.on('data', this.input._dataHandler = function(data) {
    Program.instances.forEach(function(program) {
      if (program.input !== self.input) return;
      program.emit('data', data);
    });
  });

  keys.emitKeypressEvents(this.input);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._listenOutput"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_listenOutput ()](#apidoc.element.blessed.Program.prototype._listenOutput)
- description and source-code
```javascript
_listenOutput = function () {
  var self = this;

  if (!this.output.isTTY) {
    nextTick(function() {
      self.emit('warning', 'Output is not a TTY');
    });
  }

  // Output
  function resize() {
    Program.instances.forEach(function(program) {
      if (program.output !== self.output) return;
      program.cols = program.output.columns;
      program.rows = program.output.rows;
      program.emit('resize');
    });
  }

  this.output.on('resize', this.output._resizeHandler = function() {
    Program.instances.forEach(function(program) {
      if (program.output !== self.output) return;
      if (!program.options.resizeTimeout) {
        return resize();
      }
      if (program._resizeTimer) {
        clearTimeout(program._resizeTimer);
        delete program._resizeTimer;
      }
      var time = typeof program.options.resizeTimeout === 'number'
        ? program.options.resizeTimeout
        : 300;
      program._resizeTimer = setTimeout(resize, time);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._log"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_log (pre, msg)](#apidoc.element.blessed.Program.prototype._log)
- description and source-code
```javascript
_log = function (pre, msg) {
  if (!this._logger) return;
  return this._logger.write(pre + ': ' + msg + '\n-\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._ncoords"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_ncoords ()](#apidoc.element.blessed.Program.prototype._ncoords)
- description and source-code
```javascript
_ncoords = function () {
  if (this.x < 0) this.x = 0;
  else if (this.x >= this.cols) this.x = this.cols - 1;
  if (this.y < 0) this.y = 0;
  else if (this.y >= this.rows) this.y = this.rows - 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._owrite"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_owrite (text)](#apidoc.element.blessed.Program.prototype._owrite)
- description and source-code
```javascript
_owrite = function (text) {
  if (!this.output.writable) return;
  return this.output.write(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._twrite"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_twrite (data)](#apidoc.element.blessed.Program.prototype._twrite)
- description and source-code
```javascript
_twrite = function (data) {
  var self = this
    , iterations = 0
    , timer;

  if (this.tmux) {
    // Replace all STs with BELs so they can be nested within the DCS code.
    data = data.replace(/\x1b\\/g, '\x07');

    // Wrap in tmux forward DCS:
    data = '\x1bPtmux;\x1b' + data + '\x1b\\';

    // If we've never even flushed yet, it means we're still in
    // the normal buffer. Wait for alt screen buffer.
    if (this.output.bytesWritten === 0) {
      timer = setInterval(function() {
        if (self.output.bytesWritten > 0 || ++iterations === 50) {
          clearInterval(timer);
          self.flush();
          self._owrite(data);
        }
      }, 100);
      return true;
    }

    // NOTE: Flushing the buffer is required in some cases.
    // The DCS code must be at the start of the output.
    this.flush();

    // Write out raw now that the buffer is flushed.
    return this._owrite(data);
  }

  return this._write(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype._write"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>_write (text)](#apidoc.element.blessed.Program.prototype._write)
- description and source-code
```javascript
_write = function (text) {
  if (this.ret) return text;
  if (this.useBuffer) {
    return this._buffer(text);
  }
  return this._owrite(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ae"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ae ()](#apidoc.element.blessed.Program.prototype.ae)
- description and source-code
```javascript
ae = function () {
  return this.charset('ascii');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.alternate"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>alternate ()](#apidoc.element.blessed.Program.prototype.alternate)
- description and source-code
```javascript
alternate = function () {
  this.isAlt = true;
  if (this.tput) return this.put.smcup();
  if (this.term('vt') || this.term('linux')) return;
  this.setMode('?47');
  return this.setMode('?1049');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.alternateBuffer"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>alternateBuffer ()](#apidoc.element.blessed.Program.prototype.alternateBuffer)
- description and source-code
```javascript
alternateBuffer = function () {
  this.isAlt = true;
  if (this.tput) return this.put.smcup();
  if (this.term('vt') || this.term('linux')) return;
  this.setMode('?47');
  return this.setMode('?1049');
}
```
- example usage
```shell
...
    program.move(data.x, data.y);
    program.bg('red');
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
program.enableMouse();
program.hideCursor();
program.clear();

program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
...
```

#### <a name="apidoc.element.blessed.Program.prototype.as"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>as ()](#apidoc.element.blessed.Program.prototype.as)
- description and source-code
```javascript
as = function () {
  return this.charset('acs');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.attr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>attr (param, val)](#apidoc.element.blessed.Program.prototype.attr)
- description and source-code
```javascript
attr = function (param, val) {
  return this._write(this._attr(param, val));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.back"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>back (param)](#apidoc.element.blessed.Program.prototype.back)
- description and source-code
```javascript
back = function (param) {
  this.x -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_left_cursor) {
      return this._write(this.repeat(this.tput.cub1(), param));
    }
    return this.put.cub(param);
  }
  return this._write('\x1b[' + (param || '') + 'D');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.backspace"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>backspace ()](#apidoc.element.blessed.Program.prototype.backspace)
- description and source-code
```javascript
backspace = function () {
  this.x--;
  this._ncoords();
  if (this.has('kbs')) return this.put.kbs();
  return this._write('\x08');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.bel"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bel ()](#apidoc.element.blessed.Program.prototype.bel)
- description and source-code
```javascript
bel = function () {
  if (this.has('bel')) return this.put.bel();
  return this._write('\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.bell"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bell ()](#apidoc.element.blessed.Program.prototype.bell)
- description and source-code
```javascript
bell = function () {
  if (this.has('bel')) return this.put.bel();
  return this._write('\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.bg"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bg (color, val)](#apidoc.element.blessed.Program.prototype.bg)
- description and source-code
```javascript
bg = function (color, val) {
  color = color.split(/\s*[,;]\s*/).join(' bg, ') + ' bg';
  return this.attr(color, val);
}
```
- example usage
```shell
...
  program.normalBuffer();
  process.exit(0);
});

program.on('mouse', function(data) {
  if (data.action === 'mousemove') {
    program.move(data.x, data.y);
    program.bg('red');
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
program.enableMouse();
...
```

#### <a name="apidoc.element.blessed.Program.prototype.bindMouse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bindMouse ()](#apidoc.element.blessed.Program.prototype.bindMouse)
- description and source-code
```javascript
bindMouse = function () {
  if (this._boundMouse) return;
  this._boundMouse = true;

  var decoder = new StringDecoder('utf8')
    , self = this;

  this.on('data', function(data) {
    var text = decoder.write(data);
    if (!text) return;
    self._bindMouse(text, data);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.bindResponse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>bindResponse ()](#apidoc.element.blessed.Program.prototype.bindResponse)
- description and source-code
```javascript
bindResponse = function () {
  if (this._boundResponse) return;
  this._boundResponse = true;

  var decoder = new StringDecoder('utf8')
    , self = this;

  this.on('data', function(data) {
    data = decoder.write(data);
    if (!data) return;
    self._bindResponse(data);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cbt"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cbt (param)](#apidoc.element.blessed.Program.prototype.cbt)
- description and source-code
```javascript
cbt = function (param) {
  this.x -= 8;
  this._ncoords();
  if (this.tput) return this.put.cbt(param);
  return this._write('\x1b[' + (param || 1) + 'Z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cha"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cha (param)](#apidoc.element.blessed.Program.prototype.cha)
- description and source-code
```javascript
cha = function (param) {
  if (!this.zero) {
    param = (param || 1) - 1;
  } else {
    param = param || 0;
  }
  this.x = param;
  this.y = 0;
  this._ncoords();
  if (this.tput) return this.put.hpa(param);
  return this._write('\x1b[' + (param + 1) + 'G');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.charAttributes"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charAttributes (param, val)](#apidoc.element.blessed.Program.prototype.charAttributes)
- description and source-code
```javascript
charAttributes = function (param, val) {
  return this._write(this._attr(param, val));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.charPosAbsolute"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charPosAbsolute (param)](#apidoc.element.blessed.Program.prototype.charPosAbsolute)
- description and source-code
```javascript
charPosAbsolute = function (param) {
  this.x = param || 0;
  this._ncoords();
  if (this.tput) {
    return this.put.hpa.apply(this.put, arguments);
  }
  param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + ''');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.charset"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>charset (val, level)](#apidoc.element.blessed.Program.prototype.charset)
- description and source-code
```javascript
charset = function (val, level) {
  level = level || 0;

  // See also:
  // acs_chars / acsc / ac
  // enter_alt_charset_mode / smacs / as
  // exit_alt_charset_mode / rmacs / ae
  // enter_pc_charset_mode / smpch / S2
  // exit_pc_charset_mode / rmpch / S3

  switch (level) {
    case 0:
      level = '(';
      break;
    case 1:
      level = ')';
      break;
    case 2:
      level = '*';
      break;
    case 3:
      level = '+';
      break;
  }

  var name = typeof val === 'string'
    ? val.toLowerCase()
    : val;

  switch (name) {
    case 'acs':
    case 'scld': // DEC Special Character and Line Drawing Set.
      if (this.tput) return this.put.smacs();
      val = '0';
      break;
    case 'uk': // UK
      val = 'A';
      break;
    case 'us': // United States (USASCII).
    case 'usascii':
    case 'ascii':
      if (this.tput) return this.put.rmacs();
      val = 'B';
      break;
    case 'dutch': // Dutch
      val = '4';
      break;
    case 'finnish': // Finnish
      val = 'C';
      val = '5';
      break;
    case 'french': // French
      val = 'R';
      break;
    case 'frenchcanadian': // FrenchCanadian
      val = 'Q';
      break;
    case 'german':  // German
      val = 'K';
      break;
    case 'italian': // Italian
      val = 'Y';
      break;
    case 'norwegiandanish': // NorwegianDanish
      val = 'E';
      val = '6';
      break;
    case 'spanish': // Spanish
      val = 'Z';
      break;
    case 'swedish': // Swedish
      val = 'H';
      val = '7';
      break;
    case 'swiss': // Swiss
      val = '=';
      break;
    case 'isolatin': // ISOLatin (actually /A)
      val = '/A';
      break;
    default: // Default
      if (this.tput) return this.put.rmacs();
      val = 'B';
      break;
  }

  return this._write('\x1b(' + val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cht"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cht (param)](#apidoc.element.blessed.Program.prototype.cht)
- description and source-code
```javascript
cht = function (param) {
  this.x += 8;
  this._ncoords();
  if (this.tput) return this.put.tab(param);
  return this._write('\x1b[' + (param || 1) + 'I');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.civis"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>civis ()](#apidoc.element.blessed.Program.prototype.civis)
- description and source-code
```javascript
civis = function () {
  this.cursorHidden = true;
  if (this.tput) return this.put.civis();
  return this.resetMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.clear"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>clear ()](#apidoc.element.blessed.Program.prototype.clear)
- description and source-code
```javascript
clear = function () {
  this.x = 0;
  this.y = 0;
  if (this.tput) return this.put.clear();
  return this._write('\x1b[H\x1b[J');
}
```
- example usage
```shell
...
The main functionality is exposed in the main 'blessed' module:

''' js
var blessed = require('blessed')
  , program = blessed.program();

program.key('q', function(ch, key) {
  program.clear();
  program.disableMouse();
  program.showCursor();
  program.normalBuffer();
  process.exit(0);
});

program.on('mouse', function(data) {
...
```

#### <a name="apidoc.element.blessed.Program.prototype.cnl"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cnl (param)](#apidoc.element.blessed.Program.prototype.cnl)
- description and source-code
```javascript
cnl = function (param) {
  this.y += param || 1;
  this._ncoords();
  return this._write('\x1b[' + (param || '') + 'E');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cnorm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cnorm ()](#apidoc.element.blessed.Program.prototype.cnorm)
- description and source-code
```javascript
cnorm = function () {
  this.cursorHidden = false;
  // NOTE: In xterm terminfo:
  // cnorm stops blinking cursor
  // cvvis starts blinking cursor
  if (this.tput) return this.put.cnorm();
  //if (this.tput) return this.put.cvvis();
  // return this._write('\x1b[?12l\x1b[?25h'); // cursor_normal
  // return this._write('\x1b[?12;25h'); // cursor_visible
  return this.setMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.copyRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>copyRectangle ()](#apidoc.element.blessed.Program.prototype.copyRectangle)
- description and source-code
```javascript
copyRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$v');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.copyToClipboard"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>copyToClipboard (text)](#apidoc.element.blessed.Program.prototype.copyToClipboard)
- description and source-code
```javascript
copyToClipboard = function (text) {
  if (this.isiTerm2) {
    this._twrite('\x1b]50;CopyToCliboard=' + text + '\x07');
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cpl"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cpl (param)](#apidoc.element.blessed.Program.prototype.cpl)
- description and source-code
```javascript
cpl = function (param) {
  this.y -= param || 1;
  this._ncoords();
  return this._write('\x1b[' + (param || '') + 'F');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cr ()](#apidoc.element.blessed.Program.prototype.cr)
- description and source-code
```javascript
cr = function () {
  this.x = 0;
  if (this.has('cr')) return this.put.cr();
  return this._write('\r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.csr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>csr (top, bottom)](#apidoc.element.blessed.Program.prototype.csr)
- description and source-code
```javascript
csr = function (top, bottom) {
  if (!this.zero) {
    top = (top || 1) - 1;
    bottom = (bottom || this.rows) - 1;
  } else {
    top = top || 0;
    bottom = bottom || (this.rows - 1);
  }
  this.scrollTop = top;
  this.scrollBottom = bottom;
  this.x = 0;
  this.y = 0;
  this._ncoords();
  if (this.tput) return this.put.csr(top, bottom);
  return this._write('\x1b[' + (top + 1) + ';' + (bottom + 1) + 'r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cub"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cub (param)](#apidoc.element.blessed.Program.prototype.cub)
- description and source-code
```javascript
cub = function (param) {
  this.x -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_left_cursor) {
      return this._write(this.repeat(this.tput.cub1(), param));
    }
    return this.put.cub(param);
  }
  return this._write('\x1b[' + (param || '') + 'D');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cud"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cud (param)](#apidoc.element.blessed.Program.prototype.cud)
- description and source-code
```javascript
cud = function (param) {
  this.y += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_down_cursor) {
      return this._write(this.repeat(this.tput.cud1(), param));
    }
    return this.put.cud(param);
  }
  return this._write('\x1b[' + (param || '') + 'B');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cuf"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cuf (param)](#apidoc.element.blessed.Program.prototype.cuf)
- description and source-code
```javascript
cuf = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_right_cursor) {
      return this._write(this.repeat(this.tput.cuf1(), param));
    }
    return this.put.cuf(param);
  }
  return this._write('\x1b[' + (param || '') + 'C');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cup"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cup (row, col)](#apidoc.element.blessed.Program.prototype.cup)
- description and source-code
```javascript
cup = function (row, col) {
  if (!this.zero) {
    row = (row || 1) - 1;
    col = (col || 1) - 1;
  } else {
    row = row || 0;
    col = col || 0;
  }
  this.x = col;
  this.y = row;
  this._ncoords();
  if (this.tput) return this.put.cup(row, col);
  return this._write('\x1b[' + (row + 1) + ';' + (col + 1) + 'H');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorBackward"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorBackward (param)](#apidoc.element.blessed.Program.prototype.cursorBackward)
- description and source-code
```javascript
cursorBackward = function (param) {
  this.x -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_left_cursor) {
      return this._write(this.repeat(this.tput.cub1(), param));
    }
    return this.put.cub(param);
  }
  return this._write('\x1b[' + (param || '') + 'D');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorBackwardTab"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorBackwardTab (param)](#apidoc.element.blessed.Program.prototype.cursorBackwardTab)
- description and source-code
```javascript
cursorBackwardTab = function (param) {
  this.x -= 8;
  this._ncoords();
  if (this.tput) return this.put.cbt(param);
  return this._write('\x1b[' + (param || 1) + 'Z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorCharAbsolute"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorCharAbsolute (param)](#apidoc.element.blessed.Program.prototype.cursorCharAbsolute)
- description and source-code
```javascript
cursorCharAbsolute = function (param) {
  if (!this.zero) {
    param = (param || 1) - 1;
  } else {
    param = param || 0;
  }
  this.x = param;
  this.y = 0;
  this._ncoords();
  if (this.tput) return this.put.hpa(param);
  return this._write('\x1b[' + (param + 1) + 'G');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorColor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorColor (color)](#apidoc.element.blessed.Program.prototype.cursorColor)
- description and source-code
```javascript
cursorColor = function (color) {
  if (this.term('xterm') || this.term('rxvt') || this.term('screen')) {
    this._twrite('\x1b]12;' + color + '\x07');
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorDown"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorDown (param)](#apidoc.element.blessed.Program.prototype.cursorDown)
- description and source-code
```javascript
cursorDown = function (param) {
  this.y += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_down_cursor) {
      return this._write(this.repeat(this.tput.cud1(), param));
    }
    return this.put.cud(param);
  }
  return this._write('\x1b[' + (param || '') + 'B');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorForward"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorForward (param)](#apidoc.element.blessed.Program.prototype.cursorForward)
- description and source-code
```javascript
cursorForward = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_right_cursor) {
      return this._write(this.repeat(this.tput.cuf1(), param));
    }
    return this.put.cuf(param);
  }
  return this._write('\x1b[' + (param || '') + 'C');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorForwardTab"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorForwardTab (param)](#apidoc.element.blessed.Program.prototype.cursorForwardTab)
- description and source-code
```javascript
cursorForwardTab = function (param) {
  this.x += 8;
  this._ncoords();
  if (this.tput) return this.put.tab(param);
  return this._write('\x1b[' + (param || 1) + 'I');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorNextLine"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorNextLine (param)](#apidoc.element.blessed.Program.prototype.cursorNextLine)
- description and source-code
```javascript
cursorNextLine = function (param) {
  this.y += param || 1;
  this._ncoords();
  return this._write('\x1b[' + (param || '') + 'E');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorPos"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorPos (row, col)](#apidoc.element.blessed.Program.prototype.cursorPos)
- description and source-code
```javascript
cursorPos = function (row, col) {
  if (!this.zero) {
    row = (row || 1) - 1;
    col = (col || 1) - 1;
  } else {
    row = row || 0;
    col = col || 0;
  }
  this.x = col;
  this.y = row;
  this._ncoords();
  if (this.tput) return this.put.cup(row, col);
  return this._write('\x1b[' + (row + 1) + ';' + (col + 1) + 'H');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorPrecedingLine"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorPrecedingLine (param)](#apidoc.element.blessed.Program.prototype.cursorPrecedingLine)
- description and source-code
```javascript
cursorPrecedingLine = function (param) {
  this.y -= param || 1;
  this._ncoords();
  return this._write('\x1b[' + (param || '') + 'F');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorReset"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorReset ()](#apidoc.element.blessed.Program.prototype.cursorReset)
- description and source-code
```javascript
cursorReset = function () {
  if (this.term('xterm') || this.term('rxvt') || this.term('screen')) {
    // XXX
    // return this.resetColors();
    this._twrite('\x1b[0 q');
    this._twrite('\x1b]112\x07');
    // urxvt doesnt support OSC 112
    this._twrite('\x1b]12;white\x07');
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorShape"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorShape (shape, blink)](#apidoc.element.blessed.Program.prototype.cursorShape)
- description and source-code
```javascript
cursorShape = function (shape, blink) {
  if (this.isiTerm2) {
    switch (shape) {
      case 'block':
        if (!blink) {
          this._twrite('\x1b]50;CursorShape=0;BlinkingCursorEnabled=0\x07');
        } else {
          this._twrite('\x1b]50;CursorShape=0;BlinkingCursorEnabled=1\x07');
        }
        break;
      case 'underline':
        if (!blink) {
          // this._twrite('\x1b]50;CursorShape=n;BlinkingCursorEnabled=0\x07');
        } else {
          // this._twrite('\x1b]50;CursorShape=n;BlinkingCursorEnabled=1\x07');
        }
        break;
      case 'line':
        if (!blink) {
          this._twrite('\x1b]50;CursorShape=1;BlinkingCursorEnabled=0\x07');
        } else {
          this._twrite('\x1b]50;CursorShape=1;BlinkingCursorEnabled=1\x07');
        }
        break;
    }
    return true;
  } else if (this.term('xterm') || this.term('screen')) {
    switch (shape) {
      case 'block':
        if (!blink) {
          this._twrite('\x1b[0 q');
        } else {
          this._twrite('\x1b[1 q');
        }
        break;
      case 'underline':
        if (!blink) {
          this._twrite('\x1b[2 q');
        } else {
          this._twrite('\x1b[3 q');
        }
        break;
      case 'line':
        if (!blink) {
          this._twrite('\x1b[4 q');
        } else {
          this._twrite('\x1b[5 q');
        }
        break;
    }
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursorUp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursorUp (param)](#apidoc.element.blessed.Program.prototype.cursorUp)
- description and source-code
```javascript
cursorUp = function (param) {
  this.y -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_up_cursor) {
      return this._write(this.repeat(this.tput.cuu1(), param));
    }
    return this.put.cuu(param);
  }
  return this._write('\x1b[' + (param || '') + 'A');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cursor_invisible"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cursor_invisible ()](#apidoc.element.blessed.Program.prototype.cursor_invisible)
- description and source-code
```javascript
cursor_invisible = function () {
  this.cursorHidden = true;
  if (this.tput) return this.put.civis();
  return this.resetMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cuu"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cuu (param)](#apidoc.element.blessed.Program.prototype.cuu)
- description and source-code
```javascript
cuu = function (param) {
  this.y -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_up_cursor) {
      return this._write(this.repeat(this.tput.cuu1(), param));
    }
    return this.put.cuu(param);
  }
  return this._write('\x1b[' + (param || '') + 'A');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.cvvis"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>cvvis ()](#apidoc.element.blessed.Program.prototype.cvvis)
- description and source-code
```javascript
cvvis = function () {
  this.cursorHidden = false;
  // NOTE: In xterm terminfo:
  // cnorm stops blinking cursor
  // cvvis starts blinking cursor
  if (this.tput) return this.put.cnorm();
  //if (this.tput) return this.put.cvvis();
  // return this._write('\x1b[?12l\x1b[?25h'); // cursor_normal
  // return this._write('\x1b[?12;25h'); // cursor_visible
  return this.setMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.da"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>da (param, callback)](#apidoc.element.blessed.Program.prototype.da)
- description and source-code
```javascript
da = function (param, callback) {
  return this.response('device-attributes',
    '\x1b[' + (param || '') + 'c', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.dch"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dch (param)](#apidoc.element.blessed.Program.prototype.dch)
- description and source-code
```javascript
dch = function (param) {
  if (this.tput) return this.put.dch(param);
  return this._write('\x1b[' + (param || '') + 'P');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.debug"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>debug ()](#apidoc.element.blessed.Program.prototype.debug)
- description and source-code
```javascript
debug = function () {
  if (!this.options.debug) return;
  return this._log('DEBUG',  util.format.apply(util, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.deccara"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deccara ()](#apidoc.element.blessed.Program.prototype.deccara)
- description and source-code
```javascript
deccara = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.deccra"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deccra ()](#apidoc.element.blessed.Program.prototype.deccra)
- description and source-code
```javascript
deccra = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$v');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decdc"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decdc ()](#apidoc.element.blessed.Program.prototype.decdc)
- description and source-code
```javascript
decdc = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + ' ~');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decefr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decefr ()](#apidoc.element.blessed.Program.prototype.decefr)
- description and source-code
```javascript
decefr = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'w');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decelr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decelr ()](#apidoc.element.blessed.Program.prototype.decelr)
- description and source-code
```javascript
decelr = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decera"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decera ()](#apidoc.element.blessed.Program.prototype.decera)
- description and source-code
```javascript
decera = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decfra"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decfra ()](#apidoc.element.blessed.Program.prototype.decfra)
- description and source-code
```javascript
decfra = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decic"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decic ()](#apidoc.element.blessed.Program.prototype.decic)
- description and source-code
```javascript
decic = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + ' }');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decll"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decll (param)](#apidoc.element.blessed.Program.prototype.decll)
- description and source-code
```javascript
decll = function (param) {
  return this._write('\x1b[' + (param || '') + 'q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decrara"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrara ()](#apidoc.element.blessed.Program.prototype.decrara)
- description and source-code
```javascript
decrara = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decreqtparm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decreqtparm (param)](#apidoc.element.blessed.Program.prototype.decreqtparm)
- description and source-code
```javascript
decreqtparm = function (param) {
  return this._write('\x1b[' + (param || 0) + 'x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decrqlp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqlp (param, callback)](#apidoc.element.blessed.Program.prototype.decrqlp)
- description and source-code
```javascript
decrqlp = function (param, callback) {
  // See also:
  // get_mouse / getm / Gm
  // mouse_info / minfo / Mi
  // Correct for tput?
  if (this.has('req_mouse_pos')) {
    var code = this.tput.req_mouse_pos(param);
    return this.response('locator-position', code, callback);
  }
  return this.response('locator-position',
    '\x1b[' + (param || '') + '\'|', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decrqm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqm (param)](#apidoc.element.blessed.Program.prototype.decrqm)
- description and source-code
```javascript
decrqm = function (param) {
  return this._write('\x1b[' + (param || '') + '$p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decrqmp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrqmp (param)](#apidoc.element.blessed.Program.prototype.decrqmp)
- description and source-code
```javascript
decrqmp = function (param) {
  return this._write('\x1b[?' + (param || '') + '$p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decrst"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decrst ()](#apidoc.element.blessed.Program.prototype.decrst)
- description and source-code
```javascript
decrst = function () {
  var param = slice.call(arguments).join(';');
  return this.resetMode('?' + param);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decsace"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsace (param)](#apidoc.element.blessed.Program.prototype.decsace)
- description and source-code
```javascript
decsace = function (param) {
  return this._write('\x1b[' + (param || 0) + 'x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decsca"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsca (param)](#apidoc.element.blessed.Program.prototype.decsca)
- description and source-code
```javascript
decsca = function (param) {
  return this._write('\x1b[' + (param || 0) + '"q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decscl"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decscl ()](#apidoc.element.blessed.Program.prototype.decscl)
- description and source-code
```javascript
decscl = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '"p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decscusr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decscusr (param)](#apidoc.element.blessed.Program.prototype.decscusr)
- description and source-code
```javascript
decscusr = function (param) {
  switch (param) {
    case 'blinking block':
      param = 1;
      break;
    case 'block':
    case 'steady block':
      param = 2;
      break;
    case 'blinking underline':
      param = 3;
      break;
    case 'underline':
    case 'steady underline':
      param = 4;
      break;
    case 'blinking bar':
      param = 5;
      break;
    case 'bar':
    case 'steady bar':
      param = 6;
      break;
  }
  if (param === 2 && this.has('Se')) {
    return this.put.Se();
  }
  if (this.has('Ss')) {
    return this.put.Ss(param);
  }
  return this._write('\x1b[' + (param || 1) + ' q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decsera"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsera ()](#apidoc.element.blessed.Program.prototype.decsera)
- description and source-code
```javascript
decsera = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '${');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decset"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decset ()](#apidoc.element.blessed.Program.prototype.decset)
- description and source-code
```javascript
decset = function () {
  var param = slice.call(arguments).join(';');
  return this.setMode('?' + param);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decsle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsle ()](#apidoc.element.blessed.Program.prototype.decsle)
- description and source-code
```javascript
decsle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'{');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decsmbv"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decsmbv (param)](#apidoc.element.blessed.Program.prototype.decsmbv)
- description and source-code
```javascript
decsmbv = function (param) {
  return this._write('\x1b[' + (param || '') + ' u');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decstbm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decstbm (top, bottom)](#apidoc.element.blessed.Program.prototype.decstbm)
- description and source-code
```javascript
decstbm = function (top, bottom) {
  if (!this.zero) {
    top = (top || 1) - 1;
    bottom = (bottom || this.rows) - 1;
  } else {
    top = top || 0;
    bottom = bottom || (this.rows - 1);
  }
  this.scrollTop = top;
  this.scrollBottom = bottom;
  this.x = 0;
  this.y = 0;
  this._ncoords();
  if (this.tput) return this.put.csr(top, bottom);
  return this._write('\x1b[' + (top + 1) + ';' + (bottom + 1) + 'r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decstr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decstr ()](#apidoc.element.blessed.Program.prototype.decstr)
- description and source-code
```javascript
decstr = function () {
  //if (this.tput) return this.put.init_2string();
  //if (this.tput) return this.put.reset_2string();
  if (this.tput) return this.put.rs2();
  //return this._write('\x1b[!p');
  //return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // init
  return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // reset
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.decswbv"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>decswbv (param)](#apidoc.element.blessed.Program.prototype.decswbv)
- description and source-code
```javascript
decswbv = function (param) {
  return this._write('\x1b[' + (param || '') + ' t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.dectcem"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dectcem ()](#apidoc.element.blessed.Program.prototype.dectcem)
- description and source-code
```javascript
dectcem = function () {
  this.cursorHidden = false;
  // NOTE: In xterm terminfo:
  // cnorm stops blinking cursor
  // cvvis starts blinking cursor
  if (this.tput) return this.put.cnorm();
  //if (this.tput) return this.put.cvvis();
  // return this._write('\x1b[?12l\x1b[?25h'); // cursor_normal
  // return this._write('\x1b[?12;25h'); // cursor_visible
  return this.setMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.dectcemh"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dectcemh ()](#apidoc.element.blessed.Program.prototype.dectcemh)
- description and source-code
```javascript
dectcemh = function () {
  this.cursorHidden = true;
  if (this.tput) return this.put.civis();
  return this.resetMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.deleteChars"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteChars (param)](#apidoc.element.blessed.Program.prototype.deleteChars)
- description and source-code
```javascript
deleteChars = function (param) {
  if (this.tput) return this.put.dch(param);
  return this._write('\x1b[' + (param || '') + 'P');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.deleteColumns"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteColumns ()](#apidoc.element.blessed.Program.prototype.deleteColumns)
- description and source-code
```javascript
deleteColumns = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + ' ~');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.deleteLines"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deleteLines (param)](#apidoc.element.blessed.Program.prototype.deleteLines)
- description and source-code
```javascript
deleteLines = function (param) {
  if (this.tput) return this.put.dl(param);
  return this._write('\x1b[' + (param || '') + 'M');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.destroy"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>destroy ()](#apidoc.element.blessed.Program.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var index = Program.instances.indexOf(this);

  if (~index) {
    Program.instances.splice(index, 1);
    Program.total--;

    this.flush();
    this._exiting = true;

    Program.global = Program.instances[0];

    if (Program.total === 0) {
      Program.global = null;

      process.removeListener('exit', Program._exitHandler);
      delete Program._exitHandler;

      delete Program._bound;
    }

    this.input._blessedInput--;
    this.output._blessedOutput--;

    if (this.input._blessedInput === 0) {
      this.input.removeListener('keypress', this.input._keypressHandler);
      this.input.removeListener('data', this.input._dataHandler);
      delete this.input._keypressHandler;
      delete this.input._dataHandler;

      if (this.input.setRawMode) {
        if (this.input.isRaw) {
          this.input.setRawMode(false);
        }
        if (!this.input.destroyed) {
          this.input.pause();
        }
      }
    }

    if (this.output._blessedOutput === 0) {
      this.output.removeListener('resize', this.output._resizeHandler);
      delete this.output._resizeHandler;
    }

    this.removeListener('newListener', this._newHandler);
    delete this._newHandler;

    this.destroyed = true;
    this.emit('destroy');
  }
}
```
- example usage
```shell
...
  output: client,
  terminal: 'xterm-256color',
  fullUnicode: true
});

client.on('close', function() {
  if (!screen.destroyed) {
    screen.destroy();
  }
});

screen.key(['C-c', 'q'], function(ch, key) {
  screen.destroy();
});
...
```

#### <a name="apidoc.element.blessed.Program.prototype.deviceStatus"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>deviceStatus (param, callback, dec, noBypass)](#apidoc.element.blessed.Program.prototype.deviceStatus)
- description and source-code
```javascript
deviceStatus = function (param, callback, dec, noBypass) {
  if (dec) {
    return this.response('device-status',
      '\x1b[?' + (param || '0') + 'n', callback, noBypass);
  }
  return this.response('device-status',
    '\x1b[' + (param || '0') + 'n', callback, noBypass);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.disableGpm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableGpm ()](#apidoc.element.blessed.Program.prototype.disableGpm)
- description and source-code
```javascript
disableGpm = function () {
  if (this.gpm) {
    this.gpm.stop();
    delete this.gpm;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.disableModifiers"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableModifiers (param)](#apidoc.element.blessed.Program.prototype.disableModifiers)
- description and source-code
```javascript
disableModifiers = function (param) {
  return this._write('\x1b[>' + (param || '') + 'n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.disableMouse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>disableMouse ()](#apidoc.element.blessed.Program.prototype.disableMouse)
- description and source-code
```javascript
disableMouse = function () {
  if (!this._currentMouse) return;

  var obj = {};

  Object.keys(this._currentMouse).forEach(function(key) {
    obj[key] = false;
  });

  return this.setMouse(obj, false);
}
```
- example usage
```shell
...

''' js
var blessed = require('blessed')
, program = blessed.program();

program.key('q', function(ch, key) {
program.clear();
program.disableMouse();
program.showCursor();
program.normalBuffer();
process.exit(0);
});

program.on('mouse', function(data) {
if (data.action === 'mousemove') {
...
```

#### <a name="apidoc.element.blessed.Program.prototype.dl"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dl (param)](#apidoc.element.blessed.Program.prototype.dl)
- description and source-code
```javascript
dl = function (param) {
  if (this.tput) return this.put.dl(param);
  return this._write('\x1b[' + (param || '') + 'M');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.down"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>down (param)](#apidoc.element.blessed.Program.prototype.down)
- description and source-code
```javascript
down = function (param) {
  this.y += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_down_cursor) {
      return this._write(this.repeat(this.tput.cud1(), param));
    }
    return this.put.cud(param);
  }
  return this._write('\x1b[' + (param || '') + 'B');
}
```
- example usage
```shell
...
program.hideCursor();
program.clear();

program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
program.setx((program.cols / 2 | 0) - 4);
program.down(5);
program.write('Hi again!');
program.bg('!black');
program.feed();
'''


#### Testing
...
```

#### <a name="apidoc.element.blessed.Program.prototype.dsr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dsr (param, callback, dec, noBypass)](#apidoc.element.blessed.Program.prototype.dsr)
- description and source-code
```javascript
dsr = function (param, callback, dec, noBypass) {
  if (dec) {
    return this.response('device-status',
      '\x1b[?' + (param || '0') + 'n', callback, noBypass);
  }
  return this.response('device-status',
    '\x1b[' + (param || '0') + 'n', callback, noBypass);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.dynamicColors"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>dynamicColors (param)](#apidoc.element.blessed.Program.prototype.dynamicColors)
- description and source-code
```javascript
dynamicColors = function (param) {
  if (this.has('Cs')) {
    return this.put.Cs(param);
  }
  return this._twrite('\x1b]12;' + param + '\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ech"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ech (param)](#apidoc.element.blessed.Program.prototype.ech)
- description and source-code
```javascript
ech = function (param) {
  if (this.tput) return this.put.ech(param);
  return this._write('\x1b[' + (param || '') + 'X');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.echo"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>echo (text, attr)](#apidoc.element.blessed.Program.prototype.echo)
- description and source-code
```javascript
echo = function (text, attr) {
  return attr
    ? this._write(this.text(text, attr))
    : this._write(text);
}
```
- example usage
```shell
...
// Make the client look like a tty:
client.setRawMode = function(mode) {
  client.isRaw = mode;
  if (!client.writable) return;
  if (mode) {
    client.do.suppress_go_ahead();
    client.will.suppress_go_ahead();
    client.will.echo();
  } else {
    client.dont.suppress_go_ahead();
    client.wont.suppress_go_ahead();
    client.wont.echo();
  }
};
client.isTTY = true;
...
```

#### <a name="apidoc.element.blessed.Program.prototype.ed"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ed (param)](#apidoc.element.blessed.Program.prototype.ed)
- description and source-code
```javascript
ed = function (param) {
  if (this.tput) {
    switch (param) {
      case 'above':
        param = 1;
        break;
      case 'all':
        param = 2;
        break;
      case 'saved':
        param = 3;
        break;
      case 'below':
      default:
        param = 0;
        break;
    }
    // extended tput.E3 = ^[[3;J
    return this.put.ed(param);
  }
  switch (param) {
    case 'above':
      return this._write('\X1b[1J');
    case 'all':
      return this._write('\x1b[2J');
    case 'saved':
      return this._write('\x1b[3J');
    case 'below':
    default:
      return this._write('\x1b[J');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.el"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>el (param)](#apidoc.element.blessed.Program.prototype.el)
- description and source-code
```javascript
el = function (param) {
  if (this.tput) {
    //if (this.tput.back_color_erase) ...
    switch (param) {
      case 'left':
        param = 1;
        break;
      case 'all':
        param = 2;
        break;
      case 'right':
      default:
        param = 0;
        break;
    }
    return this.put.el(param);
  }
  switch (param) {
    case 'left':
      return this._write('\x1b[1K');
    case 'all':
      return this._write('\x1b[2K');
    case 'right':
    default:
      return this._write('\x1b[K');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.enableFilterRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableFilterRectangle ()](#apidoc.element.blessed.Program.prototype.enableFilterRectangle)
- description and source-code
```javascript
enableFilterRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'w');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.enableGpm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableGpm ()](#apidoc.element.blessed.Program.prototype.enableGpm)
- description and source-code
```javascript
enableGpm = function () {
  var self = this;
  var gpmclient = require('./gpmclient');

  if (this.gpm) return;

  this.gpm = gpmclient();

  this.gpm.on('btndown', function(btn, modifier, x, y) {
    x--, y--;

    var key = {
      name: 'mouse',
      type: 'GPM',
      action: 'mousedown',
      button: self.gpm.ButtonName(btn),
      raw: [btn, modifier, x, y],
      x: x,
      y: y,
      shift: self.gpm.hasShiftKey(modifier),
      meta: self.gpm.hasMetaKey(modifier),
      ctrl: self.gpm.hasCtrlKey(modifier)
    };

    self.emit('mouse', key);
  });

  this.gpm.on('btnup', function(btn, modifier, x, y) {
    x--, y--;

    var key = {
      name: 'mouse',
      type: 'GPM',
      action: 'mouseup',
      button: self.gpm.ButtonName(btn),
      raw: [btn, modifier, x, y],
      x: x,
      y: y,
      shift: self.gpm.hasShiftKey(modifier),
      meta: self.gpm.hasMetaKey(modifier),
      ctrl: self.gpm.hasCtrlKey(modifier)
    };

    self.emit('mouse', key);
  });

  this.gpm.on('move', function(btn, modifier, x, y) {
    x--, y--;

    var key = {
      name: 'mouse',
      type: 'GPM',
      action: 'mousemove',
      button: self.gpm.ButtonName(btn),
      raw: [btn, modifier, x, y],
      x: x,
      y: y,
      shift: self.gpm.hasShiftKey(modifier),
      meta: self.gpm.hasMetaKey(modifier),
      ctrl: self.gpm.hasCtrlKey(modifier)
    };

    self.emit('mouse', key);
  });

  this.gpm.on('drag', function(btn, modifier, x, y) {
    x--, y--;

    var key = {
      name: 'mouse',
      type: 'GPM',
      action: 'mousemove',
      button: self.gpm.ButtonName(btn),
      raw: [btn, modifier, x, y],
      x: x,
      y: y,
      shift: self.gpm.hasShiftKey(modifier),
      meta: self.gpm.hasMetaKey(modifier),
      ctrl: self.gpm.hasCtrlKey(modifier)
    };

    self.emit('mouse', key);
  });

  this.gpm.on('mousewheel', function(btn, modifier, x, y, dx, dy) {
    var key = {
      name: 'mouse',
      type: 'GPM',
      action: dy > 0 ? 'wheelup' : 'wheeldown',
      button: self.gpm.ButtonName(btn),
      raw: [btn, modifier, x, y, dx, dy],
      x: x,
      y: y,
      shift: self.gpm.hasShiftKey(modifier),
      meta: self.gpm.hasMetaKey(modifier),
      ctrl: self.gpm.hasCtrlKey(modifier)
    };

    self.emit('mouse', key);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.enableLocatorReporting"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableLocatorReporting ()](#apidoc.element.blessed.Program.prototype.enableLocatorReporting)
- description and source-code
```javascript
enableLocatorReporting = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.enableMouse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enableMouse ()](#apidoc.element.blessed.Program.prototype.enableMouse)
- description and source-code
```javascript
enableMouse = function () {
  if (process.env.BLESSED_FORCE_MODES) {
    var modes = process.env.BLESSED_FORCE_MODES.split(',');
    var options = {};
    for (var n = 0; n < modes.length; ++n) {
      var pair = modes[n].split('=');
      var v = pair[1] !== '0';
      switch (pair[0].toUpperCase()) {
        case 'SGRMOUSE':
          options.sgrMouse = v;
          break;
        case 'UTFMOUSE':
          options.utfMouse = v;
          break;
        case 'VT200MOUSE':
          options.vt200Mouse = v;
          break;
        case 'URXVTMOUSE':
          options.urxvtMouse = v;
          break;
        case 'X10MOUSE':
          options.x10Mouse = v;
          break;
        case 'DECMOUSE':
          options.decMouse = v;
          break;
        case 'PTERMMOUSE':
          options.ptermMouse = v;
          break;
        case 'JSBTERMMOUSE':
          options.jsbtermMouse = v;
          break;
        case 'VT200HILITE':
          options.vt200Hilite = v;
          break;
        case 'GPMMOUSE':
          options.gpmMouse = v;
          break;
        case 'CELLMOTION':
          options.cellMotion = v;
          break;
        case 'ALLMOTION':
          options.allMotion = v;
          break;
        case 'SENDFOCUS':
          options.sendFocus = v;
          break;
      }
    }
    return this.setMouse(options, true);
  }

  // NOTE:
  // Cell Motion isn't normally need for anything below here, but we'll
  // activate it for tmux (whether using it or not) in case our all-motion
  // passthrough does not work. It can't hurt.

  if (this.term('rxvt-unicode')) {
    return this.setMouse({
      urxvtMouse: true,
      cellMotion: true,
      allMotion: true
    }, true);
  }

  // rxvt does not support the X10 UTF extensions
  if (this.term('rxvt')) {
    return this.setMouse({
      vt200Mouse: true,
      x10Mouse: true,
      cellMotion: true,
      allMotion: true
    }, true);
  }

  // libvte is broken. Older versions do not support the
  // X10 UTF extension. However, later versions do support
  // SGR/URXVT.
  if (this.isVTE) {
    return this.setMouse({
      // NOTE: Could also use urxvtMouse here.
      sgrMouse: true,
      cellMotion: true,
      allMotion: true
    }, true);
  }

  if (this.term('linux')) {
    return this.setMouse({
      vt200Mouse: true,
      gpmMouse: true
    }, true);
  }

  if (this.term('xterm')
      || this.term('screen')
      || (this.tput && this.tput.strings.key_mouse)) {
    return this.setMouse({
      vt200Mouse: true,
      utfMouse: true,
      cellMotion: true,
      allMotion: true
    }, true);
  }
}
```
- example usage
```shell
...
- __resize__ - Received on screen resize.
- __mouse__ - Received on mouse events.
- __keypress__ - Received on key events.
- __element [name]__ - Global events received for all elements.
- __key [name]__ - Received on key event for [name].
- __focus, blur__ - Received when the terminal window focuses/blurs. Requires a
terminal supporting the focus protocol and focus needs to be passed to
program.enableMouse().
- __prerender__ - Received before render.
- __render__ - Received on render.
- __warning__ - Received when blessed notices something untoward (output is not
a tty, terminfo not found, etc).
- __destroy__ - Received when the screen is destroyed (only useful when using
multiple screens).
...
```

#### <a name="apidoc.element.blessed.Program.prototype.enter_alt_charset_mode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>enter_alt_charset_mode ()](#apidoc.element.blessed.Program.prototype.enter_alt_charset_mode)
- description and source-code
```javascript
enter_alt_charset_mode = function () {
  return this.charset('acs');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.eraseChars"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseChars (param)](#apidoc.element.blessed.Program.prototype.eraseChars)
- description and source-code
```javascript
eraseChars = function (param) {
  if (this.tput) return this.put.ech(param);
  return this._write('\x1b[' + (param || '') + 'X');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.eraseInDisplay"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseInDisplay (param)](#apidoc.element.blessed.Program.prototype.eraseInDisplay)
- description and source-code
```javascript
eraseInDisplay = function (param) {
  if (this.tput) {
    switch (param) {
      case 'above':
        param = 1;
        break;
      case 'all':
        param = 2;
        break;
      case 'saved':
        param = 3;
        break;
      case 'below':
      default:
        param = 0;
        break;
    }
    // extended tput.E3 = ^[[3;J
    return this.put.ed(param);
  }
  switch (param) {
    case 'above':
      return this._write('\X1b[1J');
    case 'all':
      return this._write('\x1b[2J');
    case 'saved':
      return this._write('\x1b[3J');
    case 'below':
    default:
      return this._write('\x1b[J');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.eraseInLine"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseInLine (param)](#apidoc.element.blessed.Program.prototype.eraseInLine)
- description and source-code
```javascript
eraseInLine = function (param) {
  if (this.tput) {
    //if (this.tput.back_color_erase) ...
    switch (param) {
      case 'left':
        param = 1;
        break;
      case 'all':
        param = 2;
        break;
      case 'right':
      default:
        param = 0;
        break;
    }
    return this.put.el(param);
  }
  switch (param) {
    case 'left':
      return this._write('\x1b[1K');
    case 'all':
      return this._write('\x1b[2K');
    case 'right':
    default:
      return this._write('\x1b[K');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.eraseRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>eraseRectangle ()](#apidoc.element.blessed.Program.prototype.eraseRectangle)
- description and source-code
```javascript
eraseRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$z');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.exit_alt_charset_mode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>exit_alt_charset_mode ()](#apidoc.element.blessed.Program.prototype.exit_alt_charset_mode)
- description and source-code
```javascript
exit_alt_charset_mode = function () {
  return this.charset('ascii');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.feed"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>feed ()](#apidoc.element.blessed.Program.prototype.feed)
- description and source-code
```javascript
feed = function () {
  if (this.tput && this.tput.bools.eat_newline_glitch && this.x >= this.cols) {
    return;
  }
  this.x = 0;
  this.y++;
  this._ncoords();
  if (this.has('nel')) return this.put.nel();
  return this._write('\n');
}
```
- example usage
```shell
...
program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
program.setx((program.cols / 2 | 0) - 4);
program.down(5);
program.write('Hi again!');
program.bg('!black');
program.feed();
'''


#### Testing

Most tests contained in the 'test/' directory are interactive. It's up to the
programmer to determine whether the test is properly displayed. In the future
...
```

#### <a name="apidoc.element.blessed.Program.prototype.ff"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ff ()](#apidoc.element.blessed.Program.prototype.ff)
- description and source-code
```javascript
ff = function () {
  if (this.has('ff')) return this.put.ff();
  return this._write('\x0c');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.fg"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>fg (color, val)](#apidoc.element.blessed.Program.prototype.fg)
- description and source-code
```javascript
fg = function (color, val) {
  color = color.split(/\s*[,;]\s*/).join(' fg, ') + ' fg';
  return this.attr(color, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.fillRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>fillRectangle ()](#apidoc.element.blessed.Program.prototype.fillRectangle)
- description and source-code
```javascript
fillRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.flush"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>flush ()](#apidoc.element.blessed.Program.prototype.flush)
- description and source-code
```javascript
flush = function () {
  if (!this._buf) return;
  this._owrite(this._buf);
  this._buf = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.form"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>form ()](#apidoc.element.blessed.Program.prototype.form)
- description and source-code
```javascript
form = function () {
  if (this.has('ff')) return this.put.ff();
  return this._write('\x0c');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.forward"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>forward (param)](#apidoc.element.blessed.Program.prototype.forward)
- description and source-code
```javascript
forward = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_right_cursor) {
      return this._write(this.repeat(this.tput.cuf1(), param));
    }
    return this.put.cuf(param);
  }
  return this._write('\x1b[' + (param || '') + 'C');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.getCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getCursor (callback)](#apidoc.element.blessed.Program.prototype.getCursor)
- description and source-code
```javascript
getCursor = function (callback) {
  return this.deviceStatus(6, callback, false, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.getCursorColor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getCursorColor (callback)](#apidoc.element.blessed.Program.prototype.getCursorColor)
- description and source-code
```javascript
getCursorColor = function (callback) {
  return this.getTextParams(12, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.getTextParams"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getTextParams (param, callback)](#apidoc.element.blessed.Program.prototype.getTextParams)
- description and source-code
```javascript
getTextParams = function (param, callback) {
  return this.response('text-params', '\x1b]' + param + ';?\x07', function(err, data) {
    if (err) return callback(err);
    return callback(null, data.pt);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.getWindowSize"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>getWindowSize (callback)](#apidoc.element.blessed.Program.prototype.getWindowSize)
- description and source-code
```javascript
getWindowSize = function (callback) {
  return this.manipulateWindow(18, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.has"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>has (name)](#apidoc.element.blessed.Program.prototype.has)
- description and source-code
```javascript
has = function (name) {
  return this.tput
    ? this.tput.has(name)
    : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.hideCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hideCursor ()](#apidoc.element.blessed.Program.prototype.hideCursor)
- description and source-code
```javascript
hideCursor = function () {
  this.cursorHidden = true;
  if (this.tput) return this.put.civis();
  return this.resetMode('?25');
}
```
- example usage
```shell
...
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
program.enableMouse();
program.hideCursor();
program.clear();

program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
program.setx((program.cols / 2 | 0) - 4);
program.down(5);
...
```

#### <a name="apidoc.element.blessed.Program.prototype.hpa"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hpa (param)](#apidoc.element.blessed.Program.prototype.hpa)
- description and source-code
```javascript
hpa = function (param) {
  this.x = param || 0;
  this._ncoords();
  if (this.tput) {
    return this.put.hpa.apply(this.put, arguments);
  }
  param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + ''');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.hpr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hpr (param)](#apidoc.element.blessed.Program.prototype.hpr)
- description and source-code
```javascript
hpr = function (param) {
  if (this.tput) return this.cuf(param);
  this.x += param || 1;
  this._ncoords();
  // Does not exist:
  // if (this.tput) return this.put.hpr(param);
  return this._write('\x1b[' + (param || '') + 'a');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ht"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ht ()](#apidoc.element.blessed.Program.prototype.ht)
- description and source-code
```javascript
ht = function () {
  this.x += 8;
  this._ncoords();
  if (this.has('ht')) return this.put.ht();
  return this._write('\t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.hvp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>hvp (row, col)](#apidoc.element.blessed.Program.prototype.hvp)
- description and source-code
```javascript
hvp = function (row, col) {
  if (!this.zero) {
    row = (row || 1) - 1;
    col = (col || 1) - 1;
  } else {
    row = row || 0;
    col = col || 0;
  }
  this.y = row;
  this.x = col;
  this._ncoords();
  // Does not exist (?):
  // if (this.tput) return this.put.hvp(row, col);
  if (this.tput) return this.put.cup(row, col);
  return this._write('\x1b[' + (row + 1) + ';' + (col + 1) + 'f');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ich"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ich (param)](#apidoc.element.blessed.Program.prototype.ich)
- description and source-code
```javascript
ich = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) return this.put.ich(param);
  return this._write('\x1b[' + (param || 1) + '@');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.il"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>il (param)](#apidoc.element.blessed.Program.prototype.il)
- description and source-code
```javascript
il = function (param) {
  if (this.tput) return this.put.il(param);
  return this._write('\x1b[' + (param || '') + 'L');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ind"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ind ()](#apidoc.element.blessed.Program.prototype.ind)
- description and source-code
```javascript
ind = function () {
  this.y++;
  this._ncoords();
  if (this.tput) return this.put.ind();
  return this._write('\x1bD');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.index"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>index ()](#apidoc.element.blessed.Program.prototype.index)
- description and source-code
```javascript
index = function () {
  this.y++;
  this._ncoords();
  if (this.tput) return this.put.ind();
  return this._write('\x1bD');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.initMouseTracking"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>initMouseTracking ()](#apidoc.element.blessed.Program.prototype.initMouseTracking)
- description and source-code
```javascript
initMouseTracking = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + 'T');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.insertChars"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertChars (param)](#apidoc.element.blessed.Program.prototype.insertChars)
- description and source-code
```javascript
insertChars = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) return this.put.ich(param);
  return this._write('\x1b[' + (param || 1) + '@');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.insertColumns"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertColumns ()](#apidoc.element.blessed.Program.prototype.insertColumns)
- description and source-code
```javascript
insertColumns = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + ' }');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.insertLines"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>insertLines (param)](#apidoc.element.blessed.Program.prototype.insertLines)
- description and source-code
```javascript
insertLines = function (param) {
  if (this.tput) return this.put.il(param);
  return this._write('\x1b[' + (param || '') + 'L');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.kbs"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>kbs ()](#apidoc.element.blessed.Program.prototype.kbs)
- description and source-code
```javascript
kbs = function () {
  this.x--;
  this._ncoords();
  if (this.has('kbs')) return this.put.kbs();
  return this._write('\x08');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.key"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>key (key, listener)](#apidoc.element.blessed.Program.prototype.key)
- description and source-code
```javascript
key = function (key, listener) {
  if (typeof key === 'string') key = key.split(/\s*,\s*/);
  key.forEach(function(key) {
    return this.on('key ' + key, listener);
  }, this);
}
```
- example usage
```shell
...
// If our box is clicked, change the content.
box.on('click', function(data) {
  box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
  screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
  box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
  box.setLine(1, 'bar');
  box.insertLine(1, 'foo');
  screen.render();
});

// Quit on Escape, q, or Control-C.
...
```

#### <a name="apidoc.element.blessed.Program.prototype.left"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>left (param)](#apidoc.element.blessed.Program.prototype.left)
- description and source-code
```javascript
left = function (param) {
  this.x -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_left_cursor) {
      return this._write(this.repeat(this.tput.cub1(), param));
    }
    return this.put.cub(param);
  }
  return this._write('\x1b[' + (param || '') + 'D');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.lineHeight"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lineHeight ()](#apidoc.element.blessed.Program.prototype.lineHeight)
- description and source-code
```javascript
lineHeight = function () {
  return this._write('\x1b#');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.linePosAbsolute"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>linePosAbsolute (param)](#apidoc.element.blessed.Program.prototype.linePosAbsolute)
- description and source-code
```javascript
linePosAbsolute = function (param) {
  this.y = param || 1;
  this._ncoords();
  if (this.tput) {
    return this.put.vpa.apply(this.put, arguments);
  }
  param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.listen"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>listen ()](#apidoc.element.blessed.Program.prototype.listen)
- description and source-code
```javascript
listen = function () {
  var self = this;

  // Potentially reset window title on exit:
  // if (!this.isRxvt) {
  //   if (!this.isVTE) this.setTitleModeFeature(3);
  //   this.manipulateWindow(21, function(err, data) {
  //     if (err) return;
  //     self._originalTitle = data.text;
  //   });
  // }

  // Listen for keys/mouse on input
  if (!this.input._blessedInput) {
    this.input._blessedInput = 1;
    this._listenInput();
  } else {
    this.input._blessedInput++;
  }

  this.on('newListener', this._newHandler = function fn(type) {
    if (type === 'keypress' || type === 'mouse') {
      self.removeListener('newListener', fn);
      if (self.input.setRawMode && !self.input.isRaw) {
        self.input.setRawMode(true);
        self.input.resume();
      }
    }
  });

  this.on('newListener', function fn(type) {
    if (type === 'mouse') {
      self.removeListener('newListener', fn);
      self.bindMouse();
    }
  });

  // Listen for resize on output
  if (!this.output._blessedOutput) {
    this.output._blessedOutput = 1;
    this._listenOutput();
  } else {
    this.output._blessedOutput++;
  }
}
```
- example usage
```shell
...
    width: '80%',
    height: '90%',
    border: 'line',
    content: 'Welcome to my server. Here is your own private session.'
  });

  screen.render();
}).listen(2300);
'''

Once you've written something similar and started it, you can simply telnet
into your blessed app:

''' bash
$ telnet localhost 2300
...
```

#### <a name="apidoc.element.blessed.Program.prototype.loadLEDs"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>loadLEDs (param)](#apidoc.element.blessed.Program.prototype.loadLEDs)
- description and source-code
```javascript
loadLEDs = function (param) {
  return this._write('\x1b[' + (param || '') + 'q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.log"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>log ()](#apidoc.element.blessed.Program.prototype.log)
- description and source-code
```javascript
log = function () {
  return this._log('LOG',  util.format.apply(util, arguments));
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```

#### <a name="apidoc.element.blessed.Program.prototype.lrestoreCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lrestoreCursor (key, hide)](#apidoc.element.blessed.Program.prototype.lrestoreCursor)
- description and source-code
```javascript
lrestoreCursor = function (key, hide) {
  var pos;
  key = key || 'local';
  if (!this._saved || !this._saved[key]) return;
  pos = this._saved[key];
  //delete this._saved[key];
  this.cup(pos.y, pos.x);
  if (hide && pos.hidden !== this.cursorHidden) {
    if (pos.hidden) {
      this.hideCursor();
    } else {
      this.showCursor();
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.lsaveCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>lsaveCursor (key)](#apidoc.element.blessed.Program.prototype.lsaveCursor)
- description and source-code
```javascript
lsaveCursor = function (key) {
  key = key || 'local';
  this._saved = this._saved || {};
  this._saved[key] = this._saved[key] || {};
  this._saved[key].x = this.x;
  this._saved[key].y = this.y;
  this._saved[key].hidden = this.cursorHidden;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.manipulateWindow"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>manipulateWindow ()](#apidoc.element.blessed.Program.prototype.manipulateWindow)
- description and source-code
```javascript
manipulateWindow = function () {
  var args = slice.call(arguments);

  var callback = typeof args[args.length - 1] === 'function'
    ? args.pop()
    : function() {};

  return this.response('window-manipulation',
    '\x1b[' + args.join(';') + 't', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mc"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc ()](#apidoc.element.blessed.Program.prototype.mc)
- description and source-code
```javascript
mc = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + 'i');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mc0"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc0 ()](#apidoc.element.blessed.Program.prototype.mc0)
- description and source-code
```javascript
mc0 = function () {
  if (this.tput) return this.put.mc0();
  return this.mc('0');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mc4"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc4 ()](#apidoc.element.blessed.Program.prototype.mc4)
- description and source-code
```javascript
mc4 = function () {
  if (this.tput) return this.put.mc4();
  return this.mc('4');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mc5"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc5 ()](#apidoc.element.blessed.Program.prototype.mc5)
- description and source-code
```javascript
mc5 = function () {
  if (this.tput) return this.put.mc5();
  return this.mc('5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mc5p"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mc5p ()](#apidoc.element.blessed.Program.prototype.mc5p)
- description and source-code
```javascript
mc5p = function () {
  if (this.tput) return this.put.mc5p();
  return this.mc('?5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.mediaCopy"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>mediaCopy ()](#apidoc.element.blessed.Program.prototype.mediaCopy)
- description and source-code
```javascript
mediaCopy = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + 'i');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.move"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>move (x, y)](#apidoc.element.blessed.Program.prototype.move)
- description and source-code
```javascript
move = function (x, y) {
  return this.cursorPos(y, x);
}
```
- example usage
```shell
...
  program.showCursor();
  program.normalBuffer();
  process.exit(0);
});

program.on('mouse', function(data) {
  if (data.action === 'mousemove') {
    program.move(data.x, data.y);
    program.bg('red');
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
...
```

#### <a name="apidoc.element.blessed.Program.prototype.nel"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nel ()](#apidoc.element.blessed.Program.prototype.nel)
- description and source-code
```javascript
nel = function () {
  if (this.tput && this.tput.bools.eat_newline_glitch && this.x >= this.cols) {
    return;
  }
  this.x = 0;
  this.y++;
  this._ncoords();
  if (this.has('nel')) return this.put.nel();
  return this._write('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.newline"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>newline ()](#apidoc.element.blessed.Program.prototype.newline)
- description and source-code
```javascript
newline = function () {
  if (this.tput && this.tput.bools.eat_newline_glitch && this.x >= this.cols) {
    return;
  }
  this.x = 0;
  this.y++;
  this._ncoords();
  if (this.has('nel')) return this.put.nel();
  return this._write('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.nextLine"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nextLine ()](#apidoc.element.blessed.Program.prototype.nextLine)
- description and source-code
```javascript
nextLine = function () {
  this.y++;
  this.x = 0;
  this._ncoords();
  if (this.has('nel')) return this.put.nel();
  return this._write('\x1bE');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.normalBuffer"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>normalBuffer ()](#apidoc.element.blessed.Program.prototype.normalBuffer)
- description and source-code
```javascript
normalBuffer = function () {
  this.isAlt = false;
  if (this.tput) return this.put.rmcup();
  this.resetMode('?47');
  return this.resetMode('?1049');
}
```
- example usage
```shell
...
var blessed = require('blessed')
, program = blessed.program();

program.key('q', function(ch, key) {
program.clear();
program.disableMouse();
program.showCursor();
program.normalBuffer();
process.exit(0);
});

program.on('mouse', function(data) {
if (data.action === 'mousemove') {
  program.move(data.x, data.y);
  program.bg('red');
...
```

#### <a name="apidoc.element.blessed.Program.prototype.nul"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>nul ()](#apidoc.element.blessed.Program.prototype.nul)
- description and source-code
```javascript
nul = function () {
  //if (this.has('pad')) return this.put.pad();
  return this._write('\200');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.omove"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>omove (x, y)](#apidoc.element.blessed.Program.prototype.omove)
- description and source-code
```javascript
omove = function (x, y) {
  if (!this.zero) {
    x = (x || 1) - 1;
    y = (y || 1) - 1;
  } else {
    x = x || 0;
    y = y || 0;
  }
  if (y === this.y && x === this.x) {
    return;
  }
  if (y === this.y) {
    if (x > this.x) {
      this.cuf(x - this.x);
    } else if (x < this.x) {
      this.cub(this.x - x);
    }
  } else if (x === this.x) {
    if (y > this.y) {
      this.cud(y - this.y);
    } else if (y < this.y) {
      this.cuu(this.y - y);
    }
  } else {
    if (!this.zero) x++, y++;
    this.cup(y, x);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.onceKey"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>onceKey (key, listener)](#apidoc.element.blessed.Program.prototype.onceKey)
- description and source-code
```javascript
onceKey = function (key, listener) {
  if (typeof key === 'string') key = key.split(/\s*,\s*/);
  key.forEach(function(key) {
    return this.once('key ' + key, listener);
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.out"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>out (name)](#apidoc.element.blessed.Program.prototype.out)
- description and source-code
```javascript
out = function (name) {
  var args = Array.prototype.slice.call(arguments, 1);
  this.ret = true;
  var out = this[name].apply(this, args);
  this.ret = false;
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.pO"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pO ()](#apidoc.element.blessed.Program.prototype.pO)
- description and source-code
```javascript
pO = function () {
  if (this.tput) return this.put.mc5p();
  return this.mc('?5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.pause"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pause (callback)](#apidoc.element.blessed.Program.prototype.pause)
- description and source-code
```javascript
pause = function (callback) {
  var self = this
    , isAlt = this.isAlt
    , mouseEnabled = this.mouseEnabled;

  this.lsaveCursor('pause');
  //this.csr(0, screen.height - 1);
  if (isAlt) this.normalBuffer();
  this.showCursor();
  if (mouseEnabled) this.disableMouse();

  var write = this.output.write;
  this.output.write = function() {};
  if (this.input.setRawMode) {
    this.input.setRawMode(false);
  }
  this.input.pause();

  return this._resume = function() {
    delete self._resume;

    if (self.input.setRawMode) {
      self.input.setRawMode(true);
    }
    self.input.resume();
    self.output.write = write;

    if (isAlt) self.alternateBuffer();
    //self.csr(0, screen.height - 1);
    if (mouseEnabled) self.enableMouse();
    self.lrestoreCursor('pause', true);

    if (callback) callback();
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.pf"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pf ()](#apidoc.element.blessed.Program.prototype.pf)
- description and source-code
```javascript
pf = function () {
  if (this.tput) return this.put.mc4();
  return this.mc('4');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.po"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>po ()](#apidoc.element.blessed.Program.prototype.po)
- description and source-code
```javascript
po = function () {
  if (this.tput) return this.put.mc5();
  return this.mc('5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.pos"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>pos (row, col)](#apidoc.element.blessed.Program.prototype.pos)
- description and source-code
```javascript
pos = function (row, col) {
  if (!this.zero) {
    row = (row || 1) - 1;
    col = (col || 1) - 1;
  } else {
    row = row || 0;
    col = col || 0;
  }
  this.x = col;
  this.y = row;
  this._ncoords();
  if (this.tput) return this.put.cup(row, col);
  return this._write('\x1b[' + (row + 1) + ';' + (col + 1) + 'H');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.print"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>print (text, attr)](#apidoc.element.blessed.Program.prototype.print)
- description and source-code
```javascript
print = function (text, attr) {
  return attr
    ? this._write(this.text(text, attr))
    : this._write(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.print_screen"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>print_screen ()](#apidoc.element.blessed.Program.prototype.print_screen)
- description and source-code
```javascript
print_screen = function () {
  if (this.tput) return this.put.mc0();
  return this.mc('0');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.prtr_non"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_non ()](#apidoc.element.blessed.Program.prototype.prtr_non)
- description and source-code
```javascript
prtr_non = function () {
  if (this.tput) return this.put.mc5p();
  return this.mc('?5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.prtr_off"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_off ()](#apidoc.element.blessed.Program.prototype.prtr_off)
- description and source-code
```javascript
prtr_off = function () {
  if (this.tput) return this.put.mc4();
  return this.mc('4');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.prtr_on"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>prtr_on ()](#apidoc.element.blessed.Program.prototype.prtr_on)
- description and source-code
```javascript
prtr_on = function () {
  if (this.tput) return this.put.mc5();
  return this.mc('5');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ps"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ps ()](#apidoc.element.blessed.Program.prototype.ps)
- description and source-code
```javascript
ps = function () {
  if (this.tput) return this.put.mc0();
  return this.mc('0');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rc"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rc (key, hide)](#apidoc.element.blessed.Program.prototype.rc)
- description and source-code
```javascript
rc = function (key, hide) {
  if (key) return this.lrestoreCursor(key, hide);
  this.x = this.savedX || 0;
  this.y = this.savedY || 0;
  if (this.tput) return this.put.rc();
  return this._write('\x1b8');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rcA"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rcA ()](#apidoc.element.blessed.Program.prototype.rcA)
- description and source-code
```javascript
rcA = function () {
  this.x = this.savedX || 0;
  this.y = this.savedY || 0;
  if (this.tput) return this.put.rc();
  return this._write('\x1b[u');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.removeKey"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>removeKey (key, listener)](#apidoc.element.blessed.Program.prototype.removeKey)
- description and source-code
```javascript
removeKey = function (key, listener) {
  if (typeof key === 'string') key = key.split(/\s*,\s*/);
  key.forEach(function(key) {
    return this.removeListener('key ' + key, listener);
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rep"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rep (param)](#apidoc.element.blessed.Program.prototype.rep)
- description and source-code
```javascript
rep = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) return this.put.rep(param);
  return this._write('\x1b[' + (param || 1) + 'b');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.repeat"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>repeat (ch, i)](#apidoc.element.blessed.Program.prototype.repeat)
- description and source-code
```javascript
repeat = function (ch, i) {
  if (!i || i < 0) i = 0;
  return Array(i + 1).join(ch);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.repeatPrecedingCharacter"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>repeatPrecedingCharacter (param)](#apidoc.element.blessed.Program.prototype.repeatPrecedingCharacter)
- description and source-code
```javascript
repeatPrecedingCharacter = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) return this.put.rep(param);
  return this._write('\x1b[' + (param || 1) + 'b');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.req_mouse_pos"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>req_mouse_pos (param, callback)](#apidoc.element.blessed.Program.prototype.req_mouse_pos)
- description and source-code
```javascript
req_mouse_pos = function (param, callback) {
  // See also:
  // get_mouse / getm / Gm
  // mouse_info / minfo / Mi
  // Correct for tput?
  if (this.has('req_mouse_pos')) {
    var code = this.tput.req_mouse_pos(param);
    return this.response('locator-position', code, callback);
  }
  return this.response('locator-position',
    '\x1b[' + (param || '') + '\'|', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.reqmp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reqmp (param, callback)](#apidoc.element.blessed.Program.prototype.reqmp)
- description and source-code
```javascript
reqmp = function (param, callback) {
  // See also:
  // get_mouse / getm / Gm
  // mouse_info / minfo / Mi
  // Correct for tput?
  if (this.has('req_mouse_pos')) {
    var code = this.tput.req_mouse_pos(param);
    return this.response('locator-position', code, callback);
  }
  return this.response('locator-position',
    '\x1b[' + (param || '') + '\'|', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.requestAnsiMode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestAnsiMode (param)](#apidoc.element.blessed.Program.prototype.requestAnsiMode)
- description and source-code
```javascript
requestAnsiMode = function (param) {
  return this._write('\x1b[' + (param || '') + '$p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.requestLocatorPosition"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestLocatorPosition (param, callback)](#apidoc.element.blessed.Program.prototype.requestLocatorPosition)
- description and source-code
```javascript
requestLocatorPosition = function (param, callback) {
  // See also:
  // get_mouse / getm / Gm
  // mouse_info / minfo / Mi
  // Correct for tput?
  if (this.has('req_mouse_pos')) {
    var code = this.tput.req_mouse_pos(param);
    return this.response('locator-position', code, callback);
  }
  return this.response('locator-position',
    '\x1b[' + (param || '') + '\'|', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.requestParameters"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestParameters (param)](#apidoc.element.blessed.Program.prototype.requestParameters)
- description and source-code
```javascript
requestParameters = function (param) {
  return this._write('\x1b[' + (param || 0) + 'x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.requestPrivateMode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>requestPrivateMode (param)](#apidoc.element.blessed.Program.prototype.requestPrivateMode)
- description and source-code
```javascript
requestPrivateMode = function (param) {
  return this._write('\x1b[?' + (param || '') + '$p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.reset"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reset ()](#apidoc.element.blessed.Program.prototype.reset)
- description and source-code
```javascript
reset = function () {
  this.x = this.y = 0;
  if (this.has('rs1') || this.has('ris')) {
    return this.has('rs1')
      ? this.put.rs1()
      : this.put.ris();
  }
  return this._write('\x1bc');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.resetColors"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetColors (param)](#apidoc.element.blessed.Program.prototype.resetColors)
- description and source-code
```javascript
resetColors = function (param) {
  if (this.has('Cr')) {
    return this.put.Cr(param);
  }
  return this._twrite('\x1b]112\x07');
  //return this._twrite('\x1b]112;' + param + '\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.resetCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetCursor ()](#apidoc.element.blessed.Program.prototype.resetCursor)
- description and source-code
```javascript
resetCursor = function () {
  if (this.term('xterm') || this.term('rxvt') || this.term('screen')) {
    // XXX
    // return this.resetColors();
    this._twrite('\x1b[0 q');
    this._twrite('\x1b]112\x07');
    // urxvt doesnt support OSC 112
    this._twrite('\x1b]12;white\x07');
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.resetMode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetMode ()](#apidoc.element.blessed.Program.prototype.resetMode)
- description and source-code
```javascript
resetMode = function () {
  var param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'l');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.resetTitleModes"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resetTitleModes ()](#apidoc.element.blessed.Program.prototype.resetTitleModes)
- description and source-code
```javascript
resetTitleModes = function () {
  return this._write('\x1b[>' + slice.call(arguments).join(';') + 'T');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.response"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>response (name, text, callback, noBypass)](#apidoc.element.blessed.Program.prototype.response)
- description and source-code
```javascript
response = function (name, text, callback, noBypass) {
  var self = this;

  if (arguments.length === 2) {
    callback = text;
    text = name;
    name = null;
  }

  if (!callback) {
    callback = function() {};
  }

  this.bindResponse();

  name = name
    ? 'response ' + name
    : 'response';

  var onresponse;

  this.once(name, onresponse = function(event) {
    if (timeout) clearTimeout(timeout);
    if (event.type === 'error') {
      return callback(new Error(event.event + ': ' + event.text));
    }
    return callback(null, event);
  });

  var timeout = setTimeout(function() {
    self.removeListener(name, onresponse);
    return callback(new Error('Timeout.'));
  }, 2000);

  return noBypass
    ? this._write(text)
    : this._twrite(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.restoreCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreCursor (key, hide)](#apidoc.element.blessed.Program.prototype.restoreCursor)
- description and source-code
```javascript
restoreCursor = function (key, hide) {
  if (key) return this.lrestoreCursor(key, hide);
  this.x = this.savedX || 0;
  this.y = this.savedY || 0;
  if (this.tput) return this.put.rc();
  return this._write('\x1b8');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.restoreCursorA"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreCursorA ()](#apidoc.element.blessed.Program.prototype.restoreCursorA)
- description and source-code
```javascript
restoreCursorA = function () {
  this.x = this.savedX || 0;
  this.y = this.savedY || 0;
  if (this.tput) return this.put.rc();
  return this._write('\x1b[u');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.restorePrivateValues"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restorePrivateValues ()](#apidoc.element.blessed.Program.prototype.restorePrivateValues)
- description and source-code
```javascript
restorePrivateValues = function () {
  return this._write('\x1b[?' + slice.call(arguments).join(';') + 'r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.restoreReportedCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>restoreReportedCursor ()](#apidoc.element.blessed.Program.prototype.restoreReportedCursor)
- description and source-code
```javascript
restoreReportedCursor = function () {
  if (this._rx == null) return;
  return this.cup(this._ry, this._rx);
  // return this.nel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.resume"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>resume ()](#apidoc.element.blessed.Program.prototype.resume)
- description and source-code
```javascript
resume = function () {
  if (this._resume) return this._resume();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.return"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>return ()](#apidoc.element.blessed.Program.prototype.return)
- description and source-code
```javascript
return = function () {
  this.x = 0;
  if (this.has('cr')) return this.put.cr();
  return this._write('\r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.reverse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverse ()](#apidoc.element.blessed.Program.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  this.y--;
  this._ncoords();
  if (this.tput) return this.put.ri();
  return this._write('\x1bM');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.reverseAttrInRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverseAttrInRectangle ()](#apidoc.element.blessed.Program.prototype.reverseAttrInRectangle)
- description and source-code
```javascript
reverseAttrInRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.reverseIndex"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>reverseIndex ()](#apidoc.element.blessed.Program.prototype.reverseIndex)
- description and source-code
```javascript
reverseIndex = function () {
  this.y--;
  this._ncoords();
  if (this.tput) return this.put.ri();
  return this._write('\x1bM');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.ri"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>ri ()](#apidoc.element.blessed.Program.prototype.ri)
- description and source-code
```javascript
ri = function () {
  this.y--;
  this._ncoords();
  if (this.tput) return this.put.ri();
  return this._write('\x1bM');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.right"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>right (param)](#apidoc.element.blessed.Program.prototype.right)
- description and source-code
```javascript
right = function (param) {
  this.x += param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_right_cursor) {
      return this._write(this.repeat(this.tput.cuf1(), param));
    }
    return this.put.cuf(param);
  }
  return this._write('\x1b[' + (param || '') + 'C');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rm ()](#apidoc.element.blessed.Program.prototype.rm)
- description and source-code
```javascript
rm = function () {
  var param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'l');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rmacs"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmacs ()](#apidoc.element.blessed.Program.prototype.rmacs)
- description and source-code
```javascript
rmacs = function () {
  return this.charset('ascii');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rmcup"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmcup ()](#apidoc.element.blessed.Program.prototype.rmcup)
- description and source-code
```javascript
rmcup = function () {
  this.isAlt = false;
  if (this.tput) return this.put.rmcup();
  this.resetMode('?47');
  return this.resetMode('?1049');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rmove"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rmove (x, y)](#apidoc.element.blessed.Program.prototype.rmove)
- description and source-code
```javascript
rmove = function (x, y) {
  this.rsetx(x);
  this.rsety(y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rs2"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rs2 ()](#apidoc.element.blessed.Program.prototype.rs2)
- description and source-code
```javascript
rs2 = function () {
  //if (this.tput) return this.put.init_2string();
  //if (this.tput) return this.put.reset_2string();
  if (this.tput) return this.put.rs2();
  //return this._write('\x1b[!p');
  //return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // init
  return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // reset
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rsetx"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rsetx (x)](#apidoc.element.blessed.Program.prototype.rsetx)
- description and source-code
```javascript
rsetx = function (x) {
  // return this.HPositionRelative(x);
  if (!x) return;
  return x > 0
    ? this.forward(x)
    : this.back(-x);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.rsety"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>rsety (y)](#apidoc.element.blessed.Program.prototype.rsety)
- description and source-code
```javascript
rsety = function (y) {
  // return this.VPositionRelative(y);
  if (!y) return;
  return y > 0
    ? this.up(y)
    : this.down(-y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.saveCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveCursor (key)](#apidoc.element.blessed.Program.prototype.saveCursor)
- description and source-code
```javascript
saveCursor = function (key) {
  if (key) return this.lsaveCursor(key);
  this.savedX = this.x || 0;
  this.savedY = this.y || 0;
  if (this.tput) return this.put.sc();
  return this._write('\x1b7');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.saveCursorA"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveCursorA ()](#apidoc.element.blessed.Program.prototype.saveCursorA)
- description and source-code
```javascript
saveCursorA = function () {
  this.savedX = this.x;
  this.savedY = this.y;
  if (this.tput) return this.put.sc();
  return this._write('\x1b[s');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.savePrivateValues"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>savePrivateValues ()](#apidoc.element.blessed.Program.prototype.savePrivateValues)
- description and source-code
```javascript
savePrivateValues = function () {
  return this._write('\x1b[?' + slice.call(arguments).join(';') + 's');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.saveReportedCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>saveReportedCursor (callback)](#apidoc.element.blessed.Program.prototype.saveReportedCursor)
- description and source-code
```javascript
saveReportedCursor = function (callback) {
  var self = this;
  if (this.tput.strings.user7 === '\x1b[6n' || this.term('screen')) {
    return this.getCursor(function(err, data) {
      if (data) {
        self._rx = data.status.x;
        self._ry = data.status.y;
      }
      if (!callback) return;
      return callback(err);
    });
  }
  if (!callback) return;
  return callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.sc"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sc (key)](#apidoc.element.blessed.Program.prototype.sc)
- description and source-code
```javascript
sc = function (key) {
  if (key) return this.lsaveCursor(key);
  this.savedX = this.x || 0;
  this.savedY = this.y || 0;
  if (this.tput) return this.put.sc();
  return this._write('\x1b7');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.scA"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scA ()](#apidoc.element.blessed.Program.prototype.scA)
- description and source-code
```javascript
scA = function () {
  this.savedX = this.x;
  this.savedY = this.y;
  if (this.tput) return this.put.sc();
  return this._write('\x1b[s');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.scrollDown"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scrollDown (param)](#apidoc.element.blessed.Program.prototype.scrollDown)
- description and source-code
```javascript
scrollDown = function (param) {
  this.y += param || 1;
  this._ncoords();
  if (this.tput) return this.put.parm_rindex(param);
  return this._write('\x1b[' + (param || 1) + 'T');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.scrollUp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>scrollUp (param)](#apidoc.element.blessed.Program.prototype.scrollUp)
- description and source-code
```javascript
scrollUp = function (param) {
  this.y -= param || 1;
  this._ncoords();
  if (this.tput) return this.put.parm_index(param);
  return this._write('\x1b[' + (param || 1) + 'S');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.sd"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sd (param)](#apidoc.element.blessed.Program.prototype.sd)
- description and source-code
```javascript
sd = function (param) {
  this.y += param || 1;
  this._ncoords();
  if (this.tput) return this.put.parm_rindex(param);
  return this._write('\x1b[' + (param || 1) + 'T');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.selData"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selData (a, b)](#apidoc.element.blessed.Program.prototype.selData)
- description and source-code
```javascript
selData = function (a, b) {
  if (this.has('Ms')) {
    return this.put.Ms(a, b);
  }
  return this._twrite('\x1b]52;' + a + ';' + b + '\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.selectChangeExtent"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selectChangeExtent (param)](#apidoc.element.blessed.Program.prototype.selectChangeExtent)
- description and source-code
```javascript
selectChangeExtent = function (param) {
  return this._write('\x1b[' + (param || 0) + 'x');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.selectiveEraseRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>selectiveEraseRectangle ()](#apidoc.element.blessed.Program.prototype.selectiveEraseRectangle)
- description and source-code
```javascript
selectiveEraseRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '${');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.sendDeviceAttributes"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sendDeviceAttributes (param, callback)](#apidoc.element.blessed.Program.prototype.sendDeviceAttributes)
- description and source-code
```javascript
sendDeviceAttributes = function (param, callback) {
  return this.response('device-attributes',
    '\x1b[' + (param || '') + 'c', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setAttrInRectangle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setAttrInRectangle ()](#apidoc.element.blessed.Program.prototype.setAttrInRectangle)
- description and source-code
```javascript
setAttrInRectangle = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '$r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setBackground"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setBackground (color, val)](#apidoc.element.blessed.Program.prototype.setBackground)
- description and source-code
```javascript
setBackground = function (color, val) {
  color = color.split(/\s*[,;]\s*/).join(' bg, ') + ' bg';
  return this.attr(color, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setCharProtectionAttr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setCharProtectionAttr (param)](#apidoc.element.blessed.Program.prototype.setCharProtectionAttr)
- description and source-code
```javascript
setCharProtectionAttr = function (param) {
  return this._write('\x1b[' + (param || 0) + '"q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setConformanceLevel"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setConformanceLevel ()](#apidoc.element.blessed.Program.prototype.setConformanceLevel)
- description and source-code
```javascript
setConformanceLevel = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '"p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setCursorStyle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setCursorStyle (param)](#apidoc.element.blessed.Program.prototype.setCursorStyle)
- description and source-code
```javascript
setCursorStyle = function (param) {
  switch (param) {
    case 'blinking block':
      param = 1;
      break;
    case 'block':
    case 'steady block':
      param = 2;
      break;
    case 'blinking underline':
      param = 3;
      break;
    case 'underline':
    case 'steady underline':
      param = 4;
      break;
    case 'blinking bar':
      param = 5;
      break;
    case 'bar':
    case 'steady bar':
      param = 6;
      break;
  }
  if (param === 2 && this.has('Se')) {
    return this.put.Se();
  }
  if (this.has('Ss')) {
    return this.put.Ss(param);
  }
  return this._write('\x1b[' + (param || 1) + ' q');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setForeground"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setForeground (color, val)](#apidoc.element.blessed.Program.prototype.setForeground)
- description and source-code
```javascript
setForeground = function (color, val) {
  color = color.split(/\s*[,;]\s*/).join(' fg, ') + ' fg';
  return this.attr(color, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setG"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setG (val)](#apidoc.element.blessed.Program.prototype.setG)
- description and source-code
```javascript
setG = function (val) {
  // if (this.tput) return this.put.S2();
  // if (this.tput) return this.put.S3();
  switch (val) {
    case 1:
      val = '~'; // GR
      break;
    case 2:
      val = 'n'; // GL
      val = '}'; // GR
      val = 'N'; // Next Char Only
      break;
    case 3:
      val = 'o'; // GL
      val = '|'; // GR
      val = 'O'; // Next Char Only
      break;
  }
  return this._write('\x1b' + val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setLocatorEvents"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setLocatorEvents ()](#apidoc.element.blessed.Program.prototype.setLocatorEvents)
- description and source-code
```javascript
setLocatorEvents = function () {
  return this._write('\x1b[' + slice.call(arguments).join(';') + '\'{');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setMarginBellVolume"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMarginBellVolume (param)](#apidoc.element.blessed.Program.prototype.setMarginBellVolume)
- description and source-code
```javascript
setMarginBellVolume = function (param) {
  return this._write('\x1b[' + (param || '') + ' u');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setMode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMode ()](#apidoc.element.blessed.Program.prototype.setMode)
- description and source-code
```javascript
setMode = function () {
  var param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'h');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setMouse"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setMouse (opt, enable)](#apidoc.element.blessed.Program.prototype.setMouse)
- description and source-code
```javascript
setMouse = function (opt, enable) {
  if (opt.normalMouse != null) {
    opt.vt200Mouse = opt.normalMouse;
    opt.allMotion = opt.normalMouse;
  }

  if (opt.hiliteTracking != null) {
    opt.vt200Hilite = opt.hiliteTracking;
  }

  if (enable === true) {
    if (this._currentMouse) {
      this.setMouse(opt);
      Object.keys(opt).forEach(function(key) {
        this._currentMouse[key] = opt[key];
      }, this);
      return;
    }
    this._currentMouse = opt;
    this.mouseEnabled = true;
  } else if (enable === false) {
    delete this._currentMouse;
    this.mouseEnabled = false;
  }

  //     Ps = 9  -> Send Mouse X & Y on button press.  See the sec-
  //     tion Mouse Tracking.
  //     Ps = 9  -> Don't send Mouse X & Y on button press.
  // x10 mouse
  if (opt.x10Mouse != null) {
    if (opt.x10Mouse) this.setMode('?9');
    else this.resetMode('?9');
  }

  //     Ps = 1 0 0 0  -> Send Mouse X & Y on button press and
  //     release.  See the section Mouse Tracking.
  //     Ps = 1 0 0 0  -> Don't send Mouse X & Y on button press and
  //     release.  See the section Mouse Tracking.
  // vt200 mouse
  if (opt.vt200Mouse != null) {
    if (opt.vt200Mouse) this.setMode('?1000');
    else this.resetMode('?1000');
  }

  //     Ps = 1 0 0 1  -> Use Hilite Mouse Tracking.
  //     Ps = 1 0 0 1  -> Don't use Hilite Mouse Tracking.
  if (opt.vt200Hilite != null) {
    if (opt.vt200Hilite) this.setMode('?1001');
    else this.resetMode('?1001');
  }

  //     Ps = 1 0 0 2  -> Use Cell Motion Mouse Tracking.
  //     Ps = 1 0 0 2  -> Don't use Cell Motion Mouse Tracking.
  // button event mouse
  if (opt.cellMotion != null) {
    if (opt.cellMotion) this.setMode('?1002');
    else this.resetMode('?1002');
  }

  //     Ps = 1 0 0 3  -> Use All Motion Mouse Tracking.
  //     Ps = 1 0 0 3  -> Don't use All Motion Mouse Tracking.
  // any event mouse
  if (opt.allMotion != null) {
    // NOTE: Latest versions of tmux seem to only support cellMotion (not
    // allMotion). We pass all motion through to the terminal.
    if (this.tmux && this.tmuxVersion >= 2) {
      if (opt.allMotion) this._twrite('\x1b[?1003h');
      else this._twrite('\x1b[?1003l');
    } else {
      if (opt.allMotion) this.setMode('?1003');
      else this.resetMode('?1003');
    }
  }

  //     Ps = 1 0 0 4  -> Send FocusIn/FocusOut events.
  //     Ps = 1 0 0 4  -> Don't send FocusIn/FocusOut events.
  if (opt.sendFocus != null) {
    if (opt.sendFocus) this.setMode('?1004');
    else this.resetMode('?1004');
  }

  //     Ps = 1 0 0 5  -> Enable Extended Mouse Mode.
  //     Ps = 1 0 0 5  -> Disable Extended Mouse Mode.
  if (opt.utfMouse != null) {
    if (opt.utfMouse) this.setMode('?1005');
    else this.resetMode('?1005');
  }

  // sgr mouse
  if (opt.sgrMouse != null) {
    if (opt.sgrMouse) this.setMode('?1006');
    else this.resetMode('?1006');
  }

  // urxvt mouse
  if (opt.urxvtMouse != null) {
    if (opt.urxvtMouse) this.setMode('?1015');
    else this.resetMode('?1015');
  }

  // dec mouse
  if (opt.decMouse != null) {
    if (opt.decMouse) this._write('\x1b[1;2\'z\x1b[1;3\'{');
    else this._write('\x1b[\'z');
  }

  // pterm mouse
  if (opt.ptermMouse != null) {
    if (opt.ptermMouse) this._write('\x1b[>1h\x1b[>6h\x1b[>7h\x1b[>1h\x1b[>9l');
    else this._write('\x1b[>1l\x1b[>6l\x1b[>7l\x1b[>1l\x1b[>9h');
  }

  // jsbterm mouse
  if (opt.jsbtermMouse != null) {
    // + = advanced mode
    if (opt.jsbtermMouse) this._write('\x1b[0~ZwLMRK+1Q\x1b\\');
    else this._write('\x1b[0~ZwQ\x1b\\');
  }

  // gpm mouse
  if (opt.gpmMouse != null) {
    if (opt.gpmMouse) this.enableGpm();
    else this.disableGpm();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setPointerMode"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setPointerMode (param)](#apidoc.element.blessed.Program.prototype.setPointerMode)
- description and source-code
```javascript
setPointerMode = function (param) {
  return this._write('\x1b[>' + (param || '') + 'p');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setResources"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setResources ()](#apidoc.element.blessed.Program.prototype.setResources)
- description and source-code
```javascript
setResources = function () {
  return this._write('\x1b[>' + slice.call(arguments).join(';') + 'm');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setScrollRegion"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setScrollRegion (top, bottom)](#apidoc.element.blessed.Program.prototype.setScrollRegion)
- description and source-code
```javascript
setScrollRegion = function (top, bottom) {
  if (!this.zero) {
    top = (top || 1) - 1;
    bottom = (bottom || this.rows) - 1;
  } else {
    top = top || 0;
    bottom = bottom || (this.rows - 1);
  }
  this.scrollTop = top;
  this.scrollBottom = bottom;
  this.x = 0;
  this.y = 0;
  this._ncoords();
  if (this.tput) return this.put.csr(top, bottom);
  return this._write('\x1b[' + (top + 1) + ';' + (bottom + 1) + 'r');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setTerminal"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTerminal (terminal)](#apidoc.element.blessed.Program.prototype.setTerminal)
- description and source-code
```javascript
setTerminal = function (terminal) {
  this._terminal = terminal.toLowerCase();
  delete this._tputSetup;
  this.setupTput();
}
```
- example usage
```shell
...
- __aleft__ - Absolute left offset, always zero.
- __aright__ - Absolute right offset, always zero.
- __atop__ - Absolute top offset, always zero.
- __abottom__ - Absolute bottom offset, always zero.
- __grabKeys__ - Whether the focused element grabs all keypresses.
- __lockKeys__ - Prevent keypresses from being received by any element.
- __hover__ - The currently hovered element. Only set if mouse events are bound.
- __terminal__ - Set or get terminal name. 'Set' calls 'screen.setTerminal()'
  internally.
- __title__ - Set or get window title.

##### Events:

- Inherits all from Node.
- __resize__ - Received on screen resize.
...
```

#### <a name="apidoc.element.blessed.Program.prototype.setTitle"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTitle (title)](#apidoc.element.blessed.Program.prototype.setTitle)
- description and source-code
```javascript
setTitle = function (title) {
  this._title = title;

  // if (this.term('screen')) {
  //   // Tmux pane
  //   // if (this.tmux) {
  //   //   return this._write('\x1b]2;' + title + '\x1b\\');
  //   // }
  //   return this._write('\x1bk' + title + '\x1b\\');
  // }

  return this._twrite('\x1b]0;' + title + '\x07');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setTitleModeFeature"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setTitleModeFeature ()](#apidoc.element.blessed.Program.prototype.setTitleModeFeature)
- description and source-code
```javascript
setTitleModeFeature = function () {
  return this._twrite('\x1b[>' + slice.call(arguments).join(';') + 't');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setWarningBellVolume"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setWarningBellVolume (param)](#apidoc.element.blessed.Program.prototype.setWarningBellVolume)
- description and source-code
```javascript
setWarningBellVolume = function (param) {
  return this._write('\x1b[' + (param || '') + ' t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setupDump"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setupDump ()](#apidoc.element.blessed.Program.prototype.setupDump)
- description and source-code
```javascript
setupDump = function () {
  var self = this
    , write = this.output.write
    , decoder = new StringDecoder('utf8');

  function stringify(data) {
    return caret(data
      .replace(/\r/g, '\\r')
      .replace(/\n/g, '\\n')
      .replace(/\t/g, '\\t'))
      .replace(/[^ -~]/g, function(ch) {
        if (ch.charCodeAt(0) > 0xff) return ch;
        ch = ch.charCodeAt(0).toString(16);
        if (ch.length > 2) {
          if (ch.length < 4) ch = '0' + ch;
          return '\\u' + ch;
        }
        if (ch.length < 2) ch = '0' + ch;
        return '\\x' + ch;
      });
  }

  function caret(data) {
    return data.replace(/[\0\x80\x1b-\x1f\x7f\x01-\x1a]/g, function(ch) {
      switch (ch) {
        case '\0':
        case '\200':
          ch = '@';
          break;
        case '\x1b':
          ch = '[';
          break;
        case '\x1c':
          ch = '\\';
          break;
        case '\x1d':
          ch = ']';
          break;
        case '\x1e':
          ch = '^';
          break;
        case '\x1f':
          ch = '_';
          break;
        case '\x7f':
          ch = '?';
          break;
        default:
          ch = ch.charCodeAt(0);
          // From ('A' - 64) to ('Z' - 64).
          if (ch >= 1 && ch <= 26) {
            ch = String.fromCharCode(ch + 64);
          } else {
            return String.fromCharCode(ch);
          }
          break;
      }
      return '^' + ch;
    });
  }

  this.input.on('data', function(data) {
    self._log('IN', stringify(decoder.write(data)));
  });

  this.output.write = function(data) {
    self._log('OUT', stringify(data));
    return write.apply(this, arguments);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setupTput"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setupTput ()](#apidoc.element.blessed.Program.prototype.setupTput)
- description and source-code
```javascript
setupTput = function () {
  if (this._tputSetup) return;
  this._tputSetup = true;

  var self = this
    , options = this.options
    , write = this._write.bind(this);

  var tput = this.tput = new Tput({
    terminal: this.terminal,
    padding: options.padding,
    extended: options.extended,
    printf: options.printf,
    termcap: options.termcap,
    forceUnicode: options.forceUnicode
  });

  if (tput.error) {
    nextTick(function() {
      self.emit('warning', tput.error.message);
    });
  }

  if (tput.padding) {
    nextTick(function() {
      self.emit('warning', 'Terminfo padding has been enabled.');
    });
  }

  this.put = function() {
    var args = slice.call(arguments)
      , cap = args.shift();

    if (tput[cap]) {
      return this._write(tput[cap].apply(tput, args));
    }
  };

  Object.keys(tput).forEach(function(key) {
    if (self[key] == null) {
      self[key] = tput[key];
    }

    if (typeof tput[key] !== 'function') {
      self.put[key] = tput[key];
      return;
    }

    if (tput.padding) {
      self.put[key] = function() {
        return tput._print(tput[key].apply(tput, arguments), write);
      };
    } else {
      self.put[key] = function() {
        return self._write(tput[key].apply(tput, arguments));
      };
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.setx"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>setx (x)](#apidoc.element.blessed.Program.prototype.setx)
- description and source-code
```javascript
setx = function (x) {
  return this.cursorCharAbsolute(x);
  // return this.charPosAbsolute(x);
}
```
- example usage
```shell
...
program.enableMouse();
program.hideCursor();
program.clear();

program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
program.setx((program.cols / 2 | 0) - 4);
program.down(5);
program.write('Hi again!');
program.bg('!black');
program.feed();
'''
...
```

#### <a name="apidoc.element.blessed.Program.prototype.sety"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sety (y)](#apidoc.element.blessed.Program.prototype.sety)
- description and source-code
```javascript
sety = function (y) {
  return this.linePosAbsolute(y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.sgr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sgr (param, val)](#apidoc.element.blessed.Program.prototype.sgr)
- description and source-code
```javascript
sgr = function (param, val) {
  return this._write(this._attr(param, val));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.shiftIn"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>shiftIn ()](#apidoc.element.blessed.Program.prototype.shiftIn)
- description and source-code
```javascript
shiftIn = function () {
  // if (this.has('S3')) return this.put.S3();
  return this._write('\x0f');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.shiftOut"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>shiftOut ()](#apidoc.element.blessed.Program.prototype.shiftOut)
- description and source-code
```javascript
shiftOut = function () {
  // if (this.has('S2')) return this.put.S2();
  return this._write('\x0e');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.showCursor"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>showCursor ()](#apidoc.element.blessed.Program.prototype.showCursor)
- description and source-code
```javascript
showCursor = function () {
  this.cursorHidden = false;
  // NOTE: In xterm terminfo:
  // cnorm stops blinking cursor
  // cvvis starts blinking cursor
  if (this.tput) return this.put.cnorm();
  //if (this.tput) return this.put.cvvis();
  // return this._write('\x1b[?12l\x1b[?25h'); // cursor_normal
  // return this._write('\x1b[?12;25h'); // cursor_visible
  return this.setMode('?25');
}
```
- example usage
```shell
...
''' js
var blessed = require('blessed')
, program = blessed.program();

program.key('q', function(ch, key) {
program.clear();
program.disableMouse();
program.showCursor();
program.normalBuffer();
process.exit(0);
});

program.on('mouse', function(data) {
if (data.action === 'mousemove') {
  program.move(data.x, data.y);
...
```

#### <a name="apidoc.element.blessed.Program.prototype.sigtstp"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sigtstp (callback)](#apidoc.element.blessed.Program.prototype.sigtstp)
- description and source-code
```javascript
sigtstp = function (callback) {
  var resume = this.pause();

  process.once('SIGCONT', function() {
    resume();
    if (callback) callback();
  });

  process.kill(process.pid, 'SIGTSTP');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.simpleInsert"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>simpleInsert (ch, i, attr)](#apidoc.element.blessed.Program.prototype.simpleInsert)
- description and source-code
```javascript
simpleInsert = function (ch, i, attr) {
  return this._write(this.repeat(ch, i), attr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.sm"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>sm ()](#apidoc.element.blessed.Program.prototype.sm)
- description and source-code
```javascript
sm = function () {
  var param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'h');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.smacs"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>smacs ()](#apidoc.element.blessed.Program.prototype.smacs)
- description and source-code
```javascript
smacs = function () {
  return this.charset('acs');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.smcup"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>smcup ()](#apidoc.element.blessed.Program.prototype.smcup)
- description and source-code
```javascript
smcup = function () {
  this.isAlt = true;
  if (this.tput) return this.put.smcup();
  if (this.term('vt') || this.term('linux')) return;
  this.setMode('?47');
  return this.setMode('?1049');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.softReset"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>softReset ()](#apidoc.element.blessed.Program.prototype.softReset)
- description and source-code
```javascript
softReset = function () {
  //if (this.tput) return this.put.init_2string();
  //if (this.tput) return this.put.reset_2string();
  if (this.tput) return this.put.rs2();
  //return this._write('\x1b[!p');
  //return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // init
  return this._write('\x1b[!p\x1b[?3;4l\x1b[4l\x1b>'); // reset
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.su"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>su (param)](#apidoc.element.blessed.Program.prototype.su)
- description and source-code
```javascript
su = function (param) {
  this.y -= param || 1;
  this._ncoords();
  if (this.tput) return this.put.parm_index(param);
  return this._write('\x1b[' + (param || 1) + 'S');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.tab"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tab ()](#apidoc.element.blessed.Program.prototype.tab)
- description and source-code
```javascript
tab = function () {
  this.x += 8;
  this._ncoords();
  if (this.has('ht')) return this.put.ht();
  return this._write('\t');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.tabClear"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tabClear (param)](#apidoc.element.blessed.Program.prototype.tabClear)
- description and source-code
```javascript
tabClear = function (param) {
  if (this.tput) return this.put.tbc(param);
  return this._write('\x1b[' + (param || 0) + 'g');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.tabSet"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tabSet ()](#apidoc.element.blessed.Program.prototype.tabSet)
- description and source-code
```javascript
tabSet = function () {
  if (this.tput) return this.put.hts();
  return this._write('\x1bH');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.tbc"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>tbc (param)](#apidoc.element.blessed.Program.prototype.tbc)
- description and source-code
```javascript
tbc = function (param) {
  if (this.tput) return this.put.tbc(param);
  return this._write('\x1b[' + (param || 0) + 'g');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.term"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>term (is)](#apidoc.element.blessed.Program.prototype.term)
- description and source-code
```javascript
term = function (is) {
  return this.terminal.indexOf(is) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.text"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>text (text, attr)](#apidoc.element.blessed.Program.prototype.text)
- description and source-code
```javascript
text = function (text, attr) {
  return this._attr(attr, true) + text + this._attr(attr, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.unkey"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>unkey (key, listener)](#apidoc.element.blessed.Program.prototype.unkey)
- description and source-code
```javascript
unkey = function (key, listener) {
  if (typeof key === 'string') key = key.split(/\s*,\s*/);
  key.forEach(function(key) {
    return this.removeListener('key ' + key, listener);
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.up"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>up (param)](#apidoc.element.blessed.Program.prototype.up)
- description and source-code
```javascript
up = function (param) {
  this.y -= param || 1;
  this._ncoords();
  if (this.tput) {
    if (!this.tput.strings.parm_up_cursor) {
      return this._write(this.repeat(this.tput.cuu1(), param));
    }
    return this.put.cuu(param);
  }
  return this._write('\x1b[' + (param || '') + 'A');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.vi"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vi ()](#apidoc.element.blessed.Program.prototype.vi)
- description and source-code
```javascript
vi = function () {
  this.cursorHidden = true;
  if (this.tput) return this.put.civis();
  return this.resetMode('?25');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.vpa"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vpa (param)](#apidoc.element.blessed.Program.prototype.vpa)
- description and source-code
```javascript
vpa = function (param) {
  this.y = param || 1;
  this._ncoords();
  if (this.tput) {
    return this.put.vpa.apply(this.put, arguments);
  }
  param = slice.call(arguments).join(';');
  return this._write('\x1b[' + (param || '') + 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.vpr"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vpr (param)](#apidoc.element.blessed.Program.prototype.vpr)
- description and source-code
```javascript
vpr = function (param) {
  if (this.tput) return this.cud(param);
  this.y += param || 1;
  this._ncoords();
  // Does not exist:
  // if (this.tput) return this.put.vpr(param);
  return this._write('\x1b[' + (param || '') + 'e');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.vtab"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>vtab ()](#apidoc.element.blessed.Program.prototype.vtab)
- description and source-code
```javascript
vtab = function () {
  this.y++;
  this._ncoords();
  return this._write('\x0b');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Program.prototype.write"></a>[function <span class="apidocSignatureSpan">blessed.Program.prototype.</span>write (text)](#apidoc.element.blessed.Program.prototype.write)
- description and source-code
```javascript
write = function (text) {
  if (!this.output.writable) return;
  return this.output.write(text);
}
```
- example usage
```shell
...
var blessed = require('blessed');

var tput = blessed.tput({
  terminal: 'xterm-256color',
  extended: true
});

process.stdout.write(tput.setaf(4) + 'Hello' + tput.sgr0() + '\n');
'''

To play around with it on the command line, it works just like tput:

''' bash
$ tput.js setaf 2
$ tput.js sgr0
...
```



# <a name="apidoc.module.blessed.Screen"></a>[module blessed.Screen](#apidoc.module.blessed.Screen)

#### <a name="apidoc.element.blessed.Screen.Screen"></a>[function <span class="apidocSignatureSpan">blessed.</span>Screen (options)](#apidoc.element.blessed.Screen.Screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.bind"></a>[function <span class="apidocSignatureSpan">blessed.Screen.</span>bind (screen)](#apidoc.element.blessed.Screen.bind)
- description and source-code
```javascript
bind = function (screen) {
  if (!Screen.global) {
    Screen.global = screen;
  }

  if (!~Screen.instances.indexOf(screen)) {
    Screen.instances.push(screen);
    screen.index = Screen.total;
    Screen.total++;
  }

  if (Screen._bound) return;
  Screen._bound = true;

  process.on('uncaughtException', Screen._exceptionHandler = function(err) {
    if (process.listeners('uncaughtException').length > 1) {
      return;
    }
    Screen.instances.slice().forEach(function(screen) {
      screen.destroy();
    });
    err = err || new Error('Uncaught Exception.');
    console.error(err.stack ? err.stack + '' : err + '');
    nextTick(function() {
      process.exit(1);
    });
  });

  ['SIGTERM', 'SIGINT', 'SIGQUIT'].forEach(function(signal) {
    var name = '_' + signal.toLowerCase() + 'Handler';
    process.on(signal, Screen[name] = function() {
      if (process.listeners(signal).length > 1) {
        return;
      }
      nextTick(function() {
        process.exit(0);
      });
    });
  });

  process.on('exit', Screen._exitHandler = function() {
    Screen.instances.slice().forEach(function(screen) {
      screen.destroy();
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Screen.prototype"></a>[module blessed.Screen.prototype](#apidoc.module.blessed.Screen.prototype)

#### <a name="apidoc.element.blessed.Screen.prototype._cursorAttr"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_cursorAttr (cursor, dattr)](#apidoc.element.blessed.Screen.prototype._cursorAttr)
- description and source-code
```javascript
_cursorAttr = function (cursor, dattr) {
  var attr = dattr || this.dattr
    , cattr
    , ch;

  if (cursor.shape === 'line') {
    attr &= ~(0x1ff << 9);
    attr |= 7 << 9;
    ch = '\u2502';
  } else if (cursor.shape === 'underline') {
    attr &= ~(0x1ff << 9);
    attr |= 7 << 9;
    attr |= 2 << 18;
  } else if (cursor.shape === 'block') {
    attr &= ~(0x1ff << 9);
    attr |= 7 << 9;
    attr |= 8 << 18;
  } else if (typeof cursor.shape === 'object' && cursor.shape) {
    cattr = Element.prototype.sattr.call(cursor, cursor.shape);

    if (cursor.shape.bold || cursor.shape.underline
        || cursor.shape.blink || cursor.shape.inverse
        || cursor.shape.invisible) {
      attr &= ~(0x1ff << 18);
      attr |= ((cattr >> 18) & 0x1ff) << 18;
    }

    if (cursor.shape.fg) {
      attr &= ~(0x1ff << 9);
      attr |= ((cattr >> 9) & 0x1ff) << 9;
    }

    if (cursor.shape.bg) {
      attr &= ~(0x1ff << 0);
      attr |= cattr & 0x1ff;
    }

    if (cursor.shape.ch) {
      ch = cursor.shape.ch;
    }
  }

  if (cursor.color != null) {
    attr &= ~(0x1ff << 9);
    attr |= cursor.color << 9;
  }

  return {
    ch: ch,
    attr: attr
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._destroy"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_destroy ()](#apidoc.element.blessed.Screen.prototype._destroy)
- description and source-code
```javascript
_destroy = function () {
  this.detach();
  this.forDescendants(function(el) {
    el.free();
    el.destroyed = true;
    el.emit('destroy');
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._dockBorders"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_dockBorders ()](#apidoc.element.blessed.Screen.prototype._dockBorders)
- description and source-code
```javascript
_dockBorders = function () {
  var lines = this.lines
    , stops = this._borderStops
    , i
    , y
    , x
    , ch;

  // var keys, stop;
  //
  // keys = Object.keys(this._borderStops)
  //   .map(function(k) { return +k; })
  //   .sort(function(a, b) { return a - b; });
  //
  // for (i = 0; i < keys.length; i++) {
  //   y = keys[i];
  //   if (!lines[y]) continue;
  //   stop = this._borderStops[y];
  //   for (x = stop.xi; x < stop.xl; x++) {

  stops = Object.keys(stops)
    .map(function(k) { return +k; })
    .sort(function(a, b) { return a - b; });

  for (i = 0; i < stops.length; i++) {
    y = stops[i];
    if (!lines[y]) continue;
    for (x = 0; x < this.width; x++) {
      ch = lines[y][x][1];
      if (angles[ch]) {
        lines[y][x][1] = this._getAngle(lines, x, y);
        lines[y].dirty = true;
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._focus"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_focus (self, old)](#apidoc.element.blessed.Screen.prototype._focus)
- description and source-code
```javascript
_focus = function (self, old) {
  // Find a scrollable ancestor if we have one.
  var el = self;
  while (el = el.parent) {
    if (el.scrollable) break;
  }

  // If we're in a scrollable element,
  // automatically scroll to the focused element.
  if (el && !el.detached) {
    // NOTE: This is different from the other "visible" values - it needs the
    // visible height of the scrolling element itself, not the element within
    // it.
    var visible = self.screen.height - el.atop - el.itop - el.abottom - el.ibottom;
    if (self.rtop < el.childBase) {
      el.scrollTo(self.rtop);
      self.screen.render();
    } else if (self.rtop + self.height - self.ibottom > el.childBase + visible) {
      // Explanation for el.itop here: takes into account scrollable elements
      // with borders otherwise the element gets covered by the bottom border:
      el.scrollTo(self.rtop - (el.height - self.height) + el.itop, true);
      self.screen.render();
    }
  }

  if (old) {
    old.emit('blur', self);
  }

  self.emit('focus', old);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._getAngle"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_getAngle (lines, x, y)](#apidoc.element.blessed.Screen.prototype._getAngle)
- description and source-code
```javascript
_getAngle = function (lines, x, y) {
  var angle = 0
    , attr = lines[y][x][0]
    , ch = lines[y][x][1];

  if (lines[y][x - 1] && langles[lines[y][x - 1][1]]) {
    if (!this.options.ignoreDockContrast) {
      if (lines[y][x - 1][0] !== attr) return ch;
    }
    angle |= 1 << 3;
  }

  if (lines[y - 1] && uangles[lines[y - 1][x][1]]) {
    if (!this.options.ignoreDockContrast) {
      if (lines[y - 1][x][0] !== attr) return ch;
    }
    angle |= 1 << 2;
  }

  if (lines[y][x + 1] && rangles[lines[y][x + 1][1]]) {
    if (!this.options.ignoreDockContrast) {
      if (lines[y][x + 1][0] !== attr) return ch;
    }
    angle |= 1 << 1;
  }

  if (lines[y + 1] && dangles[lines[y + 1][x][1]]) {
    if (!this.options.ignoreDockContrast) {
      if (lines[y + 1][x][0] !== attr) return ch;
    }
    angle |= 1 << 0;
  }

  // Experimental: fixes this situation:
  // +----------+
  //            | <-- empty space here, should be a T angle
  // +-------+  |
  // |       |  |
  // +-------+  |
  // |          |
  // +----------+
  // if (uangles[lines[y][x][1]]) {
  //   if (lines[y + 1] && cdangles[lines[y + 1][x][1]]) {
  //     if (!this.options.ignoreDockContrast) {
  //       if (lines[y + 1][x][0] !== attr) return ch;
  //     }
  //     angle |= 1 << 0;
  //   }
  // }

  return angleTable[angle] || ch;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._getPos"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_getPos ()](#apidoc.element.blessed.Screen.prototype._getPos)
- description and source-code
```javascript
_getPos = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._initHover"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_initHover ()](#apidoc.element.blessed.Screen.prototype._initHover)
- description and source-code
```javascript
_initHover = function () {
  var self = this;

  if (this._hoverText) {
    return;
  }

  this._hoverText = new Box({
    screen: this,
    left: 0,
    top: 0,
    tags: false,
    height: 'shrink',
    width: 'shrink',
    border: 'line',
    style: {
      border: {
        fg: 'default'
      },
      bg: 'default',
      fg: 'default'
    }
  });

  this.on('mousemove', function(data) {
    if (self._hoverText.detached) return;
    self._hoverText.rleft = data.x + 1;
    self._hoverText.rtop = data.y;
    self.render();
  });

  this.on('element mouseover', function(el, data) {
    if (!el._hoverOptions) return;
    self._hoverText.parseTags = el.parseTags;
    self._hoverText.setContent(el._hoverOptions.text);
    self.append(self._hoverText);
    self._hoverText.rleft = data.x + 1;
    self._hoverText.rtop = data.y;
    self.render();
  });

  this.on('element mouseout', function() {
    if (self._hoverText.detached) return;
    self._hoverText.detach();
    self.render();
  });

  // XXX This can cause problems if the
  // terminal does not support allMotion.
  // Workaround: check to see if content is set.
  this.on('element mouseup', function(el) {
    if (!self._hoverText.getContent()) return;
    if (!el._hoverOptions) return;
    self.append(self._hoverText);
    self.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._listenKeys"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_listenKeys (el)](#apidoc.element.blessed.Screen.prototype._listenKeys)
- description and source-code
```javascript
_listenKeys = function (el) {
  var self = this;

  if (el && !~this.keyable.indexOf(el)) {
    el.keyable = true;
    this.keyable.push(el);
  }

  if (this._listenedKeys) return;
  this._listenedKeys = true;

  // NOTE: The event emissions used to be reversed:
  // element + screen
  // They are now:
  // screen + element
  // After the first keypress emitted, the handler
  // checks to make sure grabKeys, lockKeys, and focused
  // weren't changed, and handles those situations appropriately.
  this.program.on('keypress', function(ch, key) {
    if (self.lockKeys && !~self.ignoreLocked.indexOf(key.full)) {
      return;
    }

    var focused = self.focused
      , grabKeys = self.grabKeys;

    if (!grabKeys || ~self.ignoreLocked.indexOf(key.full)) {
      self.emit('keypress', ch, key);
      self.emit('key ' + key.full, ch, key);
    }

    // If something changed from the screen key handler, stop.
    if (self.grabKeys !== grabKeys || self.lockKeys) {
      return;
    }

    if (focused && focused.keyable) {
      focused.emit('keypress', ch, key);
      focused.emit('key ' + key.full, ch, key);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._listenMouse"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_listenMouse (el)](#apidoc.element.blessed.Screen.prototype._listenMouse)
- description and source-code
```javascript
_listenMouse = function (el) {
  var self = this;

  if (el && !~this.clickable.indexOf(el)) {
    el.clickable = true;
    this.clickable.push(el);
  }

  if (this._listenedMouse) return;
  this._listenedMouse = true;

  this.program.enableMouse();
  if (this.options.sendFocus) {
    this.program.setMouse({ sendFocus: true }, true);
  }

  this.on('render', function() {
    self._needsClickableSort = true;
  });

  this.program.on('mouse', function(data) {
    if (self.lockKeys) return;

    if (self._needsClickableSort) {
      self.clickable = helpers.hsort(self.clickable);
      self._needsClickableSort = false;
    }

    var i = 0
      , el
      , set
      , pos;

    for (; i < self.clickable.length; i++) {
      el = self.clickable[i];

      if (el.detached || !el.visible) {
        continue;
      }

      // if (self.grabMouse && self.focused !== el
      //     && !el.hasAncestor(self.focused)) continue;

      pos = el.lpos;
      if (!pos) continue;

      if (data.x >= pos.xi && data.x < pos.xl
          && data.y >= pos.yi && data.y < pos.yl) {
        el.emit('mouse', data);
        if (data.action === 'mousedown') {
          self.mouseDown = el;
        } else if (data.action === 'mouseup') {
          (self.mouseDown || el).emit('click', data);
          self.mouseDown = null;
        } else if (data.action === 'mousemove') {
          if (self.hover && el.index > self.hover.index) {
            set = false;
          }
          if (self.hover !== el && !set) {
            if (self.hover) {
              self.hover.emit('mouseout', data);
            }
            el.emit('mouseover', data);
            self.hover = el;
          }
          set = true;
        }
        el.emit(data.action, data);
        break;
      }
    }

    // Just mouseover?
    if ((data.action === 'mousemove'
        || data.action === 'mousedown'
        || data.action === 'mouseup')
        && self.hover
        && !set) {
      self.hover.emit('mouseout', data);
      self.hover = null;
    }

    self.emit('mouse', data);
    self.emit(data.action, data);
  });

  // Autofocus highest element.
  // this.on('element click', function(el, data) {
  //   var target;
  //   do {
  //     if (el.clickable === true && el.options.autoFocus !== false) {
  //       target = el;
  //     }
  //   } while (el = el.parent);
  //   if (target) target.focus();
  // });

  // Autofocus elements with the appropriate option.
  this.on('element click', function(el) {
    if (el.clickable === true && el.options.autoFocus !== false) {
      el.focus();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype._reduceColor"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>_reduceColor (color)](#apidoc.element.blessed.Screen.prototype._reduceColor)
- description and source-code
```javascript
_reduceColor = function (color) {
  return colors.reduce(color, this.tput.colors);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.alloc"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>alloc (dirty)](#apidoc.element.blessed.Screen.prototype.alloc)
- description and source-code
```javascript
alloc = function (dirty) {
  var x, y;

  this.lines = [];
  for (y = 0; y < this.rows; y++) {
    this.lines[y] = [];
    for (x = 0; x < this.cols; x++) {
      this.lines[y][x] = [this.dattr, ' '];
    }
    this.lines[y].dirty = !!dirty;
  }

  this.olines = [];
  for (y = 0; y < this.rows; y++) {
    this.olines[y] = [];
    for (x = 0; x < this.cols; x++) {
      this.olines[y][x] = [this.dattr, ' '];
    }
  }

  this.program.clear();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.attrCode"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>attrCode (code, cur, def)](#apidoc.element.blessed.Screen.prototype.attrCode)
- description and source-code
```javascript
attrCode = function (code, cur, def) {
  var flags = (cur >> 18) & 0x1ff
    , fg = (cur >> 9) & 0x1ff
    , bg = cur & 0x1ff
    , c
    , i;

  code = code.slice(2, -1).split(';');
  if (!code[0]) code[0] = '0';

  for (i = 0; i < code.length; i++) {
    c = +code[i] || 0;
    switch (c) {
      case 0: // normal
        bg = def & 0x1ff;
        fg = (def >> 9) & 0x1ff;
        flags = (def >> 18) & 0x1ff;
        break;
      case 1: // bold
        flags |= 1;
        break;
      case 22:
        flags = (def >> 18) & 0x1ff;
        break;
      case 4: // underline
        flags |= 2;
        break;
      case 24:
        flags = (def >> 18) & 0x1ff;
        break;
      case 5: // blink
        flags |= 4;
        break;
      case 25:
        flags = (def >> 18) & 0x1ff;
        break;
      case 7: // inverse
        flags |= 8;
        break;
      case 27:
        flags = (def >> 18) & 0x1ff;
        break;
      case 8: // invisible
        flags |= 16;
        break;
      case 28:
        flags = (def >> 18) & 0x1ff;
        break;
      case 39: // default fg
        fg = (def >> 9) & 0x1ff;
        break;
      case 49: // default bg
        bg = def & 0x1ff;
        break;
      case 100: // default fg/bg
        fg = (def >> 9) & 0x1ff;
        bg = def & 0x1ff;
        break;
      default: // color
        if (c === 48 && +code[i+1] === 5) {
          i += 2;
          bg = +code[i];
          break;
        } else if (c === 48 && +code[i+1] === 2) {
          i += 2;
          bg = colors.match(+code[i], +code[i+1], +code[i+2]);
          if (bg === -1) bg = def & 0x1ff;
          i += 2;
          break;
        } else if (c === 38 && +code[i+1] === 5) {
          i += 2;
          fg = +code[i];
          break;
        } else if (c === 38 && +code[i+1] === 2) {
          i += 2;
          fg = colors.match(+code[i], +code[i+1], +code[i+2]);
          if (fg === -1) fg = (def >> 9) & 0x1ff;
          i += 2;
          break;
        }
        if (c >= 40 && c <= 47) {
          bg = c - 40;
        } else if (c >= 100 && c <= 107) {
          bg = c - 100;
          bg += 8;
        } else if (c === 49) {
          bg = def & 0x1ff;
        } else if (c >= 30 && c <= 37) {
          fg = c - 30;
        } else if (c >= 90 && c <= 97) {
          fg = c - 90;
          fg += 8;
        } else if (c === 39) {
          fg = (def >> 9) & 0x1ff;
        } else if (c === 100) {
          fg = (def >> 9) & 0x1ff;
          bg = def & 0x1ff;
        }
        break;
    }
  }

  return (flags << 18) | (fg << 9) | bg;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.blankLine"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>blankLine (ch, dirty)](#apidoc.element.blessed.Screen.prototype.blankLine)
- description and source-code
```javascript
blankLine = function (ch, dirty) {
  var out = [];
  for (var x = 0; x < this.cols; x++) {
    out[x] = [this.dattr, ch || ' '];
  }
  out.dirty = dirty;
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.cleanSides"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cleanSides (el)](#apidoc.element.blessed.Screen.prototype.cleanSides)
- description and source-code
```javascript
cleanSides = function (el) {
  var pos = el.lpos;

  if (!pos) {
    return false;
  }

  if (pos._cleanSides != null) {
    return pos._cleanSides;
  }

  if (pos.xi <= 0 && pos.xl >= this.width) {
    return pos._cleanSides = true;
  }

  if (this.options.fastCSR) {
    // Maybe just do this instead of parsing.
    if (pos.yi < 0) return pos._cleanSides = false;
    if (pos.yl > this.height) return pos._cleanSides = false;
    if (this.width - (pos.xl - pos.xi) < 40) {
      return pos._cleanSides = true;
    }
    return pos._cleanSides = false;
  }

  if (!this.options.smartCSR) {
    return false;
  }

  // The scrollbar can't update properly, and there's also a
  // chance that the scrollbar may get moved around senselessly.
  // NOTE: In pratice, this doesn't seem to be the case.
  // if (this.scrollbar) {
  //   return pos._cleanSides = false;
  // }

  // Doesn't matter if we're only a height of 1.
  // if ((pos.yl - el.ibottom) - (pos.yi + el.itop) <= 1) {
  //   return pos._cleanSides = false;
  // }

  var yi = pos.yi + el.itop
    , yl = pos.yl - el.ibottom
    , first
    , ch
    , x
    , y;

  if (pos.yi < 0) return pos._cleanSides = false;
  if (pos.yl > this.height) return pos._cleanSides = false;
  if (pos.xi - 1 < 0) return pos._cleanSides = true;
  if (pos.xl > this.width) return pos._cleanSides = true;

  for (x = pos.xi - 1; x >= 0; x--) {
    if (!this.olines[yi]) break;
    first = this.olines[yi][x];
    for (y = yi; y < yl; y++) {
      if (!this.olines[y] || !this.olines[y][x]) break;
      ch = this.olines[y][x];
      if (ch[0] !== first[0] || ch[1] !== first[1]) {
        return pos._cleanSides = false;
      }
    }
  }

  for (x = pos.xl; x < this.width; x++) {
    if (!this.olines[yi]) break;
    first = this.olines[yi][x];
    for (y = yi; y < yl; y++) {
      if (!this.olines[y] || !this.olines[y][x]) break;
      ch = this.olines[y][x];
      if (ch[0] !== first[0] || ch[1] !== first[1]) {
        return pos._cleanSides = false;
      }
    }
  }

  return pos._cleanSides = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.clearRegion"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>clearRegion (xi, xl, yi, yl, override)](#apidoc.element.blessed.Screen.prototype.clearRegion)
- description and source-code
```javascript
clearRegion = function (xi, xl, yi, yl, override) {
  return this.fillRegion(this.dattr, ' ', xi, xl, yi, yl, override);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.codeAttr"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>codeAttr (code)](#apidoc.element.blessed.Screen.prototype.codeAttr)
- description and source-code
```javascript
codeAttr = function (code) {
  var flags = (code >> 18) & 0x1ff
    , fg = (code >> 9) & 0x1ff
    , bg = code & 0x1ff
    , out = '';

  // bold
  if (flags & 1) {
    out += '1;';
  }

  // underline
  if (flags & 2) {
    out += '4;';
  }

  // blink
  if (flags & 4) {
    out += '5;';
  }

  // inverse
  if (flags & 8) {
    out += '7;';
  }

  // invisible
  if (flags & 16) {
    out += '8;';
  }

  if (bg !== 0x1ff) {
    bg = this._reduceColor(bg);
    if (bg < 16) {
      if (bg < 8) {
        bg += 40;
      } else if (bg < 16) {
        bg -= 8;
        bg += 100;
      }
      out += bg + ';';
    } else {
      out += '48;5;' + bg + ';';
    }
  }

  if (fg !== 0x1ff) {
    fg = this._reduceColor(fg);
    if (fg < 16) {
      if (fg < 8) {
        fg += 30;
      } else if (fg < 16) {
        fg -= 8;
        fg += 90;
      }
      out += fg + ';';
    } else {
      out += '38;5;' + fg + ';';
    }
  }

  if (out[out.length - 1] === ';') out = out.slice(0, -1);

  return '\x1b[' + out + 'm';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.copyToClipboard"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>copyToClipboard (text)](#apidoc.element.blessed.Screen.prototype.copyToClipboard)
- description and source-code
```javascript
copyToClipboard = function (text) {
  return this.program.copyToClipboard(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.cursorColor"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorColor (color)](#apidoc.element.blessed.Screen.prototype.cursorColor)
- description and source-code
```javascript
cursorColor = function (color) {
  this.cursor.color = color != null
    ? colors.convert(color)
    : null;
  this.cursor._set = true;

  if (this.cursor.artificial) {
    return true;
  }

  return this.program.cursorColor(colors.ncolors[this.cursor.color]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.cursorReset"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorReset ()](#apidoc.element.blessed.Screen.prototype.cursorReset)
- description and source-code
```javascript
cursorReset = function () {
  this.cursor.shape = 'block';
  this.cursor.blink = false;
  this.cursor.color = null;
  this.cursor._set = false;

  if (this.cursor.artificial) {
    this.cursor.artificial = false;
    if (this.program.hideCursor_old) {
      this.program.hideCursor = this.program.hideCursor_old;
      delete this.program.hideCursor_old;
    }
    if (this.program.showCursor_old) {
      this.program.showCursor = this.program.showCursor_old;
      delete this.program.showCursor_old;
    }
    if (this._cursorBlink) {
      clearInterval(this._cursorBlink);
      delete this._cursorBlink;
    }
    return true;
  }

  return this.program.cursorReset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.cursorShape"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>cursorShape (shape, blink)](#apidoc.element.blessed.Screen.prototype.cursorShape)
- description and source-code
```javascript
cursorShape = function (shape, blink) {
  var self = this;

  this.cursor.shape = shape || 'block';
  this.cursor.blink = blink || false;
  this.cursor._set = true;

  if (this.cursor.artificial) {
    if (!this.program.hideCursor_old) {
      var hideCursor = this.program.hideCursor;
      this.program.hideCursor_old = this.program.hideCursor;
      this.program.hideCursor = function() {
        hideCursor.call(self.program);
        self.cursor._hidden = true;
        if (self.renders) self.render();
      };
    }
    if (!this.program.showCursor_old) {
      var showCursor = this.program.showCursor;
      this.program.showCursor_old = this.program.showCursor;
      this.program.showCursor = function() {
        self.cursor._hidden = false;
        if (self.program._exiting) showCursor.call(self.program);
        if (self.renders) self.render();
      };
    }
    if (!this._cursorBlink) {
      this._cursorBlink = setInterval(function() {
        if (!self.cursor.blink) return;
        self.cursor._state ^= 1;
        if (self.renders) self.render();
      }, 500);
      if (this._cursorBlink.unref) {
        this._cursorBlink.unref();
      }
    }
    return true;
  }

  return this.program.cursorShape(this.cursor.shape, this.cursor.blink);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.debug"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>debug ()](#apidoc.element.blessed.Screen.prototype.debug)
- description and source-code
```javascript
debug = function () {
  if (this.debugLog) {
    this.debugLog.log.apply(this.debugLog, arguments);
  }
  return this.program.debug.apply(this.program, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.deleteBottom"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteBottom (top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteBottom)
- description and source-code
```javascript
deleteBottom = function (top, bottom) {
  return this.clearRegion(0, this.width, bottom, bottom);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.deleteLine"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteLine (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteLine)
- description and source-code
```javascript
deleteLine = function (n, y, top, bottom) {
  // if (y === top) return this.deleteLineNC(n, y, top, bottom);

  if (!this.tput.strings.change_scroll_region
      || !this.tput.strings.delete_line
      || !this.tput.strings.insert_line) return;

  this._buf += this.tput.csr(top, bottom);
  this._buf += this.tput.cup(y, 0);
  this._buf += this.tput.dl(n);
  this._buf += this.tput.csr(0, this.height - 1);

  var j = bottom + 1;

  while (n--) {
    this.lines.splice(j, 0, this.blankLine());
    this.lines.splice(y, 1);
    this.olines.splice(j, 0, this.blankLine());
    this.olines.splice(y, 1);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.deleteLineNC"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteLineNC (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteLineNC)
- description and source-code
```javascript
deleteLineNC = function (n, y, top, bottom) {
  if (!this.tput.strings.change_scroll_region
      || !this.tput.strings.delete_line) return;

  this._buf += this.tput.csr(top, bottom);
  this._buf += this.tput.cup(bottom, 0);
  this._buf += Array(n + 1).join('\n');
  this._buf += this.tput.csr(0, this.height - 1);

  var j = bottom + 1;

  while (n--) {
    this.lines.splice(j, 0, this.blankLine());
    this.lines.splice(y, 1);
    this.olines.splice(j, 0, this.blankLine());
    this.olines.splice(y, 1);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.deleteTop"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>deleteTop (top, bottom)](#apidoc.element.blessed.Screen.prototype.deleteTop)
- description and source-code
```javascript
deleteTop = function (top, bottom) {
  // Same as: return this.insertBottom(top, bottom);
  return this.deleteLine(1, top, top, bottom);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.destroy"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>destroy ()](#apidoc.element.blessed.Screen.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.leave();

  var index = Screen.instances.indexOf(this);
  if (~index) {
    Screen.instances.splice(index, 1);
    Screen.total--;

    Screen.global = Screen.instances[0];

    if (Screen.total === 0) {
      Screen.global = null;

      process.removeListener('uncaughtException', Screen._exceptionHandler);
      process.removeListener('SIGTERM', Screen._sigtermHandler);
      process.removeListener('SIGINT', Screen._sigintHandler);
      process.removeListener('SIGQUIT', Screen._sigquitHandler);
      process.removeListener('exit', Screen._exitHandler);
      delete Screen._exceptionHandler;
      delete Screen._sigtermHandler;
      delete Screen._sigintHandler;
      delete Screen._sigquitHandler;
      delete Screen._exitHandler;

      delete Screen._bound;
    }

    this.destroyed = true;
    this.emit('destroy');
    this._destroy();
  }

  this.program.destroy();
}
```
- example usage
```shell
...
  output: client,
  terminal: 'xterm-256color',
  fullUnicode: true
});

client.on('close', function() {
  if (!screen.destroyed) {
    screen.destroy();
  }
});

screen.key(['C-c', 'q'], function(ch, key) {
  screen.destroy();
});
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.displayImage"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>displayImage (file, callback)](#apidoc.element.blessed.Screen.prototype.displayImage)
- description and source-code
```javascript
displayImage = function (file, callback) {
  if (!file) {
    if (!callback) return;
    return callback(new Error('No image.'));
  }

  file = path.resolve(process.cwd(), file);

  if (!~file.indexOf('://')) {
    file = 'file://' + file;
  }

  var args = ['w3m', '-T', 'text/html'];

  var input = '<title>press q to exit</title>'
    + '<img align="center" src="' + file + '">';

  var opt = {
    stdio: ['pipe', 1, 2],
    env: process.env,
    cwd: process.env.HOME
  };

  var ps = this.spawn(args[0], args.slice(1), opt);

  ps.on('error', function(err) {
    if (!callback) return;
    return callback(err);
  });

  ps.on('exit', function(code) {
    if (!callback) return;
    if (code !== 0) return callback(new Error('Exit Code: ' + code));
    return callback(null, code === 0);
  });

  ps.stdin.write(input + '\n');
  ps.stdin.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.draw"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>draw (start, end)](#apidoc.element.blessed.Screen.prototype.draw)
- description and source-code
```javascript
draw = function (start, end) {
  // this.emit('predraw');

  var x
    , y
    , line
    , out
    , ch
    , data
    , attr
    , fg
    , bg
    , flags;

  var main = ''
    , pre
    , post;

  var clr
    , neq
    , xx;

  var lx = -1
    , ly = -1
    , o;

  var acs;

  if (this._buf) {
    main += this._buf;
    this._buf = '';
  }

  for (y = start; y <= end; y++) {
    line = this.lines[y];
    o = this.olines[y];

    if (!line.dirty && !(this.cursor.artificial && y === this.program.y)) {
      continue;
    }
    line.dirty = false;

    out = '';
    attr = this.dattr;

    for (x = 0; x < line.length; x++) {
      data = line[x][0];
      ch = line[x][1];

      // Render the artificial cursor.
      if (this.cursor.artificial
          && !this.cursor._hidden
          && this.cursor._state
          && x === this.program.x
          && y === this.program.y) {
        var cattr = this._cursorAttr(this.cursor, data);
        if (cattr.ch) ch = cattr.ch;
        data = cattr.attr;
      }

      // Take advantage of xterm's back_color_erase feature by using a
      // lookahead. Stop spitting out so many damn spaces. NOTE: Is checking
      // the bg for non BCE terminals worth the overhead?
      if (this.options.useBCE
          && ch === ' '
          && (this.tput.bools.back_color_erase
          || (data & 0x1ff) === (this.dattr & 0x1ff))
          && ((data >> 18) & 8) === ((this.dattr >> 18) & 8)) {
        clr = true;
        neq = false;

        for (xx = x; xx < line.length; xx++) {
          if (line[xx][0] !== data || line[xx][1] !== ' ') {
            clr = false;
            break;
          }
          if (line[xx][0] !== o[xx][0] || line[xx][1] !== o[xx][1]) {
            neq = true;
          }
        }

        if (clr && neq) {
          lx = -1, ly = -1;
          if (data !== attr) {
            out += this.codeAttr(data);
            attr = data;
          }
          out += this.tput.cup(y, x);
          out += this.tput.el();
          for (xx = x; xx < line.length; xx++) {
            o[xx][0] = data;
            o[xx][1] = ' ';
          }
          break;
        }

        // If there's more than 10 spaces, use EL regardless
        // and start over drawing the rest of line. Might
        // not be worth it. Try to use ECH if the terminal
        // supports it. Maybe only try to use ECH here.
        // //if (this.tput.strings.erase_chars)
        // if (!clr && neq && (xx - x) > 10) {
        //   lx = -1, ly = -1;
        //   if (data !== attr) {
        //     out += this.codeAttr(data);
        //     attr = data;
        //   }
        //   out += this.tput.cup(y, x);
        //   if (this.tput.strings.erase_chars) {
        //     // Use erase_chars to avoid erasing the whole line.
        //     out += this.tput.ech(xx - x);
        //   } else {
        //     out += this.tput.el();
        //   }
        //   if (this.tput.strings.parm_right_cursor) {
        //     out += this.tput.cuf(xx - x);
        //   } else {
        //     out += this.tput.cup(y, xx);
        //   }
        //   this.fillRegion(data, ' ',
        //     x, this.tput.strings.erase_chars ? xx : line.length,
        //     y, y + 1);
        //   x = xx - 1;
        //   continue;
        // }

        // Skip to the next line if the
        // rest of the line is already drawn.
        // if (!neq) {
        //   for (; xx < line.length; xx++) {
        //     if (line[xx][0] !== o[xx][0] || line[xx][1] !== o[xx][1]) {
        //       neq = true;
        //       break;
        //     }
        //   }
        //   if (!neq) {
        //     attr = data;
        //     break;
        //   }
        // }
      }

      // Optimize by comparing the real output
      // buffer to the pending output buffer.
      if (data === o[x][0] && ch === o[x][1]) {
        if (lx === -1) {
          lx = x;
          ly = y;
        }
        continue;
      } else if (lx !== -1) {
        if (this.tput.strings.parm_right_cursor) {
          out += y === ly
            ? this.tput.cuf(x - lx)
            : this. ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.enableInput"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableInput (el)](#apidoc.element.blessed.Screen.prototype.enableInput)
- description and source-code
```javascript
enableInput = function (el) {
  this._listenMouse(el);
  this._listenKeys(el);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.enableKeys"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableKeys (el)](#apidoc.element.blessed.Screen.prototype.enableKeys)
- description and source-code
```javascript
enableKeys = function (el) {
  this._listenKeys(el);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.enableMouse"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enableMouse (el)](#apidoc.element.blessed.Screen.prototype.enableMouse)
- description and source-code
```javascript
enableMouse = function (el) {
  this._listenMouse(el);
}
```
- example usage
```shell
...
- __resize__ - Received on screen resize.
- __mouse__ - Received on mouse events.
- __keypress__ - Received on key events.
- __element [name]__ - Global events received for all elements.
- __key [name]__ - Received on key event for [name].
- __focus, blur__ - Received when the terminal window focuses/blurs. Requires a
terminal supporting the focus protocol and focus needs to be passed to
program.enableMouse().
- __prerender__ - Received before render.
- __render__ - Received on render.
- __warning__ - Received when blessed notices something untoward (output is not
a tty, terminfo not found, etc).
- __destroy__ - Received when the screen is destroyed (only useful when using
multiple screens).
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.enter"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>enter ()](#apidoc.element.blessed.Screen.prototype.enter)
- description and source-code
```javascript
enter = function () {
  if (this.program.isAlt) return;
  if (!this.cursor._set) {
    if (this.options.cursor.shape) {
      this.cursorShape(this.cursor.shape, this.cursor.blink);
    }
    if (this.options.cursor.color) {
      this.cursorColor(this.cursor.color);
    }
  }
  if (process.platform === 'win32') {
    try {
      cp.execSync('cls', { stdio: 'ignore', timeout: 1000 });
    } catch (e) {
      ;
    }
  }
  this.program.alternateBuffer();
  this.program.put.keypad_xmit();
  this.program.csr(0, this.height - 1);
  this.program.hideCursor();
  this.program.cup(0, 0);
  // We need this for tmux now:
  if (this.tput.strings.ena_acs) {
    this.program._write(this.tput.enacs());
  }
  this.alloc();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.exec"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>exec (file, args, options, callback)](#apidoc.element.blessed.Screen.prototype.exec)
- description and source-code
```javascript
exec = function (file, args, options, callback) {
  var ps = this.spawn(file, args, options);

  ps.on('error', function(err) {
    if (!callback) return;
    return callback(err, false);
  });

  ps.on('exit', function(code) {
    if (!callback) return;
    return callback(null, code === 0);
  });

  return ps;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.fillRegion"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>fillRegion (attr, ch, xi, xl, yi, yl, override)](#apidoc.element.blessed.Screen.prototype.fillRegion)
- description and source-code
```javascript
fillRegion = function (attr, ch, xi, xl, yi, yl, override) {
  var lines = this.lines
    , cell
    , xx;

  if (xi < 0) xi = 0;
  if (yi < 0) yi = 0;

  for (; yi < yl; yi++) {
    if (!lines[yi]) break;
    for (xx = xi; xx < xl; xx++) {
      cell = lines[yi][xx];
      if (!cell) break;
      if (override || attr !== cell[0] || ch !== cell[1]) {
        lines[yi][xx][0] = attr;
        lines[yi][xx][1] = ch;
        lines[yi].dirty = true;
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusNext"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusNext ()](#apidoc.element.blessed.Screen.prototype.focusNext)
- description and source-code
```javascript
focusNext = function () {
  return this.focusOffset(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusOffset"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusOffset (offset)](#apidoc.element.blessed.Screen.prototype.focusOffset)
- description and source-code
```javascript
focusOffset = function (offset) {
  var shown = this.keyable.filter(function(el) {
    return !el.detached && el.visible;
  }).length;

  if (!shown || !offset) {
    return;
  }

  var i = this.keyable.indexOf(this.focused);
  if (!~i) return;

  if (offset > 0) {
    while (offset--) {
      if (++i > this.keyable.length - 1) i = 0;
      if (this.keyable[i].detached || !this.keyable[i].visible) offset++;
    }
  } else {
    offset = -offset;
    while (offset--) {
      if (--i < 0) i = this.keyable.length - 1;
      if (this.keyable[i].detached || !this.keyable[i].visible) offset++;
    }
  }

  return this.keyable[i].focus();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusPop"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPop ()](#apidoc.element.blessed.Screen.prototype.focusPop)
- description and source-code
```javascript
focusPop = function () {
  var old = this.history.pop();
  if (this.history.length) {
    this._focus(this.history[this.history.length - 1], old);
  }
  return old;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusPrev"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPrev ()](#apidoc.element.blessed.Screen.prototype.focusPrev)
- description and source-code
```javascript
focusPrev = function () {
  return this.focusOffset(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusPrevious"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPrevious ()](#apidoc.element.blessed.Screen.prototype.focusPrevious)
- description and source-code
```javascript
focusPrevious = function () {
  return this.focusOffset(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.focusPush"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>focusPush (el)](#apidoc.element.blessed.Screen.prototype.focusPush)
- description and source-code
```javascript
focusPush = function (el) {
  if (!el) return;
  var old = this.history[this.history.length - 1];
  if (this.history.length === 10) {
    this.history.shift();
  }
  this.history.push(el);
  this._focus(el, old);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.insertBottom"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertBottom (top, bottom)](#apidoc.element.blessed.Screen.prototype.insertBottom)
- description and source-code
```javascript
insertBottom = function (top, bottom) {
  return this.deleteLine(1, top, top, bottom);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.insertLine"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertLine (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.insertLine)
- description and source-code
```javascript
insertLine = function (n, y, top, bottom) {
  // if (y === top) return this.insertLineNC(n, y, top, bottom);

  if (!this.tput.strings.change_scroll_region
      || !this.tput.strings.delete_line
      || !this.tput.strings.insert_line) return;

  this._buf += this.tput.csr(top, bottom);
  this._buf += this.tput.cup(y, 0);
  this._buf += this.tput.il(n);
  this._buf += this.tput.csr(0, this.height - 1);

  var j = bottom + 1;

  while (n--) {
    this.lines.splice(y, 0, this.blankLine());
    this.lines.splice(j, 1);
    this.olines.splice(y, 0, this.blankLine());
    this.olines.splice(j, 1);
  }
}
```
- example usage
```shell
...
  screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
  box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
  box.setLine(1, 'bar');
  box.insertLine(1, 'foo');
  screen.render();
});

// Quit on Escape, q, or Control-C.
screen.key(['escape', 'q', 'C-c'], function(ch, key) {
  return process.exit(0);
});
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.insertLineNC"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertLineNC (n, y, top, bottom)](#apidoc.element.blessed.Screen.prototype.insertLineNC)
- description and source-code
```javascript
insertLineNC = function (n, y, top, bottom) {
  if (!this.tput.strings.change_scroll_region
      || !this.tput.strings.delete_line) return;

  this._buf += this.tput.csr(top, bottom);
  this._buf += this.tput.cup(top, 0);
  this._buf += this.tput.dl(n);
  this._buf += this.tput.csr(0, this.height - 1);

  var j = bottom + 1;

  while (n--) {
    this.lines.splice(j, 0, this.blankLine());
    this.lines.splice(y, 1);
    this.olines.splice(j, 0, this.blankLine());
    this.olines.splice(y, 1);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.insertTop"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>insertTop (top, bottom)](#apidoc.element.blessed.Screen.prototype.insertTop)
- description and source-code
```javascript
insertTop = function (top, bottom) {
  return this.insertLine(1, top, top, bottom);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.key"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>key ()](#apidoc.element.blessed.Screen.prototype.key)
- description and source-code
```javascript
key = function () {
  return this.program.key.apply(this, arguments);
}
```
- example usage
```shell
...
// If our box is clicked, change the content.
box.on('click', function(data) {
  box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
  screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
  box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
  box.setLine(1, 'bar');
  box.insertLine(1, 'foo');
  screen.render();
});

// Quit on Escape, q, or Control-C.
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.leave"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>leave ()](#apidoc.element.blessed.Screen.prototype.leave)
- description and source-code
```javascript
leave = function () {
  if (!this.program.isAlt) return;
  this.program.put.keypad_local();
  if (this.program.scrollTop !== 0
      || this.program.scrollBottom !== this.rows - 1) {
    this.program.csr(0, this.height - 1);
  }
  // XXX For some reason if alloc/clear() is before this
  // line, it doesn't work on linux console.
  this.program.showCursor();
  this.alloc();
  if (this._listenedMouse) {
    this.program.disableMouse();
  }
  this.program.normalBuffer();
  if (this.cursor._set) this.cursorReset();
  this.program.flush();
  if (process.platform === 'win32') {
    try {
      cp.execSync('cls', { stdio: 'ignore', timeout: 1000 });
    } catch (e) {
      ;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.log"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>log ()](#apidoc.element.blessed.Screen.prototype.log)
- description and source-code
```javascript
log = function () {
  return this.program.log.apply(this.program, arguments);
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.onceKey"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>onceKey ()](#apidoc.element.blessed.Screen.prototype.onceKey)
- description and source-code
```javascript
onceKey = function () {
  return this.program.onceKey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.postEnter"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>postEnter ()](#apidoc.element.blessed.Screen.prototype.postEnter)
- description and source-code
```javascript
postEnter = function () {
  var self = this;
  if (this.options.debug) {
    this.debugLog = new Log({
      screen: this,
      parent: this,
      hidden: true,
      draggable: true,
      left: 'center',
      top: 'center',
      width: '30%',
      height: '30%',
      border: 'line',
      label: ' {bold}Debug Log{/bold} ',
      tags: true,
      keys: true,
      vi: true,
      mouse: true,
      scrollbar: {
        ch: ' ',
        track: {
          bg: 'yellow'
        },
        style: {
          inverse: true
        }
      }
    });

    this.debugLog.toggle = function() {
      if (self.debugLog.hidden) {
        self.saveFocus();
        self.debugLog.show();
        self.debugLog.setFront();
        self.debugLog.focus();
      } else {
        self.debugLog.hide();
        self.restoreFocus();
      }
      self.render();
    };

    this.debugLog.key(['q', 'escape'], self.debugLog.toggle);
    this.key('f12', self.debugLog.toggle);
  }

  if (this.options.warnings) {
    this.on('warning', function(text) {
      var warning = new Box({
        screen: self,
        parent: self,
        left: 'center',
        top: 'center',
        width: 'shrink',
        padding: 1,
        height: 'shrink',
        align: 'center',
        valign: 'middle',
        border: 'line',
        label: ' {red-fg}{bold}WARNING{/} ',
        content: '{bold}' + text + '{/bold}',
        tags: true
      });
      self.render();
      var timeout = setTimeout(function() {
        warning.destroy();
        self.render();
      }, 1500);
      if (timeout.unref) {
        timeout.unref();
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.readEditor"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>readEditor (options, callback)](#apidoc.element.blessed.Screen.prototype.readEditor)
- description and source-code
```javascript
readEditor = function (options, callback) {
  if (typeof options === 'string') {
    options = { editor: options };
  }

  if (!callback) {
    callback = options;
    options = null;
  }

  if (!callback) {
    callback = function() {};
  }

  options = options || {};

  var self = this
    , editor = options.editor || process.env.EDITOR || 'vi'
    , name = options.name || process.title || 'blessed'
    , rnd = Math.random().toString(36).split('.').pop()
    , file = '/tmp/' + name + '.' + rnd
    , args = [file]
    , opt;

  opt = {
    stdio: 'inherit',
    env: process.env,
    cwd: process.env.HOME
  };

  function writeFile(callback) {
    if (!options.value) return callback();
    return fs.writeFile(file, options.value, callback);
  }

  return writeFile(function(err) {
    if (err) return callback(err);
    return self.exec(editor, args, opt, function(err, success) {
      if (err) return callback(err);
      return fs.readFile(file, 'utf8', function(err, data) {
        return fs.unlink(file, function() {
          if (!success) return callback(new Error('Unsuccessful.'));
          if (err) return callback(err);
          return callback(null, data);
        });
      });
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.realloc"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>realloc ()](#apidoc.element.blessed.Screen.prototype.realloc)
- description and source-code
```javascript
realloc = function () {
  return this.alloc(true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.removeKey"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>removeKey ()](#apidoc.element.blessed.Screen.prototype.removeKey)
- description and source-code
```javascript
removeKey = function () {
  return this.program.unkey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>render ()](#apidoc.element.blessed.Screen.prototype.render)
- description and source-code
```javascript
render = function () {
  var self = this;

  if (this.destroyed) return;

  this.emit('prerender');

  this._borderStops = {};

  // TODO: Possibly get rid of .dirty altogether.
  // TODO: Could possibly drop .dirty and just clear the 'lines' buffer every
  // time before a screen.render. This way clearRegion doesn't have to be
  // called in arbitrary places for the sake of clearing a spot where an
  // element used to be (e.g. when an element moves or is hidden). There could
  // be some overhead though.
  // this.screen.clearRegion(0, this.cols, 0, this.rows);
  this._ci = 0;
  this.children.forEach(function(el) {
    el.index = self._ci++;
    //el._rendering = true;
    el.render();
    //el._rendering = false;
  });
  this._ci = -1;

  if (this.screen.dockBorders) {
    this._dockBorders();
  }

  this.draw(0, this.lines.length - 1);

  // XXX Workaround to deal with cursor pos before the screen has rendered and
  // lpos is not reliable (stale).
  if (this.focused && this.focused._updateCursor) {
    this.focused._updateCursor(true);
  }

  this.renders++;

  this.emit('render');
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.resetCursor"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>resetCursor ()](#apidoc.element.blessed.Screen.prototype.resetCursor)
- description and source-code
```javascript
resetCursor = function () {
  this.cursor.shape = 'block';
  this.cursor.blink = false;
  this.cursor.color = null;
  this.cursor._set = false;

  if (this.cursor.artificial) {
    this.cursor.artificial = false;
    if (this.program.hideCursor_old) {
      this.program.hideCursor = this.program.hideCursor_old;
      delete this.program.hideCursor_old;
    }
    if (this.program.showCursor_old) {
      this.program.showCursor = this.program.showCursor_old;
      delete this.program.showCursor_old;
    }
    if (this._cursorBlink) {
      clearInterval(this._cursorBlink);
      delete this._cursorBlink;
    }
    return true;
  }

  return this.program.cursorReset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.restoreFocus"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>restoreFocus ()](#apidoc.element.blessed.Screen.prototype.restoreFocus)
- description and source-code
```javascript
restoreFocus = function () {
  if (!this._savedFocus) return;
  this._savedFocus.focus();
  delete this._savedFocus;
  return this.focused;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.rewindFocus"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>rewindFocus ()](#apidoc.element.blessed.Screen.prototype.rewindFocus)
- description and source-code
```javascript
rewindFocus = function () {
  var old = this.history.pop()
    , el;

  while (this.history.length) {
    el = this.history.pop();
    if (!el.detached && el.visible) {
      this.history.push(el);
      this._focus(el, old);
      return el;
    }
  }

  if (old) {
    old.emit('blur');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.saveFocus"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>saveFocus ()](#apidoc.element.blessed.Screen.prototype.saveFocus)
- description and source-code
```javascript
saveFocus = function () {
  return this._savedFocus = this.focused;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.screenshot"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>screenshot (xi, xl, yi, yl, term)](#apidoc.element.blessed.Screen.prototype.screenshot)
- description and source-code
```javascript
screenshot = function (xi, xl, yi, yl, term) {
  if (xi == null) xi = 0;
  if (xl == null) xl = this.cols;
  if (yi == null) yi = 0;
  if (yl == null) yl = this.rows;

  if (xi < 0) xi = 0;
  if (yi < 0) yi = 0;

  var x
    , y
    , line
    , out
    , ch
    , data
    , attr;

  var sdattr = this.dattr;

  if (term) {
    this.dattr = term.defAttr;
  }

  var main = '';

  for (y = yi; y < yl; y++) {
    line = term
      ? term.lines[y]
      : this.lines[y];

    if (!line) break;

    out = '';
    attr = this.dattr;

    for (x = xi; x < xl; x++) {
      if (!line[x]) break;

      data = line[x][0];
      ch = line[x][1];

      if (data !== attr) {
        if (attr !== this.dattr) {
          out += '\x1b[m';
        }
        if (data !== this.dattr) {
          var _data = data;
          if (term) {
            if (((_data >> 9) & 0x1ff) === 257) _data |= 0x1ff << 9;
            if ((_data & 0x1ff) === 256) _data |= 0x1ff;
          }
          out += this.codeAttr(_data);
        }
      }

      if (this.fullUnicode) {
        if (unicode.charWidth(line[x][1]) === 2) {
          if (x === xl - 1) {
            ch = ' ';
          } else {
            x++;
          }
        }
      }

      out += ch;
      attr = data;
    }

    if (attr !== this.dattr) {
      out += '\x1b[m';
    }

    if (out) {
      main += (y > 0 ? '\n' : '') + out;
    }
  }

  main = main.replace(/(?:\s*\x1b\[40m\s*\x1b\[m\s*)*$/, '') + '\n';

  if (term) {
    this.dattr = sdattr;
  }

  return main;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.setEffects"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>setEffects (el, fel, over, out, effects, temp)](#apidoc.element.blessed.Screen.prototype.setEffects)
- description and source-code
```javascript
setEffects = function (el, fel, over, out, effects, temp) {
  if (!effects) return;

  var tmp = {};
  if (temp) el[temp] = tmp;

  if (typeof el !== 'function') {
    var _el = el;
    el = function() { return _el; };
  }

  fel.on(over, function() {
    var element = el();
    Object.keys(effects).forEach(function(key) {
      var val = effects[key];
      if (val !== null && typeof val === 'object') {
        tmp[key] = tmp[key] || {};
        // element.style[key] = element.style[key] || {};
        Object.keys(val).forEach(function(k) {
          var v = val[k];
          tmp[key][k] = element.style[key][k];
          element.style[key][k] = v;
        });
        return;
      }
      tmp[key] = element.style[key];
      element.style[key] = val;
    });
    element.screen.render();
  });

  fel.on(out, function() {
    var element = el();
    Object.keys(effects).forEach(function(key) {
      var val = effects[key];
      if (val !== null && typeof val === 'object') {
        tmp[key] = tmp[key] || {};
        // element.style[key] = element.style[key] || {};
        Object.keys(val).forEach(function(k) {
          if (tmp[key].hasOwnProperty(k)) {
            element.style[key][k] = tmp[key][k];
          }
        });
        return;
      }
      if (tmp.hasOwnProperty(key)) {
        element.style[key] = tmp[key];
      }
    });
    element.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.setTerminal"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>setTerminal (terminal)](#apidoc.element.blessed.Screen.prototype.setTerminal)
- description and source-code
```javascript
setTerminal = function (terminal) {
  var entered = !!this.program.isAlt;
  if (entered) {
    this._buf = '';
    this.program._buf = '';
    this.leave();
  }
  this.program.setTerminal(terminal);
  this.tput = this.program.tput;
  if (entered) {
    this.enter();
  }
}
```
- example usage
```shell
...
- __aleft__ - Absolute left offset, always zero.
- __aright__ - Absolute right offset, always zero.
- __atop__ - Absolute top offset, always zero.
- __abottom__ - Absolute bottom offset, always zero.
- __grabKeys__ - Whether the focused element grabs all keypresses.
- __lockKeys__ - Prevent keypresses from being received by any element.
- __hover__ - The currently hovered element. Only set if mouse events are bound.
- __terminal__ - Set or get terminal name. 'Set' calls 'screen.setTerminal()'
  internally.
- __title__ - Set or get window title.

##### Events:

- Inherits all from Node.
- __resize__ - Received on screen resize.
...
```

#### <a name="apidoc.element.blessed.Screen.prototype.sigtstp"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>sigtstp (callback)](#apidoc.element.blessed.Screen.prototype.sigtstp)
- description and source-code
```javascript
sigtstp = function (callback) {
  var self = this;
  this.program.sigtstp(function() {
    self.alloc();
    self.render();
    self.program.lrestoreCursor('pause', true);
    if (callback) callback();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.spawn"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>spawn (file, args, options)](#apidoc.element.blessed.Screen.prototype.spawn)
- description and source-code
```javascript
spawn = function (file, args, options) {
  if (!Array.isArray(args)) {
    options = args;
    args = [];
  }

  var screen = this
    , program = screen.program
    , spawn = require('child_process').spawn
    , mouse = program.mouseEnabled
    , ps;

  options = options || {};

  options.stdio = options.stdio || 'inherit';

  program.lsaveCursor('spawn');
  // program.csr(0, program.rows - 1);
  program.normalBuffer();
  program.showCursor();
  if (mouse) program.disableMouse();

  var write = program.output.write;
  program.output.write = function() {};
  program.input.pause();
  if (program.input.setRawMode) {
    program.input.setRawMode(false);
  }

  var resume = function() {
    if (resume.done) return;
    resume.done = true;

    if (program.input.setRawMode) {
      program.input.setRawMode(true);
    }
    program.input.resume();
    program.output.write = write;

    program.alternateBuffer();
    // program.csr(0, program.rows - 1);
    if (mouse) {
      program.enableMouse();
      if (screen.options.sendFocus) {
        screen.program.setMouse({ sendFocus: true }, true);
      }
    }

    screen.alloc();
    screen.render();

    screen.program.lrestoreCursor('spawn', true);
  };

  ps = spawn(file, args, options);

  ps.on('error', resume);

  ps.on('exit', resume);

  return ps;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Screen.prototype.unkey"></a>[function <span class="apidocSignatureSpan">blessed.Screen.prototype.</span>unkey ()](#apidoc.element.blessed.Screen.prototype.unkey)
- description and source-code
```javascript
unkey = function () {
  return this.program.unkey.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Tput"></a>[module blessed.Tput](#apidoc.module.blessed.Tput)

#### <a name="apidoc.element.blessed.Tput.Tput"></a>[function <span class="apidocSignatureSpan">blessed.</span>Tput (options)](#apidoc.element.blessed.Tput.Tput)
- description and source-code
```javascript
function Tput(options) {
  if (!(this instanceof Tput)) {
    return new Tput(options);
  }

  options = options || {};
  if (typeof options === 'string') {
    options = { terminal: options };
  }

  this.options = options;
  this.terminal = options.terminal
    || options.term
    || process.env.TERM
    || (process.platform === 'win32' ? 'windows-ansi' : 'xterm');

  this.terminal = this.terminal.toLowerCase();

  this.debug = options.debug;
  this.padding = options.padding;
  this.extended = options.extended;
  this.printf = options.printf;
  this.termcap = options.termcap;
  this.error = null;

  this.terminfoPrefix = options.terminfoPrefix;
  this.terminfoFile = options.terminfoFile;
  this.termcapFile = options.termcapFile;

  if (options.terminal || options.term) {
    this.setup();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput._prefix"></a>[function <span class="apidocSignatureSpan">blessed.Tput.</span>_prefix (term)](#apidoc.element.blessed.Tput._prefix)
- description and source-code
```javascript
_prefix = function (term) {
  // If we have a terminfoFile, or our
  // term looks like a filename, use it.
  if (term) {
    if (~term.indexOf(path.sep)) {
      return term;
    }
    if (this.terminfoFile) {
      return this.terminfoFile;
    }
  }

  var paths = Tput.ipaths.slice()
    , file;

  if (this.terminfoPrefix) {
    paths.unshift(this.terminfoPrefix);
  }

  // Try exact matches.
  file = this._tprefix(paths, term);
  if (file) return file;

  // Try similar matches.
  file = this._tprefix(paths, term, true);
  if (file) return file;

  // Not found.
  throw new Error('Terminfo directory not found.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput._tprefix"></a>[function <span class="apidocSignatureSpan">blessed.Tput.</span>_tprefix (prefix, term, soft)](#apidoc.element.blessed.Tput._tprefix)
- description and source-code
```javascript
_tprefix = function (prefix, term, soft) {
  if (!prefix) return;

  var file
    , dir
    , i
    , sdiff
    , sfile
    , list;

  if (Array.isArray(prefix)) {
    for (i = 0; i < prefix.length; i++) {
      file = this._tprefix(prefix[i], term, soft);
      if (file) return file;
    }
    return;
  }

  var find = function(word) {
    var file, ch;

    file = path.resolve(prefix, word[0]);
    try {
      fs.statSync(file);
      return file;
    } catch (e) {
      ;
    }

    ch = word[0].charCodeAt(0).toString(16);
    if (ch.length < 2) ch = '0' + ch;

    file = path.resolve(prefix, ch);
    try {
      fs.statSync(file);
      return file;
    } catch (e) {
      ;
    }
  };

  if (!term) {
    // Make sure the directory's sub-directories
    // are all one-letter, or hex digits.
    // return find('x') ? prefix : null;
    try {
      dir = fs.readdirSync(prefix).filter(function(file) {
        return file.length !== 1 && !/^[0-9a-fA-F]{2}$/.test(file);
      });
      if (!dir.length) {
        return prefix;
      }
    } catch (e) {
      ;
    }
    return;
  }

  term = path.basename(term);
  dir = find(term);

  if (!dir) return;

  if (soft) {
    try {
      list = fs.readdirSync(dir);
    } catch (e) {
      return;
    }

    list.forEach(function(file) {
      if (file.indexOf(term) === 0) {
        var diff = file.length - term.length;
        if (!sfile || diff < sdiff) {
          sdiff = diff;
          sfile = file;
        }
      }
    });

    return sfile && (soft || sdiff === 0)
      ? path.resolve(dir, sfile)
      : null;
  }

  file = path.resolve(dir, term);
  try {
    fs.statSync(file);
    return file;
  } catch (e) {
    ;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.print"></a>[function <span class="apidocSignatureSpan">blessed.Tput.</span>print ()](#apidoc.element.blessed.Tput.print)
- description and source-code
```javascript
print = function () {
  var fake = {
    padding: true,
    bools: { needs_xon_xoff: true, xon_xoff: false }
  };
  return Tput.prototype._print.apply(fake, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.sprintf"></a>[function <span class="apidocSignatureSpan">blessed.Tput.</span>sprintf (src)](#apidoc.element.blessed.Tput.sprintf)
- description and source-code
```javascript
function sprintf(src) {
  var params = Array.prototype.slice.call(arguments, 1)
    , rule = /%([\-+# ]{1,4})?(\d+(?:\.\d+)?)?([doxXsc])/g
    , i = 0;

  return src.replace(rule, function(_, flag, width, type) {
    var flags = (flag || '').split('')
      , param = params[i] != null ? params[i] : ''
      , initial = param
      // , width = +width
      , opt = {}
      , pre = '';

    i++;

    switch (type) {
      case 'd': // signed int
        param = (+param).toString(10);
        break;
      case 'o': // unsigned octal
        param = (+param).toString(8);
        break;
      case 'x': // unsigned hex int
        param = (+param).toString(16);
        break;
      case 'X': // unsigned hex int uppercase
        param = (+param).toString(16).toUppercase();
        break;
      case 's': // string
        break;
      case 'c': // char
        param = isFinite(param)
          ? String.fromCharCode(param || 0200)
          : '';
        break;
    }

    flags.forEach(function(flag) {
      switch (flag) {
        // left-justify by width
        case '-':
          opt.left = true;
          break;
        // always precede numbers with their signs
        case '+':
          opt.signs = true;
          break;
        // used with o, x, X - value is preceded with 0, 0x, or 0X respectively.
        // used with a, A, e, E, f, F, g, G - forces written output to contain
        // a decimal point even if no more digits follow
        case '#':
          opt.hexpoint = true;
          break;
        // if no sign is going to be written, black space in front of the value
        case ' ':
          opt.space = true;
          break;
      }
    });

    width = +width.split('.')[0];

    // Should this be for opt.left too?
    // Example: %2.2X - turns 0 into 00
    if (width && !opt.left) {
      param = param + '';
      while (param.length < width) {
        param = '0' + param;
      }
    }

    if (opt.signs) {
      if (+initial >= 0) {
        pre += '+';
      }
    }

    if (opt.space) {
      if (!opt.signs && +initial >= 0) {
        pre += ' ';
      }
    }

    if (opt.hexpoint) {
      switch (type) {
        case 'o': // unsigned octal
          pre += '0';
          break;
        case 'x': // unsigned hex int
          pre += '0x';
          break;
        case 'X': // unsigned hex int uppercase
          pre += '0X';
          break;
      }
    }

    if (opt.left) {
      if (width > (pre.length + param.length)) {
        width -= pre.length + param.length;
        pre = Array(width + 1).join(' ') + pre;
      }
    }

    return pre + param;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.tryRead"></a>[function <span class="apidocSignatureSpan">blessed.Tput.</span>tryRead (file)](#apidoc.element.blessed.Tput.tryRead)
- description and source-code
```javascript
function tryRead(file) {
  if (Array.isArray(file)) {
    for (var i = 0; i < file.length; i++) {
      var data = tryRead(file[i]);
      if (data) return data;
    }
    return '';
  }
  if (!file) return '';
  file = path.resolve.apply(path, arguments);
  try {
    return fs.readFileSync(file, 'utf8');
  } catch (e) {
    return '';
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.Tput.prototype"></a>[module blessed.Tput.prototype](#apidoc.module.blessed.Tput.prototype)

#### <a name="apidoc.element.blessed.Tput.prototype.GetConsoleCP"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>GetConsoleCP ()](#apidoc.element.blessed.Tput.prototype.GetConsoleCP)
- description and source-code
```javascript
GetConsoleCP = function () {
  var ccp;

  if (process.platform !== 'win32') {
    return -1;
  }

  // Allow unicode on all windows consoles for now:
  if (+process.env.NCURSES_UNICODE !== 0) {
    return 65001;
  }

  // cp.execSync('chcp 65001', { stdio: 'ignore', timeout: 1500 });

  try {
    // Produces something like: 'Active code page: 437\n\n'
    ccp = cp.execFileSync(process.env.WINDIR + '\\system32\\chcp.com', [], {
      stdio: ['ignore', 'pipe', 'ignore'],
      encoding: 'ascii',
      timeout: 1500
    });
    // ccp = cp.execSync('chcp', {
    //   stdio: ['ignore', 'pipe', 'ignore'],
    //   encoding: 'ascii',
    //   timeout: 1500
    // });
  } catch (e) {
    ;
  }

  ccp = /\d+/.exec(ccp);

  if (!ccp) {
    return -1;
  }

  ccp = +ccp[0];

  return ccp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._captoinfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_captoinfo (cap, s, parameterized)](#apidoc.element.blessed.Tput.prototype._captoinfo)
- description and source-code
```javascript
_captoinfo = function (cap, s, parameterized) {
  var self = this;

  var capstart;

  if (parameterized == null) {
    parameterized = 0;
  }

  var MAX_PUSHED = 16
    , stack = [];

  var stackptr = 0
    , onstack = 0
    , seenm = 0
    , seenn = 0
    , seenr = 0
    , param = 1
    , i = 0
    , out = '';

  function warn() {
    var args = Array.prototype.slice.call(arguments);
    args[0] = 'captoinfo: ' + (args[0] || '');
    return self._debug.apply(self, args);
  }

  function isdigit(ch) {
    return ch >= '0' && ch <= '9';
  }

  function isgraph(ch) {
    return ch > ' ' && ch <= '~';
  }

  // convert a character to a terminfo push
  function cvtchar(sp) {
    var c = '\0'
      , len;

    var j = i;

    switch (sp[j]) {
      case '\\':
        switch (sp[++j]) {
          case '\'':
          case '$':
          case '\\':
          case '%':
            c = sp[j];
            len = 2;
            break;
          case '\0':
            c = '\\';
            len = 1;
            break;
          case '0':
          case '1':
          case '2':
          case '3':
            len = 1;
            while (isdigit(sp[j])) {
              c = String.fromCharCode(8 * c.charCodeAt(0)
                + (sp[j++].charCodeAt(0) - '0'.charCodeAt(0)));
              len++;
            }
            break;
          default:
            c = sp[j];
            len = 2;
            break;
        }
        break;
      case '^':
        c = String.fromCharCode(sp[++j].charCodeAt(0) & 0x1f);
        len = 2;
        break;
      default:
        c = sp[j];
        len = 1;
    }
    if (isgraph(c) && c !== ',' && c !== '\'' && c !== '\\' && c !== ':') {
      out += '%\'';
      out += c;
      out += '\'';
    } else {
      out += '%{';
      if (c.charCodeAt(0) > 99) {
        out += String.fromCharCode(
          (c.charCodeAt(0) / 100 | 0) + '0'.charCodeAt(0));
      }
      if (c.charCodeAt(0) > 9) {
        out += String.fromCharCode(
          (c.charCodeAt(0) / 10 | 0) % 10 + '0'.charCodeAt(0));
      }
      out += String.fromCharCode(
        c.charCodeAt(0) % 10 + '0'.charCodeAt(0));
      out += '}';
    }

    return len;
  }

  // push n copies of param on the terminfo stack if not already there
  function getparm(parm, n) {
    if (seenr) {
      if (parm === 1) {
        parm = 2;
      } else if (parm === 2) {
        parm = 1;
      }
    }

    if (onstack === parm) {
      if (n > 1) {
        warn('string may not be optimal');
        out += '%Pa';
        while (n--) {
          out += '%ga';
        }
      }
      return;
    }

    if (onstack !== 0) {
      push();
    }

    onstack = parm;

    while (n--) {
      out += '%p';
      out += String.fromCharCode('0'.charCodeAt(0) + parm);
    }

    if (seenn && parm < 3) {
      out += '%{96}%^';
    }

    if (seenm && parm < 3) {
      out += '%{127}%^';
    }
  }

  // push onstack on to the stack
  function push() {
    if (stackptr >= MAX_PUSHED) {
      warn('string too complex to convert');
    } else {
      stack[stackptr++] = onstack;
    }
  }

  // pop the top of the stack into onstack
  function pop() {
    if (stackptr === 0) {
      if (onstack === 0) {
        warn('I\'m confused');
      } else {
        onstack = 0;
      }
    } else {
      onstack = stack[--stackptr];
    }
    param++;
  }

  function see03() {
    getparm(param, 1);
    out += '%3d';
    pop();
  }

  function invalid() {
    out += '%';
    i--;
    warn('unknown %% code %s (%#x) in %s',
      JSON.stringify(s[i]), s[i].charCodeAt(0), cap);
  }

  // skip the initial padding (if we haven't been told not to)
  capstart = null;
  if (s == null) s = '';

  if (parameterized >= 0 && isdigit(s[i])) {
    for (capstart = i;; i++) {
      if (!(isdigit(s[i]) || s[i] === '*' || s[i] === '.')) {
        break;
      }
    }
  }

  while (s[i]) {
    switch (s[i]) {
      case '%':
        i++;
        if (parameterized < 1) {
          out += '%';
          break;
        }
        switch (s[i++]) {
          case '%':
            out += '%';
            break; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._compile"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_compile (info, key, str)](#apidoc.element.blessed.Tput.prototype._compile)
- description and source-code
```javascript
_compile = function (info, key, str) {
  var v;

  this._debug('Compiling %s: %s', key, JSON.stringify(str));

  switch (typeof str) {
    case 'boolean':
      return str;
    case 'number':
      return str;
    case 'string':
      break;
    default:
      return noop;
  }

  if (!str) {
    return noop;
  }

  // See:
  // ~/ncurses/progs/tput.c - tput() - L149
  // ~/ncurses/progs/tset.c - set_init() - L992
  if (key === 'init_file' || key === 'reset_file') {
    try {
      str = fs.readFileSync(str, 'utf8');
      if (this.debug) {
        v = ('return ' + JSON.stringify(str) + ';')
          .replace(/\x1b/g, '\\x1b')
          .replace(/\r/g, '\\r')
          .replace(/\n/g, '\\n');
        process.stdout.write(v + '\n');
      }
      return function() { return str; };
    } catch (e) {
      return noop;
    }
  }

  var tkey = info.name + '.' + key
    , header = 'var v, dyn = {}, stat = {}, stack = [], out = [];'
    , footer = ';return out.join("");'
    , code = header
    , val = str
    , buff = ''
    , cap
    , ch
    , fi
    , then
    , els
    , end;

  function read(regex, no) {
    cap = regex.exec(val);
    if (!cap) return;
    val = val.substring(cap[0].length);
    ch = cap[1];
    if (!no) clear();
    return cap;
  }

  function stmt(c) {
    if (code[code.length - 1] === ',') {
      code = code.slice(0, -1);
    }
    code += c;
  }

  function expr(c) {
    code += c + ',';
  }

  function echo(c) {
    if (c === '""') return;
    expr('out.push(' + c + ')');
  }

  function print(c) {
    buff += c;
  }

  function clear() {
    if (buff) {
      echo(JSON.stringify(buff).replace(/\\u00([0-9a-fA-F]{2})/g, '\\x$1'));
      buff = '';
    }
  }

  while (val) {
    // Ignore newlines
    if (read(/^\n /, true)) {
      continue;
    }

    // '^A' -> ^A
    if (read(/^\^(.)/i, true)) {
      if (!(ch >= ' ' && ch <= '~')) {
        this._debug('%s: bad caret char.', tkey);
        // NOTE: ncurses appears to simply
        // continue in this situation, but
        // I could be wrong.
        print(cap[0]);
        continue;
      }
      if (ch === '?') {
        ch = '\x7f';
      } else {
        ch = ch.charCodeAt(0) & 31;
        if (ch === 0) ch = 128;
        ch = String.fromCharCode(ch);
      }
      print(ch);
      continue;
    }

    // 3 octal digits -> character
    if (read(/^\\([0-7]{3})/, true)) {
      print(String.fromCharCode(parseInt(ch, 8)));
      continue;
    }

    // '\e' -> ^[
    // '\n' -> \n
    // '\r' -> \r
    // '\0' -> \200 (special case)
    if (read(/^\\([eEnlrtbfs\^\\,:0]|.)/, true)) {
      switch (ch) {
        case 'e':
        case 'E':
          ch = '\x1b';
          break;
        case 'n':
          ch = '\n';
          break;
        case 'l':
          ch = '\x85';
          break;
        case 'r':
          ch = '\r';
          break;
        case 't':
          ch = '\t';
          break;
        case 'b':
          ch = '\x08';
          break;
        case 'f':
          ch = '\x0c';
          break;
        case 's':
          ch = ' ';
          break;
        case '^':
          ch = '^';
          break;
        case '\\':
          ch = '\\';
          break;
        case ',':
          ch = ',';
          break;
        case ':':
          ch = ':';
          break;
        case '0':
          ch = '\200';
          break;
        case 'a':
          ch = '\x07';
          break;
        default:
          this._debug('%s: bad backslash char.', tkey);
          ch = cap[0];
          break;
      }
      print(ch);
      continue;
    }

    // $<5> -> padding
    // e.g. flash_screen: '\u001b[?5h$<100/>\u001b[?5l',
    if (read(/^\$<(\d+)([*\/]{0,2})>/, true)) {
      if (this.padding) print(cap[0]);
      continue;
    }

    // %%   outputs '%'
    if (read(/^%%/, true)) {
      print('%');
      continue;
    }

    // %[[:]flags][width[.precision]][doxXs]
    //   as in printf, flags are [-+#] and space.  Use a ':' to allow the
    //   next character to be a '-' flag, avoiding interpreting "%-" as an
    //   operator.
    // %c ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._debug"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_debug ()](#apidoc.element.blessed.Tput.prototype._debug)
- description and source-code
```javascript
_debug = function () {
  if (!this.debug) return;
  return console.log.apply(console, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._prefix"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_prefix (term)](#apidoc.element.blessed.Tput.prototype._prefix)
- description and source-code
```javascript
_prefix = function (term) {
  // If we have a terminfoFile, or our
  // term looks like a filename, use it.
  if (term) {
    if (~term.indexOf(path.sep)) {
      return term;
    }
    if (this.terminfoFile) {
      return this.terminfoFile;
    }
  }

  var paths = Tput.ipaths.slice()
    , file;

  if (this.terminfoPrefix) {
    paths.unshift(this.terminfoPrefix);
  }

  // Try exact matches.
  file = this._tprefix(paths, term);
  if (file) return file;

  // Try similar matches.
  file = this._tprefix(paths, term, true);
  if (file) return file;

  // Not found.
  throw new Error('Terminfo directory not found.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._print"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_print (code, print, done)](#apidoc.element.blessed.Tput.prototype._print)
- description and source-code
```javascript
_print = function (code, print, done) {
  var xon = !this.bools.needs_xon_xoff || this.bools.xon_xoff;

  print = print || write;
  done = done || noop;

  if (!this.padding) {
    print(code);
    return done();
  }

  var parts = code.split(/(?=\$<[\d.]+[*\/]{0,2}>)/)
    , i = 0;

  (function next() {
    if (i === parts.length) {
      return done();
    }

    var part = parts[i++]
      , padding = /^\$<([\d.]+)([*\/]{0,2})>/.exec(part)
      , amount
      , suffix;
      // , affect;

    if (!padding) {
      print(part);
      return next();
    }

    part = part.substring(padding[0].length);
    amount = +padding[1];
    suffix = padding[2];

    // A '/'  suffix indicates  that  the  padding  is  mandatory and forces a
    // delay of the given number of milliseconds even on devices for which xon
    // is present to indicate flow control.
    if (xon && !~suffix.indexOf('/')) {
      print(part);
      return next();
    }

    // A '*' indicates that the padding required is proportional to the number
    // of lines affected by the operation, and  the amount  given  is the
    // per-affected-unit padding required.  (In the case of insert character,
    // the factor is still the number of lines affected.) Normally, padding is
    // advisory if the device has the xon capability; it is used for cost
    // computation but does not trigger delays.
    if (~suffix.indexOf('*')) {
      // XXX Disable this for now.
      amount = amount;
      // if (affect = /\x1b\[(\d+)[LM]/.exec(part)) {
      //   amount *= +affect[1];
      // }
      // The above is a huge workaround. In reality, we need to compile
      // '_print' into the string functions and check the cap name and
      // params.
      // if (cap === 'insert_line' || cap === 'delete_line') {
      //   amount *= params[0];
      // }
      // if (cap === 'clear_screen') {
      //   amount *= process.stdout.rows;
      // }
    }

    return setTimeout(function() {
      print(part);
      return next();
    }, amount);
  })();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._tprefix"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_tprefix (prefix, term, soft)](#apidoc.element.blessed.Tput.prototype._tprefix)
- description and source-code
```javascript
_tprefix = function (prefix, term, soft) {
  if (!prefix) return;

  var file
    , dir
    , i
    , sdiff
    , sfile
    , list;

  if (Array.isArray(prefix)) {
    for (i = 0; i < prefix.length; i++) {
      file = this._tprefix(prefix[i], term, soft);
      if (file) return file;
    }
    return;
  }

  var find = function(word) {
    var file, ch;

    file = path.resolve(prefix, word[0]);
    try {
      fs.statSync(file);
      return file;
    } catch (e) {
      ;
    }

    ch = word[0].charCodeAt(0).toString(16);
    if (ch.length < 2) ch = '0' + ch;

    file = path.resolve(prefix, ch);
    try {
      fs.statSync(file);
      return file;
    } catch (e) {
      ;
    }
  };

  if (!term) {
    // Make sure the directory's sub-directories
    // are all one-letter, or hex digits.
    // return find('x') ? prefix : null;
    try {
      dir = fs.readdirSync(prefix).filter(function(file) {
        return file.length !== 1 && !/^[0-9a-fA-F]{2}$/.test(file);
      });
      if (!dir.length) {
        return prefix;
      }
    } catch (e) {
      ;
    }
    return;
  }

  term = path.basename(term);
  dir = find(term);

  if (!dir) return;

  if (soft) {
    try {
      list = fs.readdirSync(dir);
    } catch (e) {
      return;
    }

    list.forEach(function(file) {
      if (file.indexOf(term) === 0) {
        var diff = file.length - term.length;
        if (!sfile || diff < sdiff) {
          sdiff = diff;
          sfile = file;
        }
      }
    });

    return sfile && (soft || sdiff === 0)
      ? path.resolve(dir, sfile)
      : null;
  }

  file = path.resolve(dir, term);
  try {
    fs.statSync(file);
    return file;
  } catch (e) {
    ;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._tryCap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_tryCap (file, term)](#apidoc.element.blessed.Tput.prototype._tryCap)
- description and source-code
```javascript
_tryCap = function (file, term) {
  if (!file) return;

  var terms
    , data
    , i;

  if (Array.isArray(file)) {
    for (i = 0; i < file.length; i++) {
      data = this._tryCap(file[i], term);
      if (data) return data;
    }
    return;
  }

  // If the termcap string starts with '/',
  // ncurses considers it a filename.
  data = file[0] === '/'
    ? tryRead(file)
    : file;

  if (!data) return;

  terms = this.parseTermcap(data, file);

  if (term && !terms[term]) {
    return;
  }

  return terms;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._useInternalCap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useInternalCap (name)](#apidoc.element.blessed.Tput.prototype._useInternalCap)
- description and source-code
```javascript
_useInternalCap = function (name) {
  name = path.basename(name);
  return this.injectTermcap(__dirname + '/../usr/' + name + '.termcap');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._useInternalInfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useInternalInfo (name)](#apidoc.element.blessed.Tput.prototype._useInternalInfo)
- description and source-code
```javascript
_useInternalInfo = function (name) {
  name = path.basename(name);
  return this.injectTerminfo(__dirname + '/../usr/' + name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._useVt102Cap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useVt102Cap ()](#apidoc.element.blessed.Tput.prototype._useVt102Cap)
- description and source-code
```javascript
_useVt102Cap = function () {
  return this.injectTermcap('vt102');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._useXtermCap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useXtermCap ()](#apidoc.element.blessed.Tput.prototype._useXtermCap)
- description and source-code
```javascript
_useXtermCap = function () {
  return this.injectTermcap(__dirname + '/../usr/xterm.termcap');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype._useXtermInfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>_useXtermInfo ()](#apidoc.element.blessed.Tput.prototype._useXtermInfo)
- description and source-code
```javascript
_useXtermInfo = function () {
  return this.injectTerminfo(__dirname + '/../usr/xterm');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.compile"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compile (info)](#apidoc.element.blessed.Tput.prototype.compile)
- description and source-code
```javascript
compile = function (info) {
  var self = this;

  if (!info) {
    throw new Error('Terminal not found.');
  }

  this.detectFeatures(info);

  this._debug(info);

  info.all = {};
  info.methods = {};

  ['bools', 'numbers', 'strings'].forEach(function(type) {
    Object.keys(info[type]).forEach(function(key) {
      info.all[key] = info[type][key];
      info.methods[key] = self._compile(info, key, info.all[key]);
    });
  });

  Tput.bools.forEach(function(key) {
    if (info.methods[key] == null) info.methods[key] = false;
  });

  Tput.numbers.forEach(function(key) {
    if (info.methods[key] == null) info.methods[key] = -1;
  });

  Tput.strings.forEach(function(key) {
    if (!info.methods[key]) info.methods[key] = noop;
  });

  Object.keys(info.methods).forEach(function(key) {
    if (!Tput.alias[key]) return;
    Tput.alias[key].forEach(function(alias) {
      info.methods[alias] = info.methods[key];
    });
    // Could just use:
    // Object.keys(Tput.aliasMap).forEach(function(key) {
    //   info.methods[key] = info.methods[Tput.aliasMap[key]];
    // });
  });

  return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.compileAll"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileAll (start)](#apidoc.element.blessed.Tput.prototype.compileAll)
- description and source-code
```javascript
compileAll = function (start) {
  var self = this
    , all = {};

  this.getAll().forEach(function(name) {
    if (start && name !== start) {
      return;
    } else {
      start = null;
    }
    all[name] = self.compileTerminfo(name);
  });

  return all;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.compileTermcap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileTermcap (term)](#apidoc.element.blessed.Tput.prototype.compileTermcap)
- description and source-code
```javascript
compileTermcap = function (term) {
  return this.compile(this.readTermcap(term));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.compileTerminfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>compileTerminfo (term)](#apidoc.element.blessed.Tput.prototype.compileTerminfo)
- description and source-code
```javascript
compileTerminfo = function (term) {
  return this.compile(this.readTerminfo(term));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectBrokenACS"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectBrokenACS (info)](#apidoc.element.blessed.Tput.prototype.detectBrokenACS)
- description and source-code
```javascript
detectBrokenACS = function (info) {
  // ncurses-compatible env variable.
  if (process.env.NCURSES_NO_UTF8_ACS != null) {
    return !!+process.env.NCURSES_NO_UTF8_ACS;
  }

  // If the terminal supports unicode, we don't need ACS.
  if (info.numbers.U8 >= 0) {
    return !!info.numbers.U8;
  }

  // The linux console is just broken for some reason.
  // Apparently the Linux console does not support ACS,
  // but it does support the PC ROM character set.
  if (info.name === 'linux') {
    return true;
  }

  // PC alternate charset
  // if (acsc.indexOf('+\x10,\x11-\x18.\x190') === 0) {
  if (this.detectPCRomSet(info)) {
    return true;
  }

  // screen termcap is bugged?
  if (this.termcap
      && info.name.indexOf('screen') === 0
      && process.env.TERMCAP
      && ~process.env.TERMCAP.indexOf('screen')
      && ~process.env.TERMCAP.indexOf('hhII00')) {
    if (~info.strings.enter_alt_charset_mode.indexOf('\016')
        || ~info.strings.enter_alt_charset_mode.indexOf('\017')
        || ~info.strings.set_attributes.indexOf('\016')
        || ~info.strings.set_attributes.indexOf('\017')) {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectFeatures"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectFeatures (info)](#apidoc.element.blessed.Tput.prototype.detectFeatures)
- description and source-code
```javascript
detectFeatures = function (info) {
  var data = this.parseACS(info);
  info.features = {
    unicode: this.detectUnicode(info),
    brokenACS: this.detectBrokenACS(info),
    PCRomSet: this.detectPCRomSet(info),
    magicCookie: this.detectMagicCookie(info),
    padding: this.detectPadding(info),
    setbuf: this.detectSetbuf(info),
    acsc: data.acsc,
    acscr: data.acscr
  };
  return info.features;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectMagicCookie"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectMagicCookie ()](#apidoc.element.blessed.Tput.prototype.detectMagicCookie)
- description and source-code
```javascript
detectMagicCookie = function () {
  return process.env.NCURSES_NO_MAGIC_COOKIE == null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectPCRomSet"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectPCRomSet (info)](#apidoc.element.blessed.Tput.prototype.detectPCRomSet)
- description and source-code
```javascript
detectPCRomSet = function (info) {
  var s = info.strings;
  if (s.enter_pc_charset_mode && s.enter_alt_charset_mode
      && s.enter_pc_charset_mode === s.enter_alt_charset_mode
      && s.exit_pc_charset_mode === s.exit_alt_charset_mode) {
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectPadding"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectPadding ()](#apidoc.element.blessed.Tput.prototype.detectPadding)
- description and source-code
```javascript
detectPadding = function () {
  return process.env.NCURSES_NO_PADDING == null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectSetbuf"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectSetbuf ()](#apidoc.element.blessed.Tput.prototype.detectSetbuf)
- description and source-code
```javascript
detectSetbuf = function () {
  return process.env.NCURSES_NO_SETBUF == null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.detectUnicode"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>detectUnicode ()](#apidoc.element.blessed.Tput.prototype.detectUnicode)
- description and source-code
```javascript
detectUnicode = function () {
  if (this.options.forceUnicode != null) {
    return this.options.forceUnicode;
  }

  var LANG = process.env.LANG
    + ':' + process.env.LANGUAGE
    + ':' + process.env.LC_ALL
    + ':' + process.env.LC_CTYPE;

  return /utf-?8/i.test(LANG) || (this.GetConsoleCP() === 65001);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.getAll"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>getAll ()](#apidoc.element.blessed.Tput.prototype.getAll)
- description and source-code
```javascript
getAll = function () {
  var dir = this._prefix()
    , list = asort(fs.readdirSync(dir))
    , infos = [];

  list.forEach(function(letter) {
    var terms = asort(fs.readdirSync(path.resolve(dir, letter)));
    infos.push.apply(infos, terms);
  });

  function asort(obj) {
    return obj.sort(function(a, b) {
      a = a.toLowerCase().charCodeAt(0);
      b = b.toLowerCase().charCodeAt(0);
      return a - b;
    });
  }

  return infos;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.has"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>has (name)](#apidoc.element.blessed.Tput.prototype.has)
- description and source-code
```javascript
has = function (name) {
  name = Tput.aliasMap[name];

  var val = this.all[name];

  if (!name) return false;

  if (typeof val === 'number') {
    return val !== -1;
  }

  return !!val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.inject"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>inject (info)](#apidoc.element.blessed.Tput.prototype.inject)
- description and source-code
```javascript
inject = function (info) {
  var self = this
    , methods = info.methods || info;

  Object.keys(methods).forEach(function(key) {
    if (typeof methods[key] !== 'function') {
      self[key] = methods[key];
      return;
    }
    self[key] = function() {
      var args = Array.prototype.slice.call(arguments);
      return methods[key].call(self, args);
    };
  });

  this.info = info;
  this.all = info.all;
  this.methods = info.methods;
  this.bools = info.bools;
  this.numbers = info.numbers;
  this.strings = info.strings;

  if (!~info.names.indexOf(this.terminal)) {
    this.terminal = info.name;
  }

  this.features = info.features;
  Object.keys(info.features).forEach(function(key) {
    if (key === 'padding') {
      if (!info.features.padding && self.options.padding !== true) {
        self.padding = false;
      }
      return;
    }
    self[key] = info.features[key];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.injectTermcap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>injectTermcap (term)](#apidoc.element.blessed.Tput.prototype.injectTermcap)
- description and source-code
```javascript
injectTermcap = function (term) {
  return this.inject(this.compileTermcap(term));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.injectTerminfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>injectTerminfo (term)](#apidoc.element.blessed.Tput.prototype.injectTerminfo)
- description and source-code
```javascript
injectTerminfo = function (term) {
  return this.inject(this.compileTerminfo(term));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.parseACS"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseACS (info)](#apidoc.element.blessed.Tput.prototype.parseACS)
- description and source-code
```javascript
parseACS = function (info) {
  var data = {};

  data.acsc = {};
  data.acscr = {};

  // Possibly just return an empty object, as done here, instead of
  // specifically saying ACS is "broken" above. This would be more
  // accurate to ncurses logic. But it doesn't really matter.
  if (this.detectPCRomSet(info)) {
    return data;
  }

  // See: ~/ncurses/ncurses/tinfo/lib_acs.c: L208
  Object.keys(Tput.acsc).forEach(function(ch) {
    var acs_chars = info.strings.acs_chars || ''
      , i = acs_chars.indexOf(ch)
      , next = acs_chars[i + 1];

    if (!next || i === -1 || !Tput.acsc[next]) {
      return;
    }

    data.acsc[ch] = Tput.acsc[next];
    data.acscr[Tput.acsc[next]] = ch;
  });

  return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.parseExtended"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseExtended (data)](#apidoc.element.blessed.Tput.prototype.parseExtended)
- description and source-code
```javascript
parseExtended = function (data) {
  var info = {}
    , l = data.length
    , i = 0;

  var h = info.header = {
    dataSize: data.length,
    headerSize: 10,
    boolCount: (data[i + 1] << 8) | data[i + 0],
    numCount: (data[i + 3] << 8) | data[i + 2],
    strCount: (data[i + 5] << 8) | data[i + 4],
    strTableSize: (data[i + 7] << 8) | data[i + 6],
    lastStrTableOffset: (data[i + 9] << 8) | data[i + 8]
  };

  // h.symOffsetCount = h.strTableSize - h.strCount;

  h.total = h.headerSize
    + h.boolCount
    + h.numCount * 2
    + h.strCount * 2
    + h.strTableSize;

  i += h.headerSize;

  // Booleans Section
  // One byte for each flag
  var _bools = [];
  l = i + h.boolCount;
  for (; i < l; i++) {
    _bools.push(data[i] === 1);
  }

  // Null byte in between to make sure numbers begin on an even byte.
  if (i % 2) {
    assert.equal(data[i], 0);
    i++;
  }

  // Numbers Section
  var _numbers = [];
  l = i + h.numCount * 2;
  for (; i < l; i += 2) {
    if (data[i + 1] === 0377 && data[i] === 0377) {
      _numbers.push(-1);
    } else {
      _numbers.push((data[i + 1] << 8) | data[i]);
    }
  }

  // Strings Section
  var _strings = [];
  l = i + h.strCount * 2;
  for (; i < l; i += 2) {
    if (data[i + 1] === 0377 && data[i] === 0377) {
      _strings.push(-1);
    } else {
      _strings.push((data[i + 1] << 8) | data[i]);
    }
  }

  // Pass over the sym offsets and get to the string table.
  i = data.length - h.lastStrTableOffset;
  // Might be better to do this instead if the file has trailing bytes:
  // i += h.symOffsetCount * 2;

  // String Table
  var high = 0;
  _strings.forEach(function(offset, k) {
    if (offset === -1) {
      _strings[k] = '';
      return;
    }

    var s = i + offset
      , j = s;

    while (data[j]) j++;

    assert(j < data.length);

    // Find out where the string table ends by
    // getting the highest string length.
    if (high < j - i) {
      high = j - i;
    }

    _strings[k] = data.toString('ascii', s, j);
  });

  // Symbol Table
  // Add one to the highest string length because we didn't count \0.
  i += high + 1;
  l = data.length;

  var sym = []
    , j;

  for (; i < l; i++) {
    j = i;
    while (data[j]) j++;
    sym.push(data.toString('ascii', i, j));
    i = j;
  }

  // Identify by name
  j = 0;

  info.bools = {};
  _bools.forEach(function(bool) {
    info.bools[sym[j++]] = bool;
  });

  info.numbers = {};
  _numbers.forEach(function(number) {
    info.numbers[sym[j++]] = number;
  });

  info.strings = {};
  _strings.forEach(function(string) {
    info.strings[sym[j++]] = string;
  });

  // Should be the very last bit of data.
  assert.equal(i, data.length);

  return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.parseTermcap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseTermcap (data, file)](#apidoc.element.blessed.Tput.prototype.parseTermcap)
- description and source-code
```javascript
parseTermcap = function (data, file) {
  var terms = {}
    , parts
    , term
    , entries
    , fields
    , field
    , names
    , i
    , j
    , k;

  // remove escaped newlines
  data = data.replace(/\\\n[ \t]*/g, '');

  // remove comments
  data = data.replace(/^#[^\n]+/gm, '');

  // split entries
  entries = data.trim().split(/\n+/);

  for (i = 0; i < entries.length; i++) {
    fields = entries[i].split(/:+/);
    for (j = 0; j < fields.length; j++) {
      field = fields[j].trim();
      if (!field) continue;

      if (j === 0) {
        names = field.split('|');
        term = {
          name: names[0],
          names: names,
          desc: names.pop(),
          file: ~file.indexOf(path.sep)
            ? path.resolve(file)
            : file,
          termcap: true
        };

        for (k = 0; k < names.length; k++) {
          terms[names[k]] = term;
        }

        term.bools = {};
        term.numbers = {};
        term.strings = {};

        continue;
      }

      if (~field.indexOf('=')) {
        parts = field.split('=');
        term.strings[parts[0]] = parts.slice(1).join('=');
      } else if (~field.indexOf('#')) {
        parts = field.split('#');
        term.numbers[parts[0]] = +parts.slice(1).join('#');
      } else {
        term.bools[field] = true;
      }
    }
  }

  return terms;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.parseTerminfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>parseTerminfo (data, file)](#apidoc.element.blessed.Tput.prototype.parseTerminfo)
- description and source-code
```javascript
parseTerminfo = function (data, file) {
  var info = {}
    , extended
    , l = data.length
    , i = 0
    , v
    , o;

  var h = info.header = {
    dataSize: data.length,
    headerSize: 12,
    magicNumber: (data[1] << 8) | data[0],
    namesSize: (data[3] << 8) | data[2],
    boolCount: (data[5] << 8) | data[4],
    numCount: (data[7] << 8) | data[6],
    strCount: (data[9] << 8) | data[8],
    strTableSize: (data[11] << 8) | data[10]
  };

  h.total = h.headerSize
    + h.namesSize
    + h.boolCount
    + h.numCount * 2
    + h.strCount * 2
    + h.strTableSize;

  i += h.headerSize;

  // Names Section
  var names = data.toString('ascii', i, i + h.namesSize - 1)
    , parts = names.split('|')
    , name = parts[0]
    , desc = parts.pop();

  info.name = name;
  info.names = parts;
  info.desc = desc;

  info.dir = path.resolve(file, '..', '..');
  info.file = file;

  i += h.namesSize - 1;

  // Names is nul-terminated.
  assert.equal(data[i], 0);
  i++;

  // Booleans Section
  // One byte for each flag
  // Same order as <term.h>
  info.bools = {};
  l = i + h.boolCount;
  o = 0;
  for (; i < l; i++) {
    v = Tput.bools[o++];
    info.bools[v] = data[i] === 1;
  }

  // Null byte in between to make sure numbers begin on an even byte.
  if (i % 2) {
    assert.equal(data[i], 0);
    i++;
  }

  // Numbers Section
  info.numbers = {};
  l = i + h.numCount * 2;
  o = 0;
  for (; i < l; i += 2) {
    v = Tput.numbers[o++];
    if (data[i + 1] === 0377 && data[i] === 0377) {
      info.numbers[v] = -1;
    } else {
      info.numbers[v] = (data[i + 1] << 8) | data[i];
    }
  }

  // Strings Section
  info.strings = {};
  l = i + h.strCount * 2;
  o = 0;
  for (; i < l; i += 2) {
    v = Tput.strings[o++];
    if (data[i + 1] === 0377 && data[i] === 0377) {
      info.strings[v] = -1;
    } else {
      info.strings[v] = (data[i + 1] << 8) | data[i];
    }
  }

  // String Table
  Object.keys(info.strings).forEach(function(key) {
    if (info.strings[key] === -1) {
      delete info.strings[key];
      return;
    }

    // Workaround: fix an odd bug in the screen-256color terminfo where it tries
    // to set -1, but it appears to have {0xfe, 0xff} instead of {0xff, 0xff}.
    // TODO: Possibly handle errors gracefully below, as well as in the
    // extended info. Also possibly do: 'if (info.strings[key] >= data.length)'.
    if (info.strings[key] === 65534) {
      delete info.strings[key];
      return;
    }

    var s = i + info.strings[key]
      , j = s;

    while (data[j]) j++;

    assert(j < data.length);

    info.strings[key] = data.toString('ascii', s, j);
  });

  // Extended Header
  if (this.extended !== false) {
    i--;
    i += h.strTableSize;
    if (i % 2) {
      assert.equal(data[i], 0);
      i++;
    }
    l = data.length;
    if (i < l - 1) {
      try {
        extended = this.parseExtended(data.slice(i));
      } catch (e) {
        if (this.debug) {
          throw e;
        }
        return info;
      }
      info.header.extended = extended.header;
      ['bools', 'numbers', 'strings'].forEach(function(key) {
        merge(info[key], extended[key]);
      });
    }
  }

  return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.readTermcap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>readTermcap (term)](#apidoc.element.blessed.Tput.prototype.readTermcap)
- description and source-code
```javascript
readTermcap = function (term) {
  var self = this
    , terms
    , term_
    , root
    , paths;

  term = term || this.terminal;

  // Termcap has a bunch of terminals usually stored in one file/string,
  // so we need to find the one containing our desired terminal.
  if (~term.indexOf(path.sep) && (terms = this._tryCap(path.resolve(term)))) {
    term_ = path.basename(term).split('.')[0];
    if (terms[process.env.TERM]) {
      term = process.env.TERM;
    } else if (terms[term_]) {
      term = term_;
    } else {
      term = Object.keys(terms)[0];
    }
  } else {
    paths = Tput.cpaths.slice();

    if (this.termcapFile) {
      paths.unshift(this.termcapFile);
    }

    paths.push(Tput.termcap);

    terms = this._tryCap(paths, term);
  }

  if (!terms) {
    throw new Error('Cannot find termcap for: ' + term);
  }

  root = terms[term];

  if (this.debug) {
    this._termcap = terms;
  }

  (function tc(term) {
    if (term && term.strings.tc) {
      root.inherits = root.inherits || [];
      root.inherits.push(term.strings.tc);

      var names = terms[term.strings.tc]
        ? terms[term.strings.tc].names
        : [term.strings.tc];

      self._debug('%s inherits from %s.',
        term.names.join('/'), names.join('/'));

      var inherit = tc(terms[term.strings.tc]);
      if (inherit) {
        ['bools', 'numbers', 'strings'].forEach(function(type) {
          merge(term[type], inherit[type]);
        });
      }
    }
    return term;
  })(root);

  // Translate termcap names to terminfo-style names.
  root = this.translateTermcap(root);

  return root;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.readTerminfo"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>readTerminfo (term)](#apidoc.element.blessed.Tput.prototype.readTerminfo)
- description and source-code
```javascript
readTerminfo = function (term) {
  var data
    , file
    , info;

  term = term || this.terminal;

  file = path.normalize(this._prefix(term));
  data = fs.readFileSync(file);
  info = this.parseTerminfo(data, file);

  if (this.debug) {
    this._terminfo = info;
  }

  return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.setup"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>setup ()](#apidoc.element.blessed.Tput.prototype.setup)
- description and source-code
```javascript
setup = function () {
  this.error = null;
  try {
    if (this.termcap) {
      try {
        this.injectTermcap();
      } catch (e) {
        if (this.debug) throw e;
        this.error = new Error('Termcap parse error.');
        this._useInternalCap(this.terminal);
      }
    } else {
      try {
        this.injectTerminfo();
      } catch (e) {
        if (this.debug) throw e;
        this.error = new Error('Terminfo parse error.');
        this._useInternalInfo(this.terminal);
      }
    }
  } catch (e) {
    // If there was an error, fallback
    // to an internally stored terminfo/cap.
    if (this.debug) throw e;
    this.error = new Error('Terminfo not found.');
    this._useXtermInfo();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.term"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>term (is)](#apidoc.element.blessed.Tput.prototype.term)
- description and source-code
```javascript
term = function (is) {
  return this.terminal.indexOf(is) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.Tput.prototype.translateTermcap"></a>[function <span class="apidocSignatureSpan">blessed.Tput.prototype.</span>translateTermcap (info)](#apidoc.element.blessed.Tput.prototype.translateTermcap)
- description and source-code
```javascript
translateTermcap = function (info) {
  var self = this
    , out = {};

  if (!info) return;

  this._debug(info);

  ['name', 'names', 'desc', 'file', 'termcap'].forEach(function(key) {
    out[key] = info[key];
  });

  // Separate aliases for termcap
  var map = (function() {
    var out = {};

    Object.keys(Tput.alias).forEach(function(key) {
      var aliases = Tput.alias[key];
      out[aliases.termcap] = key;
    });

    return out;
  })();

  // Translate termcap cap names to terminfo cap names.
  // e.g. 'up' -> 'cursor_up'
  ['bools', 'numbers', 'strings'].forEach(function(key) {
    out[key] = {};
    Object.keys(info[key]).forEach(function(cap) {
      if (key === 'strings') {
        info.strings[cap] = self._captoinfo(cap, info.strings[cap], 1);
      }
      if (map[cap]) {
        out[key][map[cap]] = info[key][cap];
      } else {
        // NOTE: Possibly include all termcap names
        // in a separate alias.js file. Some are
        // missing from the terminfo alias.js file
        // which is why we have to do this:
        // See: $ man termcap
        out[key][cap] = info[key][cap];
      }
    });
  });

  return out;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.ansiimage"></a>[module blessed.ansiimage](#apidoc.module.blessed.ansiimage)

#### <a name="apidoc.element.blessed.ansiimage.ansiimage"></a>[function <span class="apidocSignatureSpan">blessed.</span>ansiimage (options)](#apidoc.element.blessed.ansiimage.ansiimage)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage.curl"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.</span>curl (url)](#apidoc.element.blessed.ansiimage.curl)
- description and source-code
```javascript
curl = function (url) {
  try {
    return cp.execFileSync('curl',
      ['-s', '-A', '', url],
      { stdio: ['ignore', 'pipe', 'ignore'] });
  } catch (e) {
    ;
  }
  try {
    return cp.execFileSync('wget',
      ['-U', '', '-O', '-', url],
      { stdio: ['ignore', 'pipe', 'ignore'] });
  } catch (e) {
    ;
  }
  throw new Error('curl or wget failed.');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.ansiimage.prototype"></a>[module blessed.ansiimage.prototype](#apidoc.module.blessed.ansiimage.prototype)

#### <a name="apidoc.element.blessed.ansiimage.prototype.clearImage"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>clearImage ()](#apidoc.element.blessed.ansiimage.prototype.clearImage)
- description and source-code
```javascript
clearImage = function () {
  this.stop();
  this.setContent('');
  this.img = null;
  this.cellmap = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage.prototype.pause"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>pause ()](#apidoc.element.blessed.ansiimage.prototype.pause)
- description and source-code
```javascript
pause = function () {
  if (!this.img) return;
  return this.img.pause();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage.prototype.play"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>play ()](#apidoc.element.blessed.ansiimage.prototype.play)
- description and source-code
```javascript
play = function () {
  var self = this;
  if (!this.img) return;
  return this.img.play(function(bmp, cellmap) {
    self.cellmap = cellmap;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>render ()](#apidoc.element.blessed.ansiimage.prototype.render)
- description and source-code
```javascript
render = function () {
  var coords = this._render();
  if (!coords) return;

  if (this.img && this.cellmap) {
    this.img.renderElement(this.cellmap, this);
  }

  return coords;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.ansiimage.prototype.setImage"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>setImage (file)](#apidoc.element.blessed.ansiimage.prototype.setImage)
- description and source-code
```javascript
setImage = function (file) {
  this.file = typeof file === 'string' ? file : null;

  if (/^https?:/.test(file)) {
    file = ANSIImage.curl(file);
  }

  var width = this.position.width;
  var height = this.position.height;

  if (width != null) {
    width = this.width;
  }

  if (height != null) {
    height = this.height;
  }

  try {
    this.setContent('');

    this.img = tng(file, {
      colors: colors,
      width: width,
      height: height,
      scale: this.scale,
      ascii: this.options.ascii,
      speed: this.options.speed,
      filename: this.file
    });

    if (width == null || height == null) {
      this.width = this.img.cellmap[0].length;
      this.height = this.img.cellmap.length;
    }

    if (this.img.frames && this.options.animate) {
      this.play();
    } else {
      this.cellmap = this.img.cellmap;
    }
  } catch (e) {
    this.setContent('Image Error: ' + e.message);
    this.img = null;
    this.cellmap = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.ansiimage.prototype.stop"></a>[function <span class="apidocSignatureSpan">blessed.ansiimage.prototype.</span>stop ()](#apidoc.element.blessed.ansiimage.prototype.stop)
- description and source-code
```javascript
stop = function () {
  if (!this.img) return;
  return this.img.stop();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.bigtext"></a>[module blessed.bigtext](#apidoc.module.blessed.bigtext)

#### <a name="apidoc.element.blessed.bigtext.bigtext"></a>[function <span class="apidocSignatureSpan">blessed.</span>bigtext (options)](#apidoc.element.blessed.bigtext.bigtext)
- description and source-code
```javascript
function BigText(options) {
  if (!(this instanceof Node)) {
    return new BigText(options);
  }
  options = options || {};
  options.font = options.font
    || __dirname + '/../../usr/fonts/ter-u14n.json';
  options.fontBold = options.font
    || __dirname + '/../../usr/fonts/ter-u14b.json';
  this.fch = options.fch;
  this.ratio = {};
  this.font = this.loadFont(options.font);
  this.fontBold = this.loadFont(options.font);
  Box.call(this, options);
  if (this.style.bold) {
    this.font = this.fontBold;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.bigtext.prototype"></a>[module blessed.bigtext.prototype](#apidoc.module.blessed.bigtext.prototype)

#### <a name="apidoc.element.blessed.bigtext.prototype.loadFont"></a>[function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>loadFont (filename)](#apidoc.element.blessed.bigtext.prototype.loadFont)
- description and source-code
```javascript
loadFont = function (filename) {
  var self = this
    , data
    , font;

  data = JSON.parse(fs.readFileSync(filename, 'utf8'));

  this.ratio.width = data.width;
  this.ratio.height = data.height;

  function convertLetter(ch, lines) {
    var line, i;

    while (lines.length > self.ratio.height) {
      lines.shift();
      lines.pop();
    }

    lines = lines.map(function(line) {
      var chs = line.split('');
      chs = chs.map(function(ch) {
        return ch === ' ' ? 0 : 1;
      });
      while (chs.length < self.ratio.width) {
        chs.push(0);
      }
      return chs;
    });

    while (lines.length < self.ratio.height) {
      line = [];
      for (i = 0; i < self.ratio.width; i++) {
        line.push(0);
      }
      lines.push(line);
    }

    return lines;
  }

  font = Object.keys(data.glyphs).reduce(function(out, ch) {
    var lines = data.glyphs[ch].map;
    out[ch] = convertLetter(ch, lines);
    return out;
  }, {});

  delete font[' '];

  return font;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.bigtext.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>render ()](#apidoc.element.blessed.bigtext.prototype.render)
- description and source-code
```javascript
render = function () {
  if (this.position.width == null || this._shrinkWidth) {
    // if (this.width - this.iwidth < this.ratio.width * this.text.length + 1) {
      this.position.width = this.ratio.width * this.text.length + 1;
      this._shrinkWidth = true;
    // }
  }
  if (this.position.height == null || this._shrinkHeight) {
    // if (this.height - this.iheight < this.ratio.height + 0) {
      this.position.height = this.ratio.height + 0;
      this._shrinkHeight = true;
    // }
  }

  var coords = this._render();
  if (!coords) return;

  var lines = this.screen.lines
    , left = coords.xi + this.ileft
    , top = coords.yi + this.itop
    , right = coords.xl - this.iright
    , bottom = coords.yl - this.ibottom;

  var dattr = this.sattr(this.style)
    , bg = dattr & 0x1ff
    , fg = (dattr >> 9) & 0x1ff
    , flags = (dattr >> 18) & 0x1ff
    , attr = (flags << 18) | (bg << 9) | fg;

  for (var x = left, i = 0; x < right; x += this.ratio.width, i++) {
    var ch = this.text[i];
    if (!ch) break;
    var map = this.font[ch];
    if (!map) continue;
    for (var y = top; y < Math.min(bottom, top + this.ratio.height); y++) {
      if (!lines[y]) continue;
      var mline = map[y - top];
      if (!mline) continue;
      for (var mx = 0; mx < this.ratio.width; mx++) {
        var mcell = mline[mx];
        if (mcell == null) break;
        if (this.fch && this.fch !== ' ') {
          lines[y][x + mx][0] = dattr;
          lines[y][x + mx][1] = mcell === 1 ? this.fch : this.ch;
        } else {
          lines[y][x + mx][0] = mcell === 1 ? attr : dattr;
          lines[y][x + mx][1] = mcell === 1 ? ' ' : this.ch;
        }
      }
      lines[y].dirty = true;
    }
  }

  return coords;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.bigtext.prototype.setContent"></a>[function <span class="apidocSignatureSpan">blessed.bigtext.prototype.</span>setContent (content)](#apidoc.element.blessed.bigtext.prototype.setContent)
- description and source-code
```javascript
setContent = function (content) {
  this.content = '';
  this.text = content || '';
}
```
- example usage
```shell
...
height: 'shrink',
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
...
```



# <a name="apidoc.module.blessed.button"></a>[module blessed.button](#apidoc.module.blessed.button)

#### <a name="apidoc.element.blessed.button.button"></a>[function <span class="apidocSignatureSpan">blessed.</span>button (options)](#apidoc.element.blessed.button.button)
- description and source-code
```javascript
function Button(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Button(options);
  }

  options = options || {};

  if (options.autoFocus == null) {
    options.autoFocus = false;
  }

  Input.call(this, options);

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      return self.press();
    }
  });

  if (this.options.mouse) {
    this.on('click', function() {
      return self.press();
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.button.prototype"></a>[module blessed.button.prototype](#apidoc.module.blessed.button.prototype)

#### <a name="apidoc.element.blessed.button.prototype.press"></a>[function <span class="apidocSignatureSpan">blessed.button.prototype.</span>press ()](#apidoc.element.blessed.button.prototype.press)
- description and source-code
```javascript
press = function () {
  this.focus();
  this.value = true;
  var result = this.emit('press');
  delete this.value;
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.checkbox"></a>[module blessed.checkbox](#apidoc.module.blessed.checkbox)

#### <a name="apidoc.element.blessed.checkbox.checkbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>checkbox (options)](#apidoc.element.blessed.checkbox.checkbox)
- description and source-code
```javascript
function Checkbox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Checkbox(options);
  }

  options = options || {};

  Input.call(this, options);

  this.text = options.content || options.text || '';
  this.checked = this.value = options.checked || false;

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      self.toggle();
      self.screen.render();
    }
  });

  if (options.mouse) {
    this.on('click', function() {
      self.toggle();
      self.screen.render();
    });
  }

  this.on('focus', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    self.screen.program.lsaveCursor('checkbox');
    self.screen.program.cup(lpos.yi, lpos.xi + 1);
    self.screen.program.showCursor();
  });

  this.on('blur', function() {
    self.screen.program.lrestoreCursor('checkbox', true);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.checkbox.prototype"></a>[module blessed.checkbox.prototype](#apidoc.module.blessed.checkbox.prototype)

#### <a name="apidoc.element.blessed.checkbox.prototype.check"></a>[function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>check ()](#apidoc.element.blessed.checkbox.prototype.check)
- description and source-code
```javascript
check = function () {
  if (this.checked) return;
  this.checked = this.value = true;
  this.emit('check');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.checkbox.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>render ()](#apidoc.element.blessed.checkbox.prototype.render)
- description and source-code
```javascript
render = function () {
  this.clearPos(true);
  this.setContent('[' + (this.checked ? 'x' : ' ') + '] ' + this.text, true);
  return this._render();
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.checkbox.prototype.toggle"></a>[function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>toggle ()](#apidoc.element.blessed.checkbox.prototype.toggle)
- description and source-code
```javascript
toggle = function () {
  return this.checked
    ? this.uncheck()
    : this.check();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.checkbox.prototype.uncheck"></a>[function <span class="apidocSignatureSpan">blessed.checkbox.prototype.</span>uncheck ()](#apidoc.element.blessed.checkbox.prototype.uncheck)
- description and source-code
```javascript
uncheck = function () {
  if (!this.checked) return;
  this.checked = this.value = false;
  this.emit('uncheck');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.colors"></a>[module blessed.colors](#apidoc.module.blessed.colors)

#### <a name="apidoc.element.blessed.colors.RGBToHex"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>RGBToHex (r, g, b)](#apidoc.element.blessed.colors.RGBToHex)
- description and source-code
```javascript
RGBToHex = function (r, g, b) {
  if (Array.isArray(r)) {
    b = r[2], g = r[1], r = r[0];
  }

  function hex(n) {
    n = n.toString(16);
    if (n.length < 2) n = '0' + n;
    return n;
  }

  return '#' + hex(r) + hex(g) + hex(b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.blend"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>blend (attr, attr2, alpha)](#apidoc.element.blessed.colors.blend)
- description and source-code
```javascript
function blend(attr, attr2, alpha) {
  var name, i, c, nc;

  var bg = attr & 0x1ff;
  if (attr2 != null) {
    var bg2 = attr2 & 0x1ff;
    if (bg === 0x1ff) bg = 0;
    if (bg2 === 0x1ff) bg2 = 0;
    bg = exports.mixColors(bg, bg2, alpha);
  } else {
    if (blend._cache[bg] != null) {
      bg = blend._cache[bg];
    // } else if (bg < 8) {
    //   bg += 8;
    } else if (bg >= 8 && bg <= 15) {
      bg -= 8;
    } else {
      name = exports.ncolors[bg];
      if (name) {
        for (i = 0; i < exports.ncolors.length; i++) {
          if (name === exports.ncolors[i] && i !== bg) {
            c = exports.vcolors[bg];
            nc = exports.vcolors[i];
            if (nc[0] + nc[1] + nc[2] < c[0] + c[1] + c[2]) {
              blend._cache[bg] = i;
              bg = i;
              break;
            }
          }
        }
      }
    }
  }

  attr &= ~0x1ff;
  attr |= bg;

  var fg = (attr >> 9) & 0x1ff;
  if (attr2 != null) {
    var fg2 = (attr2 >> 9) & 0x1ff;
    // 0, 7, 188, 231, 251
    if (fg === 0x1ff) {
      // XXX workaround
      fg = 248;
    } else {
      if (fg === 0x1ff) fg = 7;
      if (fg2 === 0x1ff) fg2 = 7;
      fg = exports.mixColors(fg, fg2, alpha);
    }
  } else {
    if (blend._cache[fg] != null) {
      fg = blend._cache[fg];
    // } else if (fg < 8) {
    //   fg += 8;
    } else if (fg >= 8 && fg <= 15) {
      fg -= 8;
    } else {
      name = exports.ncolors[fg];
      if (name) {
        for (i = 0; i < exports.ncolors.length; i++) {
          if (name === exports.ncolors[i] && i !== fg) {
            c = exports.vcolors[fg];
            nc = exports.vcolors[i];
            if (nc[0] + nc[1] + nc[2] < c[0] + c[1] + c[2]) {
              blend._cache[fg] = i;
              fg = i;
              break;
            }
          }
        }
      }
    }
  }

  attr &= ~(0x1ff << 9);
  attr |= fg << 9;

  return attr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.convert"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>convert (color)](#apidoc.element.blessed.colors.convert)
- description and source-code
```javascript
convert = function (color) {
  if (typeof color === 'number') {
    ;
  } else if (typeof color === 'string') {
    color = color.replace(/[\- ]/g, '');
    if (colorNames[color] != null) {
      color = colorNames[color];
    } else {
      color = exports.match(color);
    }
  } else if (Array.isArray(color)) {
    color = exports.match(color);
  } else {
    color = -1;
  }
  return color !== -1 ? color : 0x1ff;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.hexToRGB"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>hexToRGB (hex)](#apidoc.element.blessed.colors.hexToRGB)
- description and source-code
```javascript
hexToRGB = function (hex) {
  if (hex.length === 4) {
    hex = hex[0]
      + hex[1] + hex[1]
      + hex[2] + hex[2]
      + hex[3] + hex[3];
  }

  var col = parseInt(hex.substring(1), 16)
    , r = (col >> 16) & 0xff
    , g = (col >> 8) & 0xff
    , b = col & 0xff;

  return [r, g, b];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.match"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>match (r1, g1, b1)](#apidoc.element.blessed.colors.match)
- description and source-code
```javascript
match = function (r1, g1, b1) {
  if (typeof r1 === 'string') {
    var hex = r1;
    if (hex[0] !== '#') {
      return -1;
    }
    hex = exports.hexToRGB(hex);
    r1 = hex[0], g1 = hex[1], b1 = hex[2];
  } else if (Array.isArray(r1)) {
    b1 = r1[2], g1 = r1[1], r1 = r1[0];
  }

  var hash = (r1 << 16) | (g1 << 8) | b1;

  if (exports._cache[hash] != null) {
    return exports._cache[hash];
  }

  var ldiff = Infinity
    , li = -1
    , i = 0
    , c
    , r2
    , g2
    , b2
    , diff;

  for (; i < exports.vcolors.length; i++) {
    c = exports.vcolors[i];
    r2 = c[0];
    g2 = c[1];
    b2 = c[2];

    diff = colorDistance(r1, g1, b1, r2, g2, b2);

    if (diff === 0) {
      li = i;
      break;
    }

    if (diff < ldiff) {
      ldiff = diff;
      li = i;
    }
  }

  return exports._cache[hash] = li;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.mixColors"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>mixColors (c1, c2, alpha)](#apidoc.element.blessed.colors.mixColors)
- description and source-code
```javascript
mixColors = function (c1, c2, alpha) {
  // if (c1 === 0x1ff) return c1;
  // if (c2 === 0x1ff) return c1;
  if (c1 === 0x1ff) c1 = 0;
  if (c2 === 0x1ff) c2 = 0;
  if (alpha == null) alpha = 0.5;

  c1 = exports.vcolors[c1];
  var r1 = c1[0];
  var g1 = c1[1];
  var b1 = c1[2];

  c2 = exports.vcolors[c2];
  var r2 = c2[0];
  var g2 = c2[1];
  var b2 = c2[2];

  r1 += (r2 - r1) * alpha | 0;
  g1 += (g2 - g1) * alpha | 0;
  b1 += (b2 - b1) * alpha | 0;

  return exports.match([r1, g1, b1]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.colors.reduce"></a>[function <span class="apidocSignatureSpan">blessed.colors.</span>reduce (color, total)](#apidoc.element.blessed.colors.reduce)
- description and source-code
```javascript
reduce = function (color, total) {
  if (color >= 16 && total <= 16) {
    color = exports.ccolors[color];
  } else if (color >= 8 && total <= 8) {
    color -= 8;
  } else if (color >= 2 && total <= 2) {
    color %= 2;
  }
  return color;
}
```
- example usage
```shell
...
// row).
if (el.position.left + el.width <= width) {
  el.position.top = rowOffset;
} else {
  // Otherwise we need to start a new row and calculate a new
  // 'rowOffset' and 'rowIndex' (the index of the child on the current
  // row).
  rowOffset += self.children.slice(rowIndex, i).reduce(function(out, el) {
    if (!self.isRendered(el)) return out;
    out = Math.max(out, el.lpos.yl - el.lpos.yi);
    return out;
  }, 0);
  rowIndex = i;
  el.position.left = 0;
  el.position.top = rowOffset;
...
```



# <a name="apidoc.module.blessed.filemanager"></a>[module blessed.filemanager](#apidoc.module.blessed.filemanager)

#### <a name="apidoc.element.blessed.filemanager.filemanager"></a>[function <span class="apidocSignatureSpan">blessed.</span>filemanager (options)](#apidoc.element.blessed.filemanager.filemanager)
- description and source-code
```javascript
function FileManager(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new FileManager(options);
  }

  options = options || {};
  options.parseTags = true;
  // options.label = ' {blue-fg}%path{/blue-fg} ';

  List.call(this, options);

  this.cwd = options.cwd || process.cwd();
  this.file = this.cwd;
  this.value = this.cwd;

  if (options.label && ~options.label.indexOf('%path')) {
    this._label.setContent(options.label.replace('%path', this.cwd));
  }

  this.on('select', function(item) {
    var value = item.content.replace(/\{[^{}]+\}/g, '').replace(/@$/, '')
      , file = path.resolve(self.cwd, value);

    return fs.stat(file, function(err, stat) {
      if (err) {
        return self.emit('error', err, file);
      }
      self.file = file;
      self.value = file;
      if (stat.isDirectory()) {
        self.emit('cd', file, self.cwd);
        self.cwd = file;
        if (options.label && ~options.label.indexOf('%path')) {
          self._label.setContent(options.label.replace('%path', file));
        }
        self.refresh();
      } else {
        self.emit('file', file);
      }
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.filemanager.prototype"></a>[module blessed.filemanager.prototype](#apidoc.module.blessed.filemanager.prototype)

#### <a name="apidoc.element.blessed.filemanager.prototype.pick"></a>[function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>pick (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.pick)
- description and source-code
```javascript
pick = function (cwd, callback) {
  if (!callback) {
    callback = cwd;
    cwd = null;
  }

  var self = this
    , focused = this.screen.focused === this
    , hidden = this.hidden
    , onfile
    , oncancel;

  function resume() {
    self.removeListener('file', onfile);
    self.removeListener('cancel', oncancel);
    if (hidden) {
      self.hide();
    }
    if (!focused) {
      self.screen.restoreFocus();
    }
    self.screen.render();
  }

  this.on('file', onfile = function(file) {
    resume();
    return callback(null, file);
  });

  this.on('cancel', oncancel = function() {
    resume();
    return callback();
  });

  this.refresh(cwd, function(err) {
    if (err) return callback(err);

    if (hidden) {
      self.show();
    }

    if (!focused) {
      self.screen.saveFocus();
      self.focus();
    }

    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.filemanager.prototype.refresh"></a>[function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>refresh (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.refresh)
- description and source-code
```javascript
refresh = function (cwd, callback) {
  if (!callback) {
    callback = cwd;
    cwd = null;
  }

  var self = this;

  if (cwd) this.cwd = cwd;
  else cwd = this.cwd;

  return fs.readdir(cwd, function(err, list) {
    if (err && err.code === 'ENOENT') {
      self.cwd = cwd !== process.env.HOME
        ? process.env.HOME
        : '/';
      return self.refresh(callback);
    }

    if (err) {
      if (callback) return callback(err);
      return self.emit('error', err, cwd);
    }

    var dirs = []
      , files = [];

    list.unshift('..');

    list.forEach(function(name) {
      var f = path.resolve(cwd, name)
        , stat;

      try {
        stat = fs.lstatSync(f);
      } catch (e) {
        ;
      }

      if ((stat && stat.isDirectory()) || name === '..') {
        dirs.push({
          name: name,
          text: '{light-blue-fg}' + name + '{/light-blue-fg}/',
          dir: true
        });
      } else if (stat && stat.isSymbolicLink()) {
        files.push({
          name: name,
          text: '{light-cyan-fg}' + name + '{/light-cyan-fg}@',
          dir: false
        });
      } else {
        files.push({
          name: name,
          text: name,
          dir: false
        });
      }
    });

    dirs = helpers.asort(dirs);
    files = helpers.asort(files);

    list = dirs.concat(files).map(function(data) {
      return data.text;
    });

    self.setItems(list);
    self.select(0);
    self.screen.render();

    self.emit('refresh');

    if (callback) callback();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.filemanager.prototype.reset"></a>[function <span class="apidocSignatureSpan">blessed.filemanager.prototype.</span>reset (cwd, callback)](#apidoc.element.blessed.filemanager.prototype.reset)
- description and source-code
```javascript
reset = function (cwd, callback) {
  if (!callback) {
    callback = cwd;
    cwd = null;
  }
  this.cwd = cwd || this.options.cwd;
  this.refresh(callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.form"></a>[module blessed.form](#apidoc.module.blessed.form)

#### <a name="apidoc.element.blessed.form.form"></a>[function <span class="apidocSignatureSpan">blessed.</span>form (options)](#apidoc.element.blessed.form.form)
- description and source-code
```javascript
function Form(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Form(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  Box.call(this, options);

  if (options.keys) {
    this.screen._listenKeys(this);
    this.on('element keypress', function(el, ch, key) {
      if ((key.name === 'tab' && !key.shift)
          || (el.type === 'textbox' && options.autoNext && key.name === 'enter')
          || key.name === 'down'
          || (options.vi && key.name === 'j')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'j') return;
          if (key.name === 'tab') {
            // Workaround, since we can't stop the tab from being added.
            el.emit('keypress', null, { name: 'backspace' });
          }
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusNext();
        return;
      }

      if ((key.name === 'tab' && key.shift)
          || key.name === 'up'
          || (options.vi && key.name === 'k')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'k') return;
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusPrevious();
        return;
      }

      if (key.name === 'escape') {
        self.focus();
        return;
      }
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.form.prototype"></a>[module blessed.form.prototype](#apidoc.module.blessed.form.prototype)

#### <a name="apidoc.element.blessed.form.prototype._refresh"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>_refresh ()](#apidoc.element.blessed.form.prototype._refresh)
- description and source-code
```javascript
_refresh = function () {
  // XXX Possibly remove this if statement and refresh on every focus.
  // Also potentially only include *visible* focusable elements.
  // This would remove the need to check for _selected.visible in previous()
  // and next().
  if (!this._children) {
    var out = [];

    this.children.forEach(function fn(el) {
      if (el.keyable) out.push(el);
      el.children.forEach(fn);
    });

    this._children = out;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype._visible"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>_visible ()](#apidoc.element.blessed.form.prototype._visible)
- description and source-code
```javascript
_visible = function () {
  return !!this._children.filter(function(el) {
    return el.visible;
  }).length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.cancel"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>cancel ()](#apidoc.element.blessed.form.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  this.emit('cancel');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.focusFirst"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusFirst ()](#apidoc.element.blessed.form.prototype.focusFirst)
- description and source-code
```javascript
focusFirst = function () {
  this.resetSelected();
  this.focusNext();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.focusLast"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusLast ()](#apidoc.element.blessed.form.prototype.focusLast)
- description and source-code
```javascript
focusLast = function () {
  this.resetSelected();
  this.focusPrevious();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.focusNext"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusNext ()](#apidoc.element.blessed.form.prototype.focusNext)
- description and source-code
```javascript
focusNext = function () {
  var next = this.next();
  if (next) next.focus();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.focusPrevious"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>focusPrevious ()](#apidoc.element.blessed.form.prototype.focusPrevious)
- description and source-code
```javascript
focusPrevious = function () {
  var previous = this.previous();
  if (previous) previous.focus();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.next"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>next ()](#apidoc.element.blessed.form.prototype.next)
- description and source-code
```javascript
next = function () {
  this._refresh();

  if (!this._visible()) return;

  if (!this._selected) {
    this._selected = this._children[0];
    if (!this._selected.visible) return this.next();
    if (this.screen.focused !== this._selected) return this._selected;
  }

  var i = this._children.indexOf(this._selected);
  if (!~i || !this._children[i + 1]) {
    this._selected = this._children[0];
    if (!this._selected.visible) return this.next();
    return this._selected;
  }

  this._selected = this._children[i + 1];
  if (!this._selected.visible) return this.next();
  return this._selected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.previous"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>previous ()](#apidoc.element.blessed.form.prototype.previous)
- description and source-code
```javascript
previous = function () {
  this._refresh();

  if (!this._visible()) return;

  if (!this._selected) {
    this._selected = this._children[this._children.length - 1];
    if (!this._selected.visible) return this.previous();
    if (this.screen.focused !== this._selected) return this._selected;
  }

  var i = this._children.indexOf(this._selected);
  if (!~i || !this._children[i - 1]) {
    this._selected = this._children[this._children.length - 1];
    if (!this._selected.visible) return this.previous();
    return this._selected;
  }

  this._selected = this._children[i - 1];
  if (!this._selected.visible) return this.previous();
  return this._selected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.reset"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>reset ()](#apidoc.element.blessed.form.prototype.reset)
- description and source-code
```javascript
reset = function () {
  this.children.forEach(function fn(el) {
    switch (el.type) {
      case 'screen':
        break;
      case 'box':
        break;
      case 'text':
        break;
      case 'line':
        break;
      case 'scrollable-box':
        break;
      case 'list':
        el.select(0);
        return;
      case 'form':
        break;
      case 'input':
        break;
      case 'textbox':
        el.clearInput();
        return;
      case 'textarea':
        el.clearInput();
        return;
      case 'button':
        delete el.value;
        break;
      case 'progress-bar':
        el.setProgress(0);
        break;
      case 'file-manager':
        el.refresh(el.options.cwd);
        return;
      case 'checkbox':
        el.uncheck();
        return;
      case 'radio-set':
        break;
      case 'radio-button':
        el.uncheck();
        return;
      case 'prompt':
        break;
      case 'question':
        break;
      case 'message':
        break;
      case 'info':
        break;
      case 'loading':
        break;
      case 'list-bar':
        //el.select(0);
        break;
      case 'dir-manager':
        el.refresh(el.options.cwd);
        return;
      case 'terminal':
        el.write('');
        return;
      case 'image':
        //el.clearImage();
        return;
    }
    el.children.forEach(fn);
  });

  this.emit('reset');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.resetSelected"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>resetSelected ()](#apidoc.element.blessed.form.prototype.resetSelected)
- description and source-code
```javascript
resetSelected = function () {
  this._selected = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.form.prototype.submit"></a>[function <span class="apidocSignatureSpan">blessed.form.prototype.</span>submit ()](#apidoc.element.blessed.form.prototype.submit)
- description and source-code
```javascript
submit = function () {
  var out = {};

  this.children.forEach(function fn(el) {
    if (el.value != null) {
      var name = el.name || el.type;
      if (Array.isArray(out[name])) {
        out[name].push(el.value);
      } else if (out[name]) {
        out[name] = [out[name], el.value];
      } else {
        out[name] = el.value;
      }
    }
    el.children.forEach(fn);
  });

  this.emit('submit', out);

  return this.submission = out;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.helpers"></a>[module blessed.helpers](#apidoc.module.blessed.helpers)

#### <a name="apidoc.element.blessed.helpers.Element"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>Element (options)](#apidoc.element.blessed.helpers.Element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.Screen"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>Screen (options)](#apidoc.element.blessed.helpers.Screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers._element"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>_element (options)](#apidoc.element.blessed.helpers._element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers._screen"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>_screen (options)](#apidoc.element.blessed.helpers._screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.asort"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>asort (obj)](#apidoc.element.blessed.helpers.asort)
- description and source-code
```javascript
asort = function (obj) {
  return obj.sort(function(a, b) {
    a = a.name.toLowerCase();
    b = b.name.toLowerCase();

    if (a[0] === '.' && b[0] === '.') {
      a = a[1];
      b = b[1];
    } else {
      a = a[0];
      b = b[0];
    }

    return a > b ? 1 : (a < b ? -1 : 0);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.attrToBinary"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>attrToBinary (style, element)](#apidoc.element.blessed.helpers.attrToBinary)
- description and source-code
```javascript
attrToBinary = function (style, element) {
  return helpers.Element.prototype.sattr.call(element || {}, style);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.cleanTags"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>cleanTags (text)](#apidoc.element.blessed.helpers.cleanTags)
- description and source-code
```javascript
cleanTags = function (text) {
  return helpers.stripTags(text).trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.dropUnicode"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>dropUnicode (text)](#apidoc.element.blessed.helpers.dropUnicode)
- description and source-code
```javascript
dropUnicode = function (text) {
  if (!text) return '';
  return text
    .replace(unicode.chars.all, '??')
    .replace(unicode.chars.combining, '')
    .replace(unicode.chars.surrogate, '?');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.escape"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>escape (text)](#apidoc.element.blessed.helpers.escape)
- description and source-code
```javascript
escape = function (text) {
  return text.replace(/[{}]/g, function(ch) {
    return ch === '{' ? '{open}' : '{close}';
  });
}
```
- example usage
```shell
...

- __merge(a, b)__ - Merge objects 'a' and 'b' into object 'a'.
- __asort(obj)__ - Sort array alphabetically by 'name' prop.
- __hsort(obj)__ - Sort array numerically by 'index' prop.
- __findFile(start, target)__ - Find a file at 'start' directory with name
'target'.
- __escape(text)__ - Escape content's tags to be passed into 'el.setContent()'.
Example: 'box.setContent('escaped tag: ' + blessed.escape('{bold}{/bold}'));'
- __parseTags(text)__ - Parse tags into SGR escape codes.
- __generateTags(style, text)__ - Generate text tags based on 'style' object.
- __attrToBinary(style, element)__ - Convert 'style' attributes to binary
format.
- __stripTags(text)__ - Strip text of tags and SGR sequences.
- __cleanTags(text)__ - Strip text of tags, SGR escape code, and
leading/trailing whitespace.
...
```

#### <a name="apidoc.element.blessed.helpers.findFile"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>findFile (start, target)](#apidoc.element.blessed.helpers.findFile)
- description and source-code
```javascript
findFile = function (start, target) {
  return (function read(dir) {
    var files, file, stat, out;

    if (dir === '/dev' || dir === '/sys'
        || dir === '/proc' || dir === '/net') {
      return null;
    }

    try {
      files = fs.readdirSync(dir);
    } catch (e) {
      files = [];
    }

    for (var i = 0; i < files.length; i++) {
      file = files[i];

      if (file === target) {
        return (dir === '/' ? '' : dir) + '/' + file;
      }

      try {
        stat = fs.lstatSync((dir === '/' ? '' : dir) + '/' + file);
      } catch (e) {
        stat = null;
      }

      if (stat && stat.isDirectory() && !stat.isSymbolicLink()) {
        out = read((dir === '/' ? '' : dir) + '/' + file);
        if (out) return out;
      }
    }

    return null;
  })(start);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.generateTags"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>generateTags (style, text)](#apidoc.element.blessed.helpers.generateTags)
- description and source-code
```javascript
generateTags = function (style, text) {
  var open = ''
    , close = '';

  Object.keys(style || {}).forEach(function(key) {
    var val = style[key];
    if (typeof val === 'string') {
      val = val.replace(/^light(?!-)/, 'light-');
      val = val.replace(/^bright(?!-)/, 'bright-');
      open = '{' + val + '-' + key + '}' + open;
      close += '{/' + val + '-' + key + '}';
    } else {
      if (val === true) {
        open = '{' + key + '}' + open;
        close += '{/' + key + '}';
      }
    }
  });

  if (text != null) {
    return open + text + close;
  }

  return {
    open: open,
    close: close
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.hsort"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>hsort (obj)](#apidoc.element.blessed.helpers.hsort)
- description and source-code
```javascript
hsort = function (obj) {
  return obj.sort(function(a, b) {
    return b.index - a.index;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.merge"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>merge (a, b)](#apidoc.element.blessed.helpers.merge)
- description and source-code
```javascript
merge = function (a, b) {
  Object.keys(b).forEach(function(key) {
    a[key] = b[key];
  });
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.parseTags"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>parseTags (text, screen)](#apidoc.element.blessed.helpers.parseTags)
- description and source-code
```javascript
parseTags = function (text, screen) {
  return helpers.Element.prototype._parseTags.call(
    { parseTags: true, screen: screen || helpers.Screen.global }, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.sprintf"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>sprintf (src)](#apidoc.element.blessed.helpers.sprintf)
- description and source-code
```javascript
function sprintf(src) {
  var params = Array.prototype.slice.call(arguments, 1)
    , rule = /%([\-+# ]{1,4})?(\d+(?:\.\d+)?)?([doxXsc])/g
    , i = 0;

  return src.replace(rule, function(_, flag, width, type) {
    var flags = (flag || '').split('')
      , param = params[i] != null ? params[i] : ''
      , initial = param
      // , width = +width
      , opt = {}
      , pre = '';

    i++;

    switch (type) {
      case 'd': // signed int
        param = (+param).toString(10);
        break;
      case 'o': // unsigned octal
        param = (+param).toString(8);
        break;
      case 'x': // unsigned hex int
        param = (+param).toString(16);
        break;
      case 'X': // unsigned hex int uppercase
        param = (+param).toString(16).toUppercase();
        break;
      case 's': // string
        break;
      case 'c': // char
        param = isFinite(param)
          ? String.fromCharCode(param || 0200)
          : '';
        break;
    }

    flags.forEach(function(flag) {
      switch (flag) {
        // left-justify by width
        case '-':
          opt.left = true;
          break;
        // always precede numbers with their signs
        case '+':
          opt.signs = true;
          break;
        // used with o, x, X - value is preceded with 0, 0x, or 0X respectively.
        // used with a, A, e, E, f, F, g, G - forces written output to contain
        // a decimal point even if no more digits follow
        case '#':
          opt.hexpoint = true;
          break;
        // if no sign is going to be written, black space in front of the value
        case ' ':
          opt.space = true;
          break;
      }
    });

    width = +width.split('.')[0];

    // Should this be for opt.left too?
    // Example: %2.2X - turns 0 into 00
    if (width && !opt.left) {
      param = param + '';
      while (param.length < width) {
        param = '0' + param;
      }
    }

    if (opt.signs) {
      if (+initial >= 0) {
        pre += '+';
      }
    }

    if (opt.space) {
      if (!opt.signs && +initial >= 0) {
        pre += ' ';
      }
    }

    if (opt.hexpoint) {
      switch (type) {
        case 'o': // unsigned octal
          pre += '0';
          break;
        case 'x': // unsigned hex int
          pre += '0x';
          break;
        case 'X': // unsigned hex int uppercase
          pre += '0X';
          break;
      }
    }

    if (opt.left) {
      if (width > (pre.length + param.length)) {
        width -= pre.length + param.length;
        pre = Array(width + 1).join(' ') + pre;
      }
    }

    return pre + param;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.stripTags"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>stripTags (text)](#apidoc.element.blessed.helpers.stripTags)
- description and source-code
```javascript
stripTags = function (text) {
  if (!text) return '';
  return text
    .replace(/{(\/?)([\w\-,;!#]*)}/g, '')
    .replace(/\x1b\[[\d;]*m/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.helpers.tryRead"></a>[function <span class="apidocSignatureSpan">blessed.helpers.</span>tryRead (file)](#apidoc.element.blessed.helpers.tryRead)
- description and source-code
```javascript
function tryRead(file) {
  if (Array.isArray(file)) {
    for (var i = 0; i < file.length; i++) {
      var data = tryRead(file[i]);
      if (data) return data;
    }
    return '';
  }
  if (!file) return '';
  file = path.resolve.apply(path, arguments);
  try {
    return fs.readFileSync(file, 'utf8');
  } catch (e) {
    return '';
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.layout"></a>[module blessed.layout](#apidoc.module.blessed.layout)

#### <a name="apidoc.element.blessed.layout.layout"></a>[function <span class="apidocSignatureSpan">blessed.</span>layout (options)](#apidoc.element.blessed.layout.layout)
- description and source-code
```javascript
function Layout(options) {
  if (!(this instanceof Node)) {
    return new Layout(options);
  }

  options = options || {};

  if ((options.width == null
      && (options.left == null && options.right == null))
      || (options.height == null
      && (options.top == null && options.bottom == null))) {
    throw new Error(''Layout' must have a width and height!');
  }

  options.layout = options.layout || 'inline';

  Element.call(this, options);

  if (options.renderer) {
    this.renderer = options.renderer;
  }
}
```
- example usage
```shell
...

Here is an example of how to provide a renderer. Note that this is also the
default renderer if none is provided. This renderer will render each child as
though they were 'display: inline-block;' in CSS, as if there were a
dynamically sized horizontal grid from left to right.

''' js
var layout = blessed.layout({
parent: screen,
top: 'center',
left: 'center',
width: '50%',
height: '50%',
border: 'line',
style: {
...
```



# <a name="apidoc.module.blessed.layout.prototype"></a>[module blessed.layout.prototype](#apidoc.module.blessed.layout.prototype)

#### <a name="apidoc.element.blessed.layout.prototype._renderCoords"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>_renderCoords ()](#apidoc.element.blessed.layout.prototype._renderCoords)
- description and source-code
```javascript
_renderCoords = function () {
  var coords = this._getCoords(true);
  var children = this.children;
  this.children = [];
  this._render();
  this.children = children;
  return coords;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.layout.prototype.getLast"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>getLast (i)](#apidoc.element.blessed.layout.prototype.getLast)
- description and source-code
```javascript
getLast = function (i) {
  while (this.children[--i]) {
    var el = this.children[i];
    if (this.isRendered(el)) return el;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.layout.prototype.getLastCoords"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>getLastCoords (i)](#apidoc.element.blessed.layout.prototype.getLastCoords)
- description and source-code
```javascript
getLastCoords = function (i) {
  var last = this.getLast(i);
  if (last) return last.lpos;
}
```
- example usage
```shell
...

    return function iterator(el, i) {
// Make our children shrinkable. If they don't have a height, for
// example, calculate it for them.
el.shrink = true;

// Find the previous rendered child's coordinates
var last = self.getLastCoords(i);

// If there is no previously rendered element, we are on the first child.
if (!last) {
  el.position.left = 0;
  el.position.top = 0;
} else {
  // Otherwise, figure out where to place this child. We'll start by
...
```

#### <a name="apidoc.element.blessed.layout.prototype.isRendered"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>isRendered (el)](#apidoc.element.blessed.layout.prototype.isRendered)
- description and source-code
```javascript
isRendered = function (el) {
  if (!el.lpos) return false;
  return (el.lpos.xl - el.lpos.xi) > 0
      && (el.lpos.yl - el.lpos.yi) > 0;
}
```
- example usage
```shell
...
if (el.position.left + el.width <= width) {
  el.position.top = rowOffset;
} else {
  // Otherwise we need to start a new row and calculate a new
  // 'rowOffset' and 'rowIndex' (the index of the child on the current
  // row).
  rowOffset += self.children.slice(rowIndex, i).reduce(function(out, el) {
    if (!self.isRendered(el)) return out;
    out = Math.max(out, el.lpos.yl - el.lpos.yi);
    return out;
  }, 0);
  rowIndex = i;
  el.position.left = 0;
  el.position.top = rowOffset;
}
...
```

#### <a name="apidoc.element.blessed.layout.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>render ()](#apidoc.element.blessed.layout.prototype.render)
- description and source-code
```javascript
render = function () {
  this._emit('prerender');

  var coords = this._renderCoords();
  if (!coords) {
    delete this.lpos;
    return;
  }

  if (coords.xl - coords.xi <= 0) {
    coords.xl = Math.max(coords.xl, coords.xi);
    return;
  }

  if (coords.yl - coords.yi <= 0) {
    coords.yl = Math.max(coords.yl, coords.yi);
    return;
  }

  this.lpos = coords;

  if (this.border) coords.xi++, coords.xl--, coords.yi++, coords.yl--;
  if (this.tpadding) {
    coords.xi += this.padding.left, coords.xl -= this.padding.right;
    coords.yi += this.padding.top, coords.yl -= this.padding.bottom;
  }

  var iterator = this.renderer(coords);

  if (this.border) coords.xi--, coords.xl++, coords.yi--, coords.yl++;
  if (this.tpadding) {
    coords.xi -= this.padding.left, coords.xl += this.padding.right;
    coords.yi -= this.padding.top, coords.yl += this.padding.bottom;
  }

  this.children.forEach(function(el, i) {
    if (el.screen._ci !== -1) {
      el.index = el.screen._ci++;
    }
    var rendered = iterator(el, i);
    if (rendered === false) {
      delete el.lpos;
      return;
    }
    // if (el.screen._rendering) {
    //   el._rendering = true;
    // }
    el.render();
    // if (el.screen._rendering) {
    //   el._rendering = false;
    // }
  });

  this._emit('render', [coords]);

  return coords;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.layout.prototype.renderer"></a>[function <span class="apidocSignatureSpan">blessed.layout.prototype.</span>renderer (coords)](#apidoc.element.blessed.layout.prototype.renderer)
- description and source-code
```javascript
renderer = function (coords) {
  var self = this;

  // The coordinates of the layout element
  var width = coords.xl - coords.xi
    , height = coords.yl - coords.yi
    , xi = coords.xi
    , yi = coords.yi;

  // The current row offset in cells (which row are we on?)
  var rowOffset = 0;

  // The index of the first child in the row
  var rowIndex = 0;
  var lastRowIndex = 0;

  // Figure out the highest width child
  if (this.options.layout === 'grid') {
    var highWidth = this.children.reduce(function(out, el) {
      out = Math.max(out, el.width);
      return out;
    }, 0);
  }

  return function iterator(el, i) {
    // Make our children shrinkable. If they don't have a height, for
    // example, calculate it for them.
    el.shrink = true;

    // Find the previous rendered child's coordinates
    var last = self.getLast(i);

    // If there is no previously rendered element, we are on the first child.
    if (!last) {
      el.position.left = 0;
      el.position.top = 0;
    } else {
      // Otherwise, figure out where to place this child. We'll start by
      // setting it's 'left'/'x' coordinate to right after the previous
      // rendered element. This child will end up directly to the right of it.
      el.position.left = last.lpos.xl - xi;

      // Make sure the position matches the highest width element
      if (self.options.layout === 'grid') {
        // Compensate with width:
        // el.position.width = el.width + (highWidth - el.width);
        // Compensate with position:
        el.position.left += highWidth - (last.lpos.xl - last.lpos.xi);
      }

      // If our child does not overlap the right side of the Layout, set it's
      // 'top'/'y' to the current 'rowOffset' (the coordinate for the current
      // row).
      if (el.position.left + el.width <= width) {
        el.position.top = rowOffset;
      } else {
        // Otherwise we need to start a new row and calculate a new
        // 'rowOffset' and 'rowIndex' (the index of the child on the current
        // row).
        rowOffset += self.children.slice(rowIndex, i).reduce(function(out, el) {
          if (!self.isRendered(el)) return out;
          out = Math.max(out, el.lpos.yl - el.lpos.yi);
          return out;
        }, 0);
        lastRowIndex = rowIndex;
        rowIndex = i;
        el.position.left = 0;
        el.position.top = rowOffset;
      }
    }

    // Make sure the elements on lower rows graviatate up as much as possible
    if (self.options.layout === 'inline') {
      var above = null;
      var abovea = Infinity;
      for (var j = lastRowIndex; j < rowIndex; j++) {
        var l = self.children[j];
        if (!self.isRendered(l)) continue;
        var abs = Math.abs(el.position.left - (l.lpos.xi - xi));
        // if (abs < abovea && (l.lpos.xl - l.lpos.xi) <= el.width) {
        if (abs < abovea) {
          above = l;
          abovea = abs;
        }
      }
      if (above) {
        el.position.top = above.lpos.yl - yi;
      }
    }

    // If our child overflows the Layout, do not render it!
    // Disable this feature for now.
    if (el.position.top + el.height > height) {
      // Returning false tells blessed to ignore this child.
      // return false;
    }
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.list"></a>[module blessed.list](#apidoc.module.blessed.list)

#### <a name="apidoc.element.blessed.list.list"></a>[function <span class="apidocSignatureSpan">blessed.</span>list (options)](#apidoc.element.blessed.list.list)
- description and source-code
```javascript
function List(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new List(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  // Possibly put this here: this.items = [];
  options.scrollable = true;
  Box.call(this, options);

  this.value = '';
  this.items = [];
  this.ritems = [];
  this.selected = 0;
  this._isList = true;

  if (!this.style.selected) {
    this.style.selected = {};
    this.style.selected.bg = options.selectedBg;
    this.style.selected.fg = options.selectedFg;
    this.style.selected.bold = options.selectedBold;
    this.style.selected.underline = options.selectedUnderline;
    this.style.selected.blink = options.selectedBlink;
    this.style.selected.inverse = options.selectedInverse;
    this.style.selected.invisible = options.selectedInvisible;
  }

  if (!this.style.item) {
    this.style.item = {};
    this.style.item.bg = options.itemBg;
    this.style.item.fg = options.itemFg;
    this.style.item.bold = options.itemBold;
    this.style.item.underline = options.itemUnderline;
    this.style.item.blink = options.itemBlink;
    this.style.item.inverse = options.itemInverse;
    this.style.item.invisible = options.itemInvisible;
  }

  // Legacy: for apps written before the addition of item attributes.
  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    if (self.style[name] != null && self.style.item[name] == null) {
      self.style.item[name] = self.style[name];
    }
  });

  if (this.options.itemHoverBg) {
    this.options.itemHoverEffects = { bg: this.options.itemHoverBg };
  }

  if (this.options.itemHoverEffects) {
    this.style.item.hover = this.options.itemHoverEffects;
  }

  if (this.options.itemFocusEffects) {
    this.style.item.focus = this.options.itemFocusEffects;
  }

  this.interactive = options.interactive !== false;

  this.mouse = options.mouse || false;

  if (options.items) {
    this.ritems = options.items;
    options.items.forEach(this.add.bind(this));
  }

  this.select(0);

  if (options.mouse) {
    this.screen._listenMouse(this);
    this.on('element wheeldown', function() {
      self.select(self.selected + 2);
      self.screen.render();
    });
    this.on('element wheelup', function() {
      self.select(self.selected - 2);
      self.screen.render();
    });
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.up();
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.down();
        self.screen.render();
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'l' && !key.shift)) {
        self.enterSelected();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.cancelSelected();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.move(-((self.height - self.iheight) / 2) | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.move((self.height - self.iheight) / 2 | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'b' && key.ctrl) {
        self.move(-(self.height - self.iheight));
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'f' && key.ctrl) {
        self.move(self.height - self.iheight);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'h' && key.shift) {
        self.move(self.childBase - self.selected);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'm' && key.shift) {
        // TODO: Maybe use Math.min(this.items.length,
        // ... for calculating visible items elsewhere.
        var visible = Math.min(
          self.height - self.iheight,
          self.items.length) / 2 | 0;
        self.move(sel ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.list.prototype"></a>[module blessed.list.prototype](#apidoc.module.blessed.list.prototype)

#### <a name="apidoc.element.blessed.list.prototype.add"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>add (content)](#apidoc.element.blessed.list.prototype.add)
- description and source-code
```javascript
add = function (content) {
  content = typeof content === 'string' ? content : content.getContent();

  var item = this.createItem(content);
  item.position.top = this.items.length;
  if (!this.screen.autoPadding) {
    item.position.top = this.itop + this.items.length;
  }

  this.ritems.push(content);
  this.items.push(item);
  this.append(item);

  if (this.items.length === 1) {
    this.select(0);
  }

  this.emit('add item');

  return item;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.addItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>addItem (content)](#apidoc.element.blessed.list.prototype.addItem)
- description and source-code
```javascript
addItem = function (content) {
  content = typeof content === 'string' ? content : content.getContent();

  var item = this.createItem(content);
  item.position.top = this.items.length;
  if (!this.screen.autoPadding) {
    item.position.top = this.itop + this.items.length;
  }

  this.ritems.push(content);
  this.items.push(item);
  this.append(item);

  if (this.items.length === 1) {
    this.select(0);
  }

  this.emit('add item');

  return item;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.appendItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>appendItem (content)](#apidoc.element.blessed.list.prototype.appendItem)
- description and source-code
```javascript
appendItem = function (content) {
  content = typeof content === 'string' ? content : content.getContent();

  var item = this.createItem(content);
  item.position.top = this.items.length;
  if (!this.screen.autoPadding) {
    item.position.top = this.itop + this.items.length;
  }

  this.ritems.push(content);
  this.items.push(item);
  this.append(item);

  if (this.items.length === 1) {
    this.select(0);
  }

  this.emit('add item');

  return item;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.cancelSelected"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>cancelSelected (i)](#apidoc.element.blessed.list.prototype.cancelSelected)
- description and source-code
```javascript
cancelSelected = function (i) {
  if (i != null) this.select(i);
  this.emit('action');
  this.emit('cancel');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.clearItems"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>clearItems ()](#apidoc.element.blessed.list.prototype.clearItems)
- description and source-code
```javascript
clearItems = function () {
  return this.setItems([]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.createItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>createItem (content)](#apidoc.element.blessed.list.prototype.createItem)
- description and source-code
```javascript
createItem = function (content) {
  var self = this;

  // Note: Could potentially use Button here.
  var options = {
    screen: this.screen,
    content: content,
    align: this.align || 'left',
    top: 0,
    left: 0,
    right: (this.scrollbar ? 1 : 0),
    tags: this.parseTags,
    height: 1,
    hoverEffects: this.mouse ? this.style.item.hover : null,
    focusEffects: this.mouse ? this.style.item.focus : null,
    autoFocus: false
  };

  if (!this.screen.autoPadding) {
    options.top = 1;
    options.left = this.ileft;
    options.right = this.iright + (this.scrollbar ? 1 : 0);
  }

  // if (this.shrink) {
  // XXX NOTE: Maybe just do this on all shrinkage once autoPadding is default?
  if (this.shrink && this.options.normalShrink) {
    delete options.right;
    options.width = 'shrink';
  }

  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    options[name] = function() {
      var attr = self.items[self.selected] === item && self.interactive
        ? self.style.selected[name]
        : self.style.item[name];
      if (typeof attr === 'function') attr = attr(item);
      return attr;
    };
  });

  if (this.style.transparent) {
    options.transparent = true;
  }

  var item = new Box(options);

  if (this.mouse) {
    item.on('click', function() {
      self.focus();
      if (self.items[self.selected] === item) {
        self.emit('action', item, self.selected);
        self.emit('select', item, self.selected);
        return;
      }
      self.select(item);
      self.screen.render();
    });
  }

  this.emit('create item');

  return item;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.down"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>down (offset)](#apidoc.element.blessed.list.prototype.down)
- description and source-code
```javascript
down = function (offset) {
  this.move(offset || 1);
}
```
- example usage
```shell
...
program.hideCursor();
program.clear();

program.move(1, 1);
program.bg('black');
program.write('Hello world', 'blue fg');
program.setx((program.cols / 2 | 0) - 4);
program.down(5);
program.write('Hi again!');
program.bg('!black');
program.feed();
'''


#### Testing
...
```

#### <a name="apidoc.element.blessed.list.prototype.enterSelected"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>enterSelected (i)](#apidoc.element.blessed.list.prototype.enterSelected)
- description and source-code
```javascript
enterSelected = function (i) {
  if (i != null) this.select(i);
  this.emit('action', this.items[this.selected], this.selected);
  this.emit('select', this.items[this.selected], this.selected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.find"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>find (search, back)](#apidoc.element.blessed.list.prototype.find)
- description and source-code
```javascript
find = function (search, back) {
  var start = this.selected + (back ? -1 : 1)
    , i;

  if (typeof search === 'number') search += '';

  if (search && search[0] === '/' && search[search.length - 1] === '/') {
    try {
      search = new RegExp(search.slice(1, -1));
    } catch (e) {
      ;
    }
  }

  var test = typeof search === 'string'
    ? function(item) { return !!~item.indexOf(search); }
    : (search.test ? search.test.bind(search) : search);

  if (typeof test !== 'function') {
    if (this.screen.options.debug) {
      throw new Error('fuzzyFind(): 'test' is not a function.');
    }
    return this.selected;
  }

  if (!back) {
    for (i = start; i < this.ritems.length; i++) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
    for (i = 0; i < start; i++) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
  } else {
    for (i = start; i >= 0; i--) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
    for (i = this.ritems.length - 1; i > start; i--) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
  }

  return this.selected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.fuzzyFind"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>fuzzyFind (search, back)](#apidoc.element.blessed.list.prototype.fuzzyFind)
- description and source-code
```javascript
fuzzyFind = function (search, back) {
  var start = this.selected + (back ? -1 : 1)
    , i;

  if (typeof search === 'number') search += '';

  if (search && search[0] === '/' && search[search.length - 1] === '/') {
    try {
      search = new RegExp(search.slice(1, -1));
    } catch (e) {
      ;
    }
  }

  var test = typeof search === 'string'
    ? function(item) { return !!~item.indexOf(search); }
    : (search.test ? search.test.bind(search) : search);

  if (typeof test !== 'function') {
    if (this.screen.options.debug) {
      throw new Error('fuzzyFind(): 'test' is not a function.');
    }
    return this.selected;
  }

  if (!back) {
    for (i = start; i < this.ritems.length; i++) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
    for (i = 0; i < start; i++) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
  } else {
    for (i = start; i >= 0; i--) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
    for (i = this.ritems.length - 1; i > start; i--) {
      if (test(helpers.cleanTags(this.ritems[i]))) return i;
    }
  }

  return this.selected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.getItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>getItem (child)](#apidoc.element.blessed.list.prototype.getItem)
- description and source-code
```javascript
getItem = function (child) {
  return this.items[this.getItemIndex(child)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.getItemIndex"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>getItemIndex (child)](#apidoc.element.blessed.list.prototype.getItemIndex)
- description and source-code
```javascript
getItemIndex = function (child) {
  if (typeof child === 'number') {
    return child;
  } else if (typeof child === 'string') {
    var i = this.ritems.indexOf(child);
    if (~i) return i;
    for (i = 0; i < this.ritems.length; i++) {
      if (helpers.cleanTags(this.ritems[i]) === child) {
        return i;
      }
    }
    return -1;
  } else {
    return this.items.indexOf(child);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.insertItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>insertItem (child, content)](#apidoc.element.blessed.list.prototype.insertItem)
- description and source-code
```javascript
insertItem = function (child, content) {
  content = typeof content === 'string' ? content : content.getContent();
  var i = this.getItemIndex(child);
  if (!~i) return;
  if (i >= this.items.length) return this.appendItem(content);
  var item = this.createItem(content);
  for (var j = i; j < this.items.length; j++) {
    this.items[j].position.top++;
  }
  item.position.top = i + (!this.screen.autoPadding ? 1 : 0);
  this.ritems.splice(i, 0, content);
  this.items.splice(i, 0, item);
  this.append(item);
  if (i === this.selected) {
    this.select(i + 1);
  }
  this.emit('insert item');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.move"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>move (offset)](#apidoc.element.blessed.list.prototype.move)
- description and source-code
```javascript
move = function (offset) {
  this.select(this.selected + offset);
}
```
- example usage
```shell
...
  program.showCursor();
  program.normalBuffer();
  process.exit(0);
});

program.on('mouse', function(data) {
  if (data.action === 'mousemove') {
    program.move(data.x, data.y);
    program.bg('red');
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
...
```

#### <a name="apidoc.element.blessed.list.prototype.pick"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>pick (label, callback)](#apidoc.element.blessed.list.prototype.pick)
- description and source-code
```javascript
pick = function (label, callback) {
  if (!callback) {
    callback = label;
    label = null;
  }

  if (!this.interactive) {
    return callback();
  }

  var self = this;
  var focused = this.screen.focused;
  if (focused && focused._done) focused._done('stop');
  this.screen.saveFocus();

  // XXX Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.focus();
  this.show();
  this.select(0);
  if (label) this.setLabel(label);
  this.screen.render();
  this.once('action', function(el, selected) {
    if (label) self.removeLabel();
    self.screen.restoreFocus();
    self.hide();
    self.screen.render();
    if (!el) return callback();
    return callback(null, helpers.cleanTags(self.ritems[selected]));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.popItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>popItem ()](#apidoc.element.blessed.list.prototype.popItem)
- description and source-code
```javascript
popItem = function () {
  return this.removeItem(this.items.length - 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.pushItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>pushItem (content)](#apidoc.element.blessed.list.prototype.pushItem)
- description and source-code
```javascript
pushItem = function (content) {
  this.appendItem(content);
  return this.items.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.removeItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>removeItem (child)](#apidoc.element.blessed.list.prototype.removeItem)
- description and source-code
```javascript
removeItem = function (child) {
  var i = this.getItemIndex(child);
  if (~i && this.items[i]) {
    child = this.items.splice(i, 1)[0];
    this.ritems.splice(i, 1);
    this.remove(child);
    for (var j = i; j < this.items.length; j++) {
      this.items[j].position.top--;
    }
    if (i === this.selected) {
      this.select(i - 1);
    }
  }
  this.emit('remove item');
  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.select"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>select (index)](#apidoc.element.blessed.list.prototype.select)
- description and source-code
```javascript
select = function (index) {
  if (!this.interactive) {
    return;
  }

  if (!this.items.length) {
    this.selected = 0;
    this.value = '';
    this.scrollTo(0);
    return;
  }

  if (typeof index === 'object') {
    index = this.items.indexOf(index);
  }

  if (index < 0) {
    index = 0;
  } else if (index >= this.items.length) {
    index = this.items.length - 1;
  }

  if (this.selected === index && this._listInitialized) return;
  this._listInitialized = true;

  this.selected = index;
  this.value = helpers.cleanTags(this.ritems[this.selected]);
  if (!this.parent) return;
  this.scrollTo(this.selected);

  // XXX Move 'action' and 'select' events here.
  this.emit('select item', this.items[this.selected], this.selected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.setItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>setItem (child, content)](#apidoc.element.blessed.list.prototype.setItem)
- description and source-code
```javascript
setItem = function (child, content) {
  content = typeof content === 'string' ? content : content.getContent();
  var i = this.getItemIndex(child);
  if (!~i) return;
  this.items[i].setContent(content);
  this.ritems[i] = content;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.setItems"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>setItems (items)](#apidoc.element.blessed.list.prototype.setItems)
- description and source-code
```javascript
setItems = function (items) {
  var original = this.items.slice()
    , selected = this.selected
    , sel = this.ritems[this.selected]
    , i = 0;

  items = items.slice();

  this.select(0);

  for (; i < items.length; i++) {
    if (this.items[i]) {
      this.items[i].setContent(items[i]);
    } else {
      this.add(items[i]);
    }
  }

  for (; i < original.length; i++) {
    this.remove(original[i]);
  }

  this.ritems = items;

  // Try to find our old item if it still exists.
  sel = items.indexOf(sel);
  if (~sel) {
    this.select(sel);
  } else if (items.length === original.length) {
    this.select(selected);
  } else {
    this.select(Math.min(selected, items.length - 1));
  }

  this.emit('set items');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.shiftItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>shiftItem ()](#apidoc.element.blessed.list.prototype.shiftItem)
- description and source-code
```javascript
shiftItem = function () {
  return this.removeItem(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.spliceItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>spliceItem (child, n)](#apidoc.element.blessed.list.prototype.spliceItem)
- description and source-code
```javascript
spliceItem = function (child, n) {
  var self = this;
  var i = this.getItemIndex(child);
  if (!~i) return;
  var items = Array.prototype.slice.call(arguments, 2);
  var removed = [];
  while (n--) {
    removed.push(this.removeItem(i));
  }
  items.forEach(function(item) {
    self.insertItem(i++, item);
  });
  return removed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.unshiftItem"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>unshiftItem (content)](#apidoc.element.blessed.list.prototype.unshiftItem)
- description and source-code
```javascript
unshiftItem = function (content) {
  this.insertItem(0, content);
  return this.items.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.list.prototype.up"></a>[function <span class="apidocSignatureSpan">blessed.list.prototype.</span>up (offset)](#apidoc.element.blessed.list.prototype.up)
- description and source-code
```javascript
up = function (offset) {
  this.move(-(offset || 1));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.listbar"></a>[module blessed.listbar](#apidoc.module.blessed.listbar)

#### <a name="apidoc.element.blessed.listbar.listbar"></a>[function <span class="apidocSignatureSpan">blessed.</span>listbar (options)](#apidoc.element.blessed.listbar.listbar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.listbar.prototype"></a>[module blessed.listbar.prototype](#apidoc.module.blessed.listbar.prototype)

#### <a name="apidoc.element.blessed.listbar.prototype.add"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>add (item, callback)](#apidoc.element.blessed.listbar.prototype.add)
- description and source-code
```javascript
add = function (item, callback) {
  var self = this
    , prev = this.items[this.items.length - 1]
    , drawn
    , cmd
    , title
    , len;

  if (!this.parent) {
    drawn = 0;
  } else {
    drawn = prev ? prev.aleft + prev.width : 0;
    if (!this.screen.autoPadding) {
      drawn += this.ileft;
    }
  }

  if (typeof item === 'object') {
    cmd = item;
    if (cmd.prefix == null) cmd.prefix = (this.items.length + 1) + '';
  }

  if (typeof item === 'string') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item,
      callback: callback
    };
  }

  if (typeof item === 'function') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item.name,
      callback: item
    };
  }

  if (cmd.keys && cmd.keys[0]) {
    cmd.prefix = cmd.keys[0];
  }

  var t = helpers.generateTags(this.style.prefix || { fg: 'lightblack' });

  title = (cmd.prefix != null ? t.open + cmd.prefix + t.close + ':' : '') + cmd.text;

  len = ((cmd.prefix != null ? cmd.prefix + ':' : '') + cmd.text).length;

  var options = {
    screen: this.screen,
    top: 0,
    left: drawn + 1,
    height: 1,
    content: title,
    width: len + 2,
    align: 'center',
    autoFocus: false,
    tags: true,
    mouse: true,
    style: helpers.merge({}, this.style.item),
    noOverflow: true
  };

  if (!this.screen.autoPadding) {
    options.top += this.itop;
    options.left += this.ileft;
  }

  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    options.style[name] = function() {
      var attr = self.items[self.selected] === el
        ? self.style.selected[name]
        : self.style.item[name];
      if (typeof attr === 'function') attr = attr(el);
      return attr;
    };
  });

  var el = new Box(options);

  this._[cmd.text] = el;
  cmd.element = el;
  el._.cmd = cmd;

  this.ritems.push(cmd.text);
  this.items.push(el);
  this.commands.push(cmd);
  this.append(el);

  if (cmd.callback) {
    if (cmd.keys) {
      this.screen.key(cmd.keys, function() {
        self.emit('action', el, self.selected);
        self.emit('select', el, self.selected);
        if (el._.cmd.callback) {
          el._.cmd.callback();
        }
        self.select(el);
        self.screen.render();
      });
    }
  }

  if (this.items.length === 1) {
    this.select(0);
  }

  // XXX May be affected by new element.options.mouse option.
  if (this.mouse) {
    el.on('click', function() {
      self.emit('action', el, self.selected);
      self.emit('select', el, self.selected);
      if (el._.cmd.callback) {
        el._.cmd.callback();
      }
      self.select(el);
      self.screen.render();
    });
  }

  this.emit('add item');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.addItem"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>addItem (item, callback)](#apidoc.element.blessed.listbar.prototype.addItem)
- description and source-code
```javascript
addItem = function (item, callback) {
  var self = this
    , prev = this.items[this.items.length - 1]
    , drawn
    , cmd
    , title
    , len;

  if (!this.parent) {
    drawn = 0;
  } else {
    drawn = prev ? prev.aleft + prev.width : 0;
    if (!this.screen.autoPadding) {
      drawn += this.ileft;
    }
  }

  if (typeof item === 'object') {
    cmd = item;
    if (cmd.prefix == null) cmd.prefix = (this.items.length + 1) + '';
  }

  if (typeof item === 'string') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item,
      callback: callback
    };
  }

  if (typeof item === 'function') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item.name,
      callback: item
    };
  }

  if (cmd.keys && cmd.keys[0]) {
    cmd.prefix = cmd.keys[0];
  }

  var t = helpers.generateTags(this.style.prefix || { fg: 'lightblack' });

  title = (cmd.prefix != null ? t.open + cmd.prefix + t.close + ':' : '') + cmd.text;

  len = ((cmd.prefix != null ? cmd.prefix + ':' : '') + cmd.text).length;

  var options = {
    screen: this.screen,
    top: 0,
    left: drawn + 1,
    height: 1,
    content: title,
    width: len + 2,
    align: 'center',
    autoFocus: false,
    tags: true,
    mouse: true,
    style: helpers.merge({}, this.style.item),
    noOverflow: true
  };

  if (!this.screen.autoPadding) {
    options.top += this.itop;
    options.left += this.ileft;
  }

  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    options.style[name] = function() {
      var attr = self.items[self.selected] === el
        ? self.style.selected[name]
        : self.style.item[name];
      if (typeof attr === 'function') attr = attr(el);
      return attr;
    };
  });

  var el = new Box(options);

  this._[cmd.text] = el;
  cmd.element = el;
  el._.cmd = cmd;

  this.ritems.push(cmd.text);
  this.items.push(el);
  this.commands.push(cmd);
  this.append(el);

  if (cmd.callback) {
    if (cmd.keys) {
      this.screen.key(cmd.keys, function() {
        self.emit('action', el, self.selected);
        self.emit('select', el, self.selected);
        if (el._.cmd.callback) {
          el._.cmd.callback();
        }
        self.select(el);
        self.screen.render();
      });
    }
  }

  if (this.items.length === 1) {
    this.select(0);
  }

  // XXX May be affected by new element.options.mouse option.
  if (this.mouse) {
    el.on('click', function() {
      self.emit('action', el, self.selected);
      self.emit('select', el, self.selected);
      if (el._.cmd.callback) {
        el._.cmd.callback();
      }
      self.select(el);
      self.screen.render();
    });
  }

  this.emit('add item');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.appendItem"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>appendItem (item, callback)](#apidoc.element.blessed.listbar.prototype.appendItem)
- description and source-code
```javascript
appendItem = function (item, callback) {
  var self = this
    , prev = this.items[this.items.length - 1]
    , drawn
    , cmd
    , title
    , len;

  if (!this.parent) {
    drawn = 0;
  } else {
    drawn = prev ? prev.aleft + prev.width : 0;
    if (!this.screen.autoPadding) {
      drawn += this.ileft;
    }
  }

  if (typeof item === 'object') {
    cmd = item;
    if (cmd.prefix == null) cmd.prefix = (this.items.length + 1) + '';
  }

  if (typeof item === 'string') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item,
      callback: callback
    };
  }

  if (typeof item === 'function') {
    cmd = {
      prefix: (this.items.length + 1) + '',
      text: item.name,
      callback: item
    };
  }

  if (cmd.keys && cmd.keys[0]) {
    cmd.prefix = cmd.keys[0];
  }

  var t = helpers.generateTags(this.style.prefix || { fg: 'lightblack' });

  title = (cmd.prefix != null ? t.open + cmd.prefix + t.close + ':' : '') + cmd.text;

  len = ((cmd.prefix != null ? cmd.prefix + ':' : '') + cmd.text).length;

  var options = {
    screen: this.screen,
    top: 0,
    left: drawn + 1,
    height: 1,
    content: title,
    width: len + 2,
    align: 'center',
    autoFocus: false,
    tags: true,
    mouse: true,
    style: helpers.merge({}, this.style.item),
    noOverflow: true
  };

  if (!this.screen.autoPadding) {
    options.top += this.itop;
    options.left += this.ileft;
  }

  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    options.style[name] = function() {
      var attr = self.items[self.selected] === el
        ? self.style.selected[name]
        : self.style.item[name];
      if (typeof attr === 'function') attr = attr(el);
      return attr;
    };
  });

  var el = new Box(options);

  this._[cmd.text] = el;
  cmd.element = el;
  el._.cmd = cmd;

  this.ritems.push(cmd.text);
  this.items.push(el);
  this.commands.push(cmd);
  this.append(el);

  if (cmd.callback) {
    if (cmd.keys) {
      this.screen.key(cmd.keys, function() {
        self.emit('action', el, self.selected);
        self.emit('select', el, self.selected);
        if (el._.cmd.callback) {
          el._.cmd.callback();
        }
        self.select(el);
        self.screen.render();
      });
    }
  }

  if (this.items.length === 1) {
    this.select(0);
  }

  // XXX May be affected by new element.options.mouse option.
  if (this.mouse) {
    el.on('click', function() {
      self.emit('action', el, self.selected);
      self.emit('select', el, self.selected);
      if (el._.cmd.callback) {
        el._.cmd.callback();
      }
      self.select(el);
      self.screen.render();
    });
  }

  this.emit('add item');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.move"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>move (offset)](#apidoc.element.blessed.listbar.prototype.move)
- description and source-code
```javascript
move = function (offset) {
  this.select(this.selected + offset);
}
```
- example usage
```shell
...
  program.showCursor();
  program.normalBuffer();
  process.exit(0);
});

program.on('mouse', function(data) {
  if (data.action === 'mousemove') {
    program.move(data.x, data.y);
    program.bg('red');
    program.write('x');
    program.bg('!red');
  }
});

program.alternateBuffer();
...
```

#### <a name="apidoc.element.blessed.listbar.prototype.moveLeft"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>moveLeft (offset)](#apidoc.element.blessed.listbar.prototype.moveLeft)
- description and source-code
```javascript
moveLeft = function (offset) {
  this.move(-(offset || 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.moveRight"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>moveRight (offset)](#apidoc.element.blessed.listbar.prototype.moveRight)
- description and source-code
```javascript
moveRight = function (offset) {
  this.move(offset || 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.removeItem"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>removeItem (child)](#apidoc.element.blessed.listbar.prototype.removeItem)
- description and source-code
```javascript
removeItem = function (child) {
  var i = typeof child !== 'number'
    ? this.items.indexOf(child)
    : child;

  if (~i && this.items[i]) {
    child = this.items.splice(i, 1)[0];
    this.ritems.splice(i, 1);
    this.commands.splice(i, 1);
    this.remove(child);
    if (i === this.selected) {
      this.select(i - 1);
    }
  }

  this.emit('remove item');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>render ()](#apidoc.element.blessed.listbar.prototype.render)
- description and source-code
```javascript
render = function () {
  var self = this
    , drawn = 0;

  if (!this.screen.autoPadding) {
    drawn += this.ileft;
  }

  this.items.forEach(function(el, i) {
    if (i < self.leftBase) {
      el.hide();
    } else {
      el.rleft = drawn + 1;
      drawn += el.width + 2;
      el.show();
    }
  });

  return this._render();
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.listbar.prototype.select"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>select (offset)](#apidoc.element.blessed.listbar.prototype.select)
- description and source-code
```javascript
select = function (offset) {
  if (typeof offset !== 'number') {
    offset = this.items.indexOf(offset);
  }

  if (offset < 0) {
    offset = 0;
  } else if (offset >= this.items.length) {
    offset = this.items.length - 1;
  }

  if (!this.parent) {
    this.emit('select item', this.items[offset], offset);
    return;
  }

  var lpos = this._getCoords();
  if (!lpos) return;

  var self = this
    , width = (lpos.xl - lpos.xi) - this.iwidth
    , drawn = 0
    , visible = 0
    , el;

  el = this.items[offset];
  if (!el) return;

  this.items.forEach(function(el, i) {
    if (i < self.leftBase) return;

    var lpos = el._getCoords();
    if (!lpos) return;

    if (lpos.xl - lpos.xi <= 0) return;

    drawn += (lpos.xl - lpos.xi) + 2;

    if (drawn <= width) visible++;
  });

  var diff = offset - (this.leftBase + this.leftOffset);
  if (offset > this.leftBase + this.leftOffset) {
    if (offset > this.leftBase + visible - 1) {
      this.leftOffset = 0;
      this.leftBase = offset;
    } else {
      this.leftOffset += diff;
    }
  } else if (offset < this.leftBase + this.leftOffset) {
    diff = -diff;
    if (offset < this.leftBase) {
      this.leftOffset = 0;
      this.leftBase = offset;
    } else {
      this.leftOffset -= diff;
    }
  }

  // XXX Move 'action' and 'select' events here.
  this.emit('select item', el, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.selectTab"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>selectTab (index)](#apidoc.element.blessed.listbar.prototype.selectTab)
- description and source-code
```javascript
selectTab = function (index) {
  var item = this.items[index];
  if (item) {
    if (item._.cmd.callback) {
      item._.cmd.callback();
    }
    this.select(index);
    this.screen.render();
  }
  this.emit('select tab', item, index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listbar.prototype.setItems"></a>[function <span class="apidocSignatureSpan">blessed.listbar.prototype.</span>setItems (commands)](#apidoc.element.blessed.listbar.prototype.setItems)
- description and source-code
```javascript
setItems = function (commands) {
  var self = this;

  if (!Array.isArray(commands)) {
    commands = Object.keys(commands).reduce(function(obj, key, i) {
      var cmd = commands[key]
        , cb;

      if (typeof cmd === 'function') {
        cb = cmd;
        cmd = { callback: cb };
      }

      if (cmd.text == null) cmd.text = key;
      if (cmd.prefix == null) cmd.prefix = ++i + '';

      if (cmd.text == null && cmd.callback) {
        cmd.text = cmd.callback.name;
      }

      obj.push(cmd);

      return obj;
    }, []);
  }

  this.items.forEach(function(el) {
    el.detach();
  });

  this.items = [];
  this.ritems = [];
  this.commands = [];

  commands.forEach(function(cmd) {
    self.add(cmd);
  });

  this.emit('set items');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.listtable"></a>[module blessed.listtable](#apidoc.module.blessed.listtable)

#### <a name="apidoc.element.blessed.listtable.listtable"></a>[function <span class="apidocSignatureSpan">blessed.</span>listtable (options)](#apidoc.element.blessed.listtable.listtable)
- description and source-code
```javascript
function ListTable(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ListTable(options);
  }

  options = options || {};
  options.shrink = true;
  options.normalShrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  this.__align = options.align || 'center';
  delete options.align;

  options.style.selected = options.style.cell.selected;
  options.style.item = options.style.cell;

  List.call(this, options);

  this._header = new Box({
    parent: this,
    left: this.screen.autoPadding ? 0 : this.ileft,
    top: 0,
    width: 'shrink',
    height: 1,
    style: options.style.header,
    tags: options.parseTags || options.tags
  });

  this.on('scroll', function() {
    self._header.setFront();
    self._header.rtop = self.childBase;
    if (!self.screen.autoPadding) {
      self._header.rtop = self.childBase + (self.border ? 1 : 0);
    }
  });

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setData(self.rows);
  });

  this.on('resize', function() {
    var selected = self.selected;
    self.setData(self.rows);
    self.select(selected);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.listtable.prototype"></a>[module blessed.listtable.prototype](#apidoc.module.blessed.listtable.prototype)

#### <a name="apidoc.element.blessed.listtable.prototype._calculateMaxes"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>_calculateMaxes ()](#apidoc.element.blessed.listtable.prototype._calculateMaxes)
- description and source-code
```javascript
_calculateMaxes = function () {
  var self = this;
  var maxes = [];

  if (this.detached) return;

  this.rows = this.rows || [];

  this.rows.forEach(function(row) {
    row.forEach(function(cell, i) {
      var clen = self.strWidth(cell);
      if (!maxes[i] || maxes[i] < clen) {
        maxes[i] = clen;
      }
    });
  });

  var total = maxes.reduce(function(total, max) {
    return total + max;
  }, 0);
  total += maxes.length + 1;

  // XXX There might be an issue with resizing where on the first resize event
  // width appears to be less than total if it's a percentage or left/right
  // combination.
  if (this.width < total) {
    delete this.position.width;
  }

  if (this.position.width != null) {
    var missing = this.width - total;
    var w = missing / maxes.length | 0;
    var wr = missing % maxes.length;
    maxes = maxes.map(function(max, i) {
      if (i === maxes.length - 1) {
        return max + w + wr;
      }
      return max + w;
    });
  } else {
    maxes = maxes.map(function(max) {
      return max + self.pad;
    });
  }

  return this._maxes = maxes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listtable.prototype._select"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>_select (index)](#apidoc.element.blessed.listtable.prototype._select)
- description and source-code
```javascript
_select = function (index) {
  if (!this.interactive) {
    return;
  }

  if (!this.items.length) {
    this.selected = 0;
    this.value = '';
    this.scrollTo(0);
    return;
  }

  if (typeof index === 'object') {
    index = this.items.indexOf(index);
  }

  if (index < 0) {
    index = 0;
  } else if (index >= this.items.length) {
    index = this.items.length - 1;
  }

  if (this.selected === index && this._listInitialized) return;
  this._listInitialized = true;

  this.selected = index;
  this.value = helpers.cleanTags(this.ritems[this.selected]);
  if (!this.parent) return;
  this.scrollTo(this.selected);

  // XXX Move 'action' and 'select' events here.
  this.emit('select item', this.items[this.selected], this.selected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listtable.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>render ()](#apidoc.element.blessed.listtable.prototype.render)
- description and source-code
```javascript
render = function () {
  var self = this;

  var coords = this._render();
  if (!coords) return;

  this._calculateMaxes();

  if (!this._maxes) return coords;

  var lines = this.screen.lines
    , xi = coords.xi
    , yi = coords.yi
    , rx
    , ry
    , i;

  var battr = this.sattr(this.style.border);

  var height = coords.yl - coords.yi - this.ibottom;

  if (!this.border || this.options.noCellBorders) return coords;

  // Draw border with correct angles.
  ry = 0;
  for (i = 0; i < height + 1; i++) {
    if (!lines[yi + ry]) break;
    rx = 0;
    self._maxes.slice(0, -1).forEach(function(max) {
      rx += max;
      if (!lines[yi + ry][xi + rx + 1]) return;
      // center
      if (ry === 0) {
        // top
        rx++;
        lines[yi + ry][xi + rx][0] = battr;
        lines[yi + ry][xi + rx][1] = '\u252c'; // '┬'
        // XXX If we alter iheight and itop for no borders - nothing should be written here
        if (!self.border.top) {
          lines[yi + ry][xi + rx][1] = '\u2502'; // '│'
        }
        lines[yi + ry].dirty = true;
      } else if (ry === height) {
        // bottom
        rx++;
        lines[yi + ry][xi + rx][0] = battr;
        lines[yi + ry][xi + rx][1] = '\u2534'; // '┴'
        // XXX If we alter iheight and ibottom for no borders - nothing should be written here
        if (!self.border.bottom) {
          lines[yi + ry][xi + rx][1] = '\u2502'; // '│'
        }
        lines[yi + ry].dirty = true;
      } else {
        // middle
        rx++;
      }
    });
    ry += 1;
  }

  // Draw internal borders.
  for (ry = 1; ry < height; ry++) {
    if (!lines[yi + ry]) break;
    rx = 0;
    self._maxes.slice(0, -1).forEach(function(max) {
      rx += max;
      if (!lines[yi + ry][xi + rx + 1]) return;
      if (self.options.fillCellBorders !== false) {
        var lbg = lines[yi + ry][xi + rx][0] & 0x1ff;
        rx++;
        lines[yi + ry][xi + rx][0] = (battr & ~0x1ff) | lbg;
      } else {
        rx++;
        lines[yi + ry][xi + rx][0] = battr;
      }
      lines[yi + ry][xi + rx][1] = '\u2502'; // '│'
      lines[yi + ry].dirty = true;
    });
  }

  return coords;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.listtable.prototype.select"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>select (i)](#apidoc.element.blessed.listtable.prototype.select)
- description and source-code
```javascript
select = function (i) {
  if (i === 0) {
    i = 1;
  }
  if (i <= this.childBase) {
    this.setScroll(this.childBase - 1);
  }
  return this._select(i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.listtable.prototype.setData"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>setData (rows)](#apidoc.element.blessed.listtable.prototype.setData)
- description and source-code
```javascript
setData = function (rows) {
  var self = this
    , align = this.__align;

  if (this.visible && this.lpos) {
    this.clearPos();
  }

  this.clearItems();

  this.rows = rows || [];

  this._calculateMaxes();

  if (!this._maxes) return;

  this.addItem('');

  this.rows.forEach(function(row, i) {
    var isHeader = i === 0;
    var text = '';
    row.forEach(function(cell, i) {
      var width = self._maxes[i];
      var clen = self.strWidth(cell);

      if (i !== 0) {
        text += ' ';
      }

      while (clen < width) {
        if (align === 'center') {
          cell = ' ' + cell + ' ';
          clen += 2;
        } else if (align === 'left') {
          cell = cell + ' ';
          clen += 1;
        } else if (align === 'right') {
          cell = ' ' + cell;
          clen += 1;
        }
      }

      if (clen > width) {
        if (align === 'center') {
          cell = cell.substring(1);
          clen--;
        } else if (align === 'left') {
          cell = cell.slice(0, -1);
          clen--;
        } else if (align === 'right') {
          cell = cell.substring(1);
          clen--;
        }
      }

      text += cell;
    });
    if (isHeader) {
      self._header.setContent(text);
    } else {
      self.addItem(text);
    }
  });

  this._header.setFront();

  this.select(0);
}
```
- example usage
```shell
...
- Inherits all from List.

##### Methods:

- Inherits all from List.
- __setRows/setData(rows)__ - Set rows in table. Array of arrays of strings.
''' js
  table.setData([
    [ 'Animals',  'Foods'  ],
    [ 'Elephant', 'Apple'  ],
    [ 'Bird',     'Orange' ]
  ]);
'''
...
```

#### <a name="apidoc.element.blessed.listtable.prototype.setRows"></a>[function <span class="apidocSignatureSpan">blessed.listtable.prototype.</span>setRows (rows)](#apidoc.element.blessed.listtable.prototype.setRows)
- description and source-code
```javascript
setRows = function (rows) {
  var self = this
    , align = this.__align;

  if (this.visible && this.lpos) {
    this.clearPos();
  }

  this.clearItems();

  this.rows = rows || [];

  this._calculateMaxes();

  if (!this._maxes) return;

  this.addItem('');

  this.rows.forEach(function(row, i) {
    var isHeader = i === 0;
    var text = '';
    row.forEach(function(cell, i) {
      var width = self._maxes[i];
      var clen = self.strWidth(cell);

      if (i !== 0) {
        text += ' ';
      }

      while (clen < width) {
        if (align === 'center') {
          cell = ' ' + cell + ' ';
          clen += 2;
        } else if (align === 'left') {
          cell = cell + ' ';
          clen += 1;
        } else if (align === 'right') {
          cell = ' ' + cell;
          clen += 1;
        }
      }

      if (clen > width) {
        if (align === 'center') {
          cell = cell.substring(1);
          clen--;
        } else if (align === 'left') {
          cell = cell.slice(0, -1);
          clen--;
        } else if (align === 'right') {
          cell = cell.substring(1);
          clen--;
        }
      }

      text += cell;
    });
    if (isHeader) {
      self._header.setContent(text);
    } else {
      self.addItem(text);
    }
  });

  this._header.setFront();

  this.select(0);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.loading"></a>[module blessed.loading](#apidoc.module.blessed.loading)

#### <a name="apidoc.element.blessed.loading.loading"></a>[function <span class="apidocSignatureSpan">blessed.</span>loading (options)](#apidoc.element.blessed.loading.loading)
- description and source-code
```javascript
function Loading(options) {
  if (!(this instanceof Node)) {
    return new Loading(options);
  }

  options = options || {};

  Box.call(this, options);

  this._.icon = new Text({
    parent: this,
    align: 'center',
    top: 2,
    left: 1,
    right: 1,
    height: 1,
    content: '|'
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.loading.prototype"></a>[module blessed.loading.prototype](#apidoc.module.blessed.loading.prototype)

#### <a name="apidoc.element.blessed.loading.prototype.load"></a>[function <span class="apidocSignatureSpan">blessed.loading.prototype.</span>load (text)](#apidoc.element.blessed.loading.prototype.load)
- description and source-code
```javascript
load = function (text) {
  var self = this;

  // XXX Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.show();
  this.setContent(text);

  if (this._.timer) {
    this.stop();
  }

  this.screen.lockKeys = true;

  this._.timer = setInterval(function() {
    if (self._.icon.content === '|') {
      self._.icon.setContent('/');
    } else if (self._.icon.content === '/') {
      self._.icon.setContent('-');
    } else if (self._.icon.content === '-') {
      self._.icon.setContent('\\');
    } else if (self._.icon.content === '\\') {
      self._.icon.setContent('|');
    }
    self.screen.render();
  }, 200);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.loading.prototype.stop"></a>[function <span class="apidocSignatureSpan">blessed.loading.prototype.</span>stop ()](#apidoc.element.blessed.loading.prototype.stop)
- description and source-code
```javascript
stop = function () {
  this.screen.lockKeys = false;
  this.hide();
  if (this._.timer) {
    clearInterval(this._.timer);
    delete this._.timer;
  }
  this.screen.render();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.log"></a>[module blessed.log](#apidoc.module.blessed.log)

#### <a name="apidoc.element.blessed.log.log"></a>[function <span class="apidocSignatureSpan">blessed.</span>log (options)](#apidoc.element.blessed.log.log)
- description and source-code
```javascript
function Log(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Log(options);
  }

  options = options || {};

  ScrollableText.call(this, options);

  this.scrollback = options.scrollback != null
    ? options.scrollback
    : Infinity;
  this.scrollOnInput = options.scrollOnInput;

  this.on('set content', function() {
    if (!self._userScrolled || self.scrollOnInput) {
      nextTick(function() {
        self.setScrollPerc(100);
        self._userScrolled = false;
        self.screen.render();
      });
    }
  });
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```



# <a name="apidoc.module.blessed.log.prototype"></a>[module blessed.log.prototype](#apidoc.module.blessed.log.prototype)

#### <a name="apidoc.element.blessed.log.prototype._scroll"></a>[function <span class="apidocSignatureSpan">blessed.log.prototype.</span>_scroll (offset, always)](#apidoc.element.blessed.log.prototype._scroll)
- description and source-code
```javascript
_scroll = function (offset, always) {
  if (!this.scrollable) return;

  if (this.detached) return;

  // Handle scrolling.
  var visible = this.height - this.iheight
    , base = this.childBase
    , d
    , p
    , t
    , b
    , max
    , emax;

  if (this.alwaysScroll || always) {
    // Semi-workaround
    this.childOffset = offset > 0
      ? visible - 1 + offset
      : offset;
  } else {
    this.childOffset += offset;
  }

  if (this.childOffset > visible - 1) {
    d = this.childOffset - (visible - 1);
    this.childOffset -= d;
    this.childBase += d;
  } else if (this.childOffset < 0) {
    d = this.childOffset;
    this.childOffset += -d;
    this.childBase += d;
  }

  if (this.childBase < 0) {
    this.childBase = 0;
  } else if (this.childBase > this.baseLimit) {
    this.childBase = this.baseLimit;
  }

  // Find max "bottom" value for
  // content and descendant elements.
  // Scroll the content if necessary.
  if (this.childBase === base) {
    return this.emit('scroll');
  }

  // When scrolling text, we want to be able to handle SGR codes as well as line
  // feeds. This allows us to take preformatted text output from other programs
  // and put it in a scrollable text box.
  this.parseContent();

  // XXX
  // max = this.getScrollHeight() - (this.height - this.iheight);

  max = this._clines.length - (this.height - this.iheight);
  if (max < 0) max = 0;
  emax = this._scrollBottom() - (this.height - this.iheight);
  if (emax < 0) emax = 0;

  this.childBase = Math.min(this.childBase, Math.max(emax, max));

  if (this.childBase < 0) {
    this.childBase = 0;
  } else if (this.childBase > this.baseLimit) {
    this.childBase = this.baseLimit;
  }

  // Optimize scrolling with CSR + IL/DL.
  p = this.lpos;
  // Only really need _getCoords() if we want
  // to allow nestable scrolling elements...
  // or if we **really** want shrinkable
  // scrolling elements.
  // p = this._getCoords();
  if (p && this.childBase !== base && this.screen.cleanSides(this)) {
    t = p.yi + this.itop;
    b = p.yl - this.ibottom - 1;
    d = this.childBase - base;

    if (d > 0 && d < visible) {
      // scrolled down
      this.screen.deleteLine(d, t, t, b);
    } else if (d < 0 && -d < visible) {
      // scrolled up
      d = -d;
      this.screen.insertLine(d, t, t, b);
    }
  }

  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.log.prototype.add"></a>[function <span class="apidocSignatureSpan">blessed.log.prototype.</span>add ()](#apidoc.element.blessed.log.prototype.add)
- description and source-code
```javascript
add = function () {
  var args = Array.prototype.slice.call(arguments);
  if (typeof args[0] === 'object') {
    args[0] = util.inspect(args[0], true, 20, true);
  }
  var text = util.format.apply(util, args);
  this.emit('log', text);
  var ret = this.pushLine(text);
  if (this._clines.fake.length > this.scrollback) {
    this.shiftLine(0, (this.scrollback / 3) | 0);
  }
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.log.prototype.log"></a>[function <span class="apidocSignatureSpan">blessed.log.prototype.</span>log ()](#apidoc.element.blessed.log.prototype.log)
- description and source-code
```javascript
log = function () {
  var args = Array.prototype.slice.call(arguments);
  if (typeof args[0] === 'object') {
    args[0] = util.inspect(args[0], true, 20, true);
  }
  var text = util.format.apply(util, args);
  this.emit('log', text);
  var ret = this.pushLine(text);
  if (this._clines.fake.length > this.scrollback) {
    this.shiftLine(0, (this.scrollback / 3) | 0);
  }
  return ret;
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```

#### <a name="apidoc.element.blessed.log.prototype.scroll"></a>[function <span class="apidocSignatureSpan">blessed.log.prototype.</span>scroll (offset, always)](#apidoc.element.blessed.log.prototype.scroll)
- description and source-code
```javascript
scroll = function (offset, always) {
  if (offset === 0) return this._scroll(offset, always);
  this._userScrolled = true;
  var ret = this._scroll(offset, always);
  if (this.getScrollPerc() === 100) {
    this._userScrolled = false;
  }
  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.message"></a>[module blessed.message](#apidoc.module.blessed.message)

#### <a name="apidoc.element.blessed.message.message"></a>[function <span class="apidocSignatureSpan">blessed.</span>message (options)](#apidoc.element.blessed.message.message)
- description and source-code
```javascript
function Message(options) {
  if (!(this instanceof Node)) {
    return new Message(options);
  }

  options = options || {};
  options.tags = true;

  Box.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.message.prototype"></a>[module blessed.message.prototype](#apidoc.module.blessed.message.prototype)

#### <a name="apidoc.element.blessed.message.prototype.display"></a>[function <span class="apidocSignatureSpan">blessed.message.prototype.</span>display (text, time, callback)](#apidoc.element.blessed.message.prototype.display)
- description and source-code
```javascript
display = function (text, time, callback) {
  var self = this;

  if (typeof time === 'function') {
    callback = time;
    time = null;
  }

  if (time == null) time = 3;

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  if (this.scrollable) {
    this.screen.saveFocus();
    this.focus();
    this.scrollTo(0);
  }

  this.show();
  this.setContent(text);
  this.screen.render();

  if (time === Infinity || time === -1 || time === 0) {
    var end = function() {
      if (end.done) return;
      end.done = true;
      if (self.scrollable) {
        try {
          self.screen.restoreFocus();
        } catch (e) {
          ;
        }
      }
      self.hide();
      self.screen.render();
      if (callback) callback();
    };

    setTimeout(function() {
      self.onScreenEvent('keypress', function fn(ch, key) {
        if (key.name === 'mouse') return;
        if (self.scrollable) {
          if ((key.name === 'up' || (self.options.vi && key.name === 'k'))
            || (key.name === 'down' || (self.options.vi && key.name === 'j'))
            || (self.options.vi && key.name === 'u' && key.ctrl)
            || (self.options.vi && key.name === 'd' && key.ctrl)
            || (self.options.vi && key.name === 'b' && key.ctrl)
            || (self.options.vi && key.name === 'f' && key.ctrl)
            || (self.options.vi && key.name === 'g' && !key.shift)
            || (self.options.vi && key.name === 'g' && key.shift)) {
            return;
          }
        }
        if (self.options.ignoreKeys && ~self.options.ignoreKeys.indexOf(key.name)) {
          return;
        }
        self.removeScreenEvent('keypress', fn);
        end();
      });
      // XXX May be affected by new element.options.mouse option.
      if (!self.options.mouse) return;
      self.onScreenEvent('mouse', function fn(data) {
        if (data.action === 'mousemove') return;
        self.removeScreenEvent('mouse', fn);
        end();
      });
    }, 10);

    return;
  }

  setTimeout(function() {
    self.hide();
    self.screen.render();
    if (callback) callback();
  }, time * 1000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.message.prototype.error"></a>[function <span class="apidocSignatureSpan">blessed.message.prototype.</span>error (text, time, callback)](#apidoc.element.blessed.message.prototype.error)
- description and source-code
```javascript
error = function (text, time, callback) {
  return this.display('{red-fg}Error: ' + text + '{/red-fg}', time, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.message.prototype.log"></a>[function <span class="apidocSignatureSpan">blessed.message.prototype.</span>log (text, time, callback)](#apidoc.element.blessed.message.prototype.log)
- description and source-code
```javascript
log = function (text, time, callback) {
  var self = this;

  if (typeof time === 'function') {
    callback = time;
    time = null;
  }

  if (time == null) time = 3;

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  if (this.scrollable) {
    this.screen.saveFocus();
    this.focus();
    this.scrollTo(0);
  }

  this.show();
  this.setContent(text);
  this.screen.render();

  if (time === Infinity || time === -1 || time === 0) {
    var end = function() {
      if (end.done) return;
      end.done = true;
      if (self.scrollable) {
        try {
          self.screen.restoreFocus();
        } catch (e) {
          ;
        }
      }
      self.hide();
      self.screen.render();
      if (callback) callback();
    };

    setTimeout(function() {
      self.onScreenEvent('keypress', function fn(ch, key) {
        if (key.name === 'mouse') return;
        if (self.scrollable) {
          if ((key.name === 'up' || (self.options.vi && key.name === 'k'))
            || (key.name === 'down' || (self.options.vi && key.name === 'j'))
            || (self.options.vi && key.name === 'u' && key.ctrl)
            || (self.options.vi && key.name === 'd' && key.ctrl)
            || (self.options.vi && key.name === 'b' && key.ctrl)
            || (self.options.vi && key.name === 'f' && key.ctrl)
            || (self.options.vi && key.name === 'g' && !key.shift)
            || (self.options.vi && key.name === 'g' && key.shift)) {
            return;
          }
        }
        if (self.options.ignoreKeys && ~self.options.ignoreKeys.indexOf(key.name)) {
          return;
        }
        self.removeScreenEvent('keypress', fn);
        end();
      });
      // XXX May be affected by new element.options.mouse option.
      if (!self.options.mouse) return;
      self.onScreenEvent('mouse', function fn(data) {
        if (data.action === 'mousemove') return;
        self.removeScreenEvent('mouse', fn);
        end();
      });
    }, 10);

    return;
  }

  setTimeout(function() {
    self.hide();
    self.screen.render();
    if (callback) callback();
  }, time * 1000);
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```



# <a name="apidoc.module.blessed.node"></a>[module blessed.node](#apidoc.module.blessed.node)

#### <a name="apidoc.element.blessed.node.node"></a>[function <span class="apidocSignatureSpan">blessed.</span>node (options)](#apidoc.element.blessed.node.node)
- description and source-code
```javascript
function Node(options) {
  var self = this;
  var Screen = require('./screen');

  if (!(this instanceof Node)) {
    return new Node(options);
  }

  EventEmitter.call(this);

  options = options || {};
  this.options = options;

  this.screen = this.screen || options.screen;

  if (!this.screen) {
    if (this.type === 'screen') {
      this.screen = this;
    } else if (Screen.total === 1) {
      this.screen = Screen.global;
    } else if (options.parent) {
      this.screen = options.parent;
      while (this.screen && this.screen.type !== 'screen') {
        this.screen = this.screen.parent;
      }
    } else if (Screen.total) {
      // This _should_ work in most cases as long as the element is appended
      // synchronously after the screen's creation. Throw error if not.
      this.screen = Screen.instances[Screen.instances.length - 1];
      process.nextTick(function() {
        if (!self.parent) {
          throw new Error('Element (' + self.type + ')'
            + ' was not appended synchronously after the'
            + ' screen\'s creation. Please set a 'parent''
            + ' or 'screen' option in the element\'s constructor'
            + ' if you are going to use multiple screens and'
            + ' append the element later.');
        }
      });
    } else {
      throw new Error('No active screen.');
    }
  }

  this.parent = options.parent || null;
  this.children = [];
  this.$ = this._ = this.data = {};
  this.uid = Node.uid++;
  this.index = this.index != null ? this.index : -1;

  if (this.type !== 'screen') {
    this.detached = true;
  }

  if (this.parent) {
    this.parent.append(this);
  }

  (options.children || []).forEach(this.append.bind(this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.node.prototype"></a>[module blessed.node.prototype](#apidoc.module.blessed.node.prototype)

#### <a name="apidoc.element.blessed.node.prototype.append"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>append (element)](#apidoc.element.blessed.node.prototype.append)
- description and source-code
```javascript
append = function (element) {
  this.insert(element, this.children.length);
}
```
- example usage
```shell
...
  hover: {
    bg: 'green'
  }
}
});

// Append our box to the screen.
screen.append(box);

// Add a png icon to the box
var icon = blessed.image({
parent: box,
top: 0,
left: 0,
type: 'overlay',
...
```

#### <a name="apidoc.element.blessed.node.prototype.collectAncestors"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>collectAncestors (s)](#apidoc.element.blessed.node.prototype.collectAncestors)
- description and source-code
```javascript
collectAncestors = function (s) {
  var out = [];
  this.forAncestors(function(el) {
    out.push(el);
  }, s);
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.collectDescendants"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>collectDescendants (s)](#apidoc.element.blessed.node.prototype.collectDescendants)
- description and source-code
```javascript
collectDescendants = function (s) {
  var out = [];
  this.forDescendants(function(el) {
    out.push(el);
  }, s);
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.destroy"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>destroy ()](#apidoc.element.blessed.node.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.detach();
  this.forDescendants(function(el) {
    el.free();
    el.destroyed = true;
    el.emit('destroy');
  }, this);
}
```
- example usage
```shell
...
  output: client,
  terminal: 'xterm-256color',
  fullUnicode: true
});

client.on('close', function() {
  if (!screen.destroyed) {
    screen.destroy();
  }
});

screen.key(['C-c', 'q'], function(ch, key) {
  screen.destroy();
});
...
```

#### <a name="apidoc.element.blessed.node.prototype.detach"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>detach ()](#apidoc.element.blessed.node.prototype.detach)
- description and source-code
```javascript
detach = function () {
  if (this.parent) this.parent.remove(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.emitAncestors"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>emitAncestors ()](#apidoc.element.blessed.node.prototype.emitAncestors)
- description and source-code
```javascript
emitAncestors = function () {
  var args = Array.prototype.slice(arguments)
    , iter;

  if (typeof args[args.length - 1] === 'function') {
    iter = args.pop();
  }

  return this.forAncestors(function(el) {
    if (iter) iter(el);
    el.emit.apply(el, args);
  }, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.emitDescendants"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>emitDescendants ()](#apidoc.element.blessed.node.prototype.emitDescendants)
- description and source-code
```javascript
emitDescendants = function () {
  var args = Array.prototype.slice(arguments)
    , iter;

  if (typeof args[args.length - 1] === 'function') {
    iter = args.pop();
  }

  return this.forDescendants(function(el) {
    if (iter) iter(el);
    el.emit.apply(el, args);
  }, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.forAncestors"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>forAncestors (iter, s)](#apidoc.element.blessed.node.prototype.forAncestors)
- description and source-code
```javascript
forAncestors = function (iter, s) {
  var el = this;
  if (s) iter(this);
  while (el = el.parent) {
    iter(el);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.forDescendants"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>forDescendants (iter, s)](#apidoc.element.blessed.node.prototype.forDescendants)
- description and source-code
```javascript
forDescendants = function (iter, s) {
  if (s) iter(this);
  this.children.forEach(function emit(el) {
    iter(el);
    el.children.forEach(emit);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.free"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>free ()](#apidoc.element.blessed.node.prototype.free)
- description and source-code
```javascript
free = function () {
  return;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.get"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>get (name, value)](#apidoc.element.blessed.node.prototype.get)
- description and source-code
```javascript
get = function (name, value) {
  if (this.data.hasOwnProperty(name)) {
    return this.data[name];
  }
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.hasAncestor"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>hasAncestor (target)](#apidoc.element.blessed.node.prototype.hasAncestor)
- description and source-code
```javascript
hasAncestor = function (target) {
  var el = this;
  while (el = el.parent) {
    if (el === target) return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.hasDescendant"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>hasDescendant (target)](#apidoc.element.blessed.node.prototype.hasDescendant)
- description and source-code
```javascript
hasDescendant = function (target) {
  return (function find(el) {
    for (var i = 0; i < el.children.length; i++) {
      if (el.children[i] === target) {
        return true;
      }
      if (find(el.children[i]) === true) {
        return true;
      }
    }
    return false;
  })(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.insert"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insert (element, i)](#apidoc.element.blessed.node.prototype.insert)
- description and source-code
```javascript
insert = function (element, i) {
  var self = this;

  if (element.screen && element.screen !== this.screen) {
    throw new Error('Cannot switch a node\'s screen.');
  }

  element.detach();
  element.parent = this;
  element.screen = this.screen;

  if (i === 0) {
    this.children.unshift(element);
  } else if (i === this.children.length) {
    this.children.push(element);
  } else {
    this.children.splice(i, 0, element);
  }

  element.emit('reparent', this);
  this.emit('adopt', element);

  (function emit(el) {
    var n = el.detached !== self.detached;
    el.detached = self.detached;
    if (n) el.emit('attach');
    el.children.forEach(emit);
  })(element);

  if (!this.screen.focused) {
    this.screen.focused = element;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.insertAfter"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insertAfter (element, other)](#apidoc.element.blessed.node.prototype.insertAfter)
- description and source-code
```javascript
insertAfter = function (element, other) {
  var i = this.children.indexOf(other);
  if (~i) this.insert(element, i + 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.insertBefore"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>insertBefore (element, other)](#apidoc.element.blessed.node.prototype.insertBefore)
- description and source-code
```javascript
insertBefore = function (element, other) {
  var i = this.children.indexOf(other);
  if (~i) this.insert(element, i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.prepend"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>prepend (element)](#apidoc.element.blessed.node.prototype.prepend)
- description and source-code
```javascript
prepend = function (element) {
  this.insert(element, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.remove"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>remove (element)](#apidoc.element.blessed.node.prototype.remove)
- description and source-code
```javascript
remove = function (element) {
  if (element.parent !== this) return;

  var i = this.children.indexOf(element);
  if (!~i) return;

  element.clearPos();

  element.parent = null;

  this.children.splice(i, 1);

  i = this.screen.clickable.indexOf(element);
  if (~i) this.screen.clickable.splice(i, 1);
  i = this.screen.keyable.indexOf(element);
  if (~i) this.screen.keyable.splice(i, 1);

  element.emit('reparent', null);
  this.emit('remove', element);

  (function emit(el) {
    var n = el.detached !== true;
    el.detached = true;
    if (n) el.emit('detach');
    el.children.forEach(emit);
  })(element);

  if (this.screen.focused === element) {
    this.screen.rewindFocus();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.node.prototype.set"></a>[function <span class="apidocSignatureSpan">blessed.node.prototype.</span>set (name, value)](#apidoc.element.blessed.node.prototype.set)
- description and source-code
```javascript
set = function (name, value) {
  return this.data[name] = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.overlayimage"></a>[module blessed.overlayimage](#apidoc.module.blessed.overlayimage)

#### <a name="apidoc.element.blessed.overlayimage.overlayimage"></a>[function <span class="apidocSignatureSpan">blessed.</span>overlayimage (options)](#apidoc.element.blessed.overlayimage.overlayimage)
- description and source-code
```javascript
function OverlayImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new OverlayImage(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.w3m) {
    OverlayImage.w3mdisplay = options.w3m;
  }

  if (OverlayImage.hasW3MDisplay == null) {
    if (fs.existsSync(OverlayImage.w3mdisplay)) {
      OverlayImage.hasW3MDisplay = true;
    } else if (options.search !== false) {
      var file = helpers.findFile('/usr', 'w3mimgdisplay')
              || helpers.findFile('/lib', 'w3mimgdisplay')
              || helpers.findFile('/bin', 'w3mimgdisplay');
      if (file) {
        OverlayImage.hasW3MDisplay = true;
        OverlayImage.w3mdisplay = file;
      } else {
        OverlayImage.hasW3MDisplay = false;
      }
    }
  }

  this.on('hide', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('show', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.on('detach', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('attach', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.onScreenEvent('resize', function() {
    self._needsRatio = true;
  });

  // Get images to overlap properly. Maybe not worth it:
  // this.onScreenEvent('render', function() {
  //   self.screen.program.flush();
  //   if (!self._noImage) return;
  //   function display(el, next) {
  //     if (el.type === 'w3mimage' && el.file) {
  //       el.setImage(el.file, next);
  //     } else {
  //       next();
  //     }
  //   }
  //   function done(el) {
  //     el.children.forEach(recurse);
  //   }
  //   function recurse(el) {
  //     display(el, function() {
  //       var pending = el.children.length;
  //       el.children.forEach(function(el) {
  //         display(el, function() {
  //           if (!--pending) done(el);
  //         });
  //       });
  //     });
  //   }
  //   recurse(self.screen);
  // });

  this.onScreenEvent('render', function() {
    self.screen.program.flush();
    if (!self._noImage) {
      self.setImage(self.file);
    }
  });

  if (this.options.file || this.options.img) {
    this.setImage(this.options.file || this.options.img);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.overlayimage.prototype"></a>[module blessed.overlayimage.prototype](#apidoc.module.blessed.overlayimage.prototype)

#### <a name="apidoc.element.blessed.overlayimage.prototype.clearImage"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>clearImage (callback)](#apidoc.element.blessed.overlayimage.prototype.clearImage)
- description and source-code
```javascript
clearImage = function (callback) {
  if (cp.execSync) {
    callback = callback || function(err, result) { return result; };
    try {
      return callback(null, this.clearImageSync());
    } catch (e) {
      return callback(e);
    }
  }

  if (OverlayImage.hasW3MDisplay === false) {
    if (!callback) return;
    return callback(new Error('W3M Image Display not available.'));
  }

  if (!this._props) {
    if (!callback) return;
    return callback(null);
  }

  var opt = {
    stdio: 'pipe',
    env: process.env,
    cwd: process.env.HOME
  };

  var ps = this.spawn(OverlayImage.w3mdisplay, [], opt, function(err, success) {
    if (!callback) return;
    return err
      ? callback(err)
      : callback(null, success);
  });

  var width = this._props.width + 2
    , height = this._props.height + 2
    , aleft = this._props.aleft
    , atop = this._props.atop;

  if (this._drag) {
    aleft -= 10;
    atop -= 10;
    width += 10;
    height += 10;
  }

  var input = '6;'
   + aleft + ';'
   + atop + ';'
   + width + ';'
   + height
   + '\n4;\n3;\n';

  delete this.file;
  delete this._props;
  delete this._lastSize;

  ps.stdin.write(input);
  ps.stdin.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.clearImageSync"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>clearImageSync ()](#apidoc.element.blessed.overlayimage.prototype.clearImageSync)
- description and source-code
```javascript
clearImageSync = function () {
  if (OverlayImage.hasW3MDisplay === false) {
    throw new Error('W3M Image Display not available.');
  }

  if (!this._props) {
    return false;
  }

  var width = this._props.width + 2
    , height = this._props.height + 2
    , aleft = this._props.aleft
    , atop = this._props.atop;

  if (this._drag) {
    aleft -= 10;
    atop -= 10;
    width += 10;
    height += 10;
  }

  var input = '6;'
   + aleft + ';'
   + atop + ';'
   + width + ';'
   + height
   + '\n4;\n3;\n';

  delete this.file;
  delete this._props;
  delete this._lastSize;

  try {
    cp.execFileSync(OverlayImage.w3mdisplay, [], {
      env: process.env,
      encoding: 'utf8',
      input: input,
      timeout: 1000
    });
  } catch (e) {
    ;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.displayImage"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>displayImage (callback)](#apidoc.element.blessed.overlayimage.prototype.displayImage)
- description and source-code
```javascript
displayImage = function (callback) {
  return this.screen.displayImage(this.file, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.getPixelRatio"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>getPixelRatio (callback)](#apidoc.element.blessed.overlayimage.prototype.getPixelRatio)
- description and source-code
```javascript
getPixelRatio = function (callback) {
  var self = this;

  if (cp.execSync) {
    callback = callback || function(err, result) { return result; };
    try {
      return callback(null, this.getPixelRatioSync());
    } catch (e) {
      return callback(e);
    }
  }

  // XXX We could cache this, but sometimes it's better
  // to recalculate to be pixel perfect.
  if (this._ratio && !this._needsRatio) {
    return callback(null, this._ratio);
  }

  return this.termSize(function(err, dimensions) {
    if (err) return callback(err);

    self._ratio = {
      tw: dimensions.width / self.screen.width,
      th: dimensions.height / self.screen.height
    };

    self._needsRatio = false;

    return callback(null, self._ratio);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.getPixelRatioSync"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>getPixelRatioSync ()](#apidoc.element.blessed.overlayimage.prototype.getPixelRatioSync)
- description and source-code
```javascript
getPixelRatioSync = function () {
  // XXX We could cache this, but sometimes it's better
  // to recalculate to be pixel perfect.
  if (this._ratio && !this._needsRatio) {
    return this._ratio;
  }
  this._needsRatio = false;

  var dimensions = this.termSizeSync();

  this._ratio = {
    tw: dimensions.width / this.screen.width,
    th: dimensions.height / this.screen.height
  };

  return this._ratio;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.imageSize"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>imageSize (callback)](#apidoc.element.blessed.overlayimage.prototype.imageSize)
- description and source-code
```javascript
imageSize = function (callback) {
  var img = this.file;

  if (cp.execSync) {
    callback = callback || function(err, result) { return result; };
    try {
      return callback(null, this.imageSizeSync());
    } catch (e) {
      return callback(e);
    }
  }

  if (OverlayImage.hasW3MDisplay === false) {
    if (!callback) return;
    return callback(new Error('W3M Image Display not available.'));
  }

  if (!img) {
    if (!callback) return;
    return callback(new Error('No image.'));
  }

  var opt = {
    stdio: 'pipe',
    env: process.env,
    cwd: process.env.HOME
  };

  var ps = this.spawn(OverlayImage.w3mdisplay, [], opt);

  var buf = '';

  ps.stdout.setEncoding('utf8');

  ps.stdout.on('data', function(data) {
    buf += data;
  });

  ps.on('error', function(err) {
    if (!callback) return;
    return callback(err);
  });

  ps.on('exit', function() {
    if (!callback) return;
    var size = buf.trim().split(/\s+/);
    return callback(null, {
      raw: buf.trim(),
      width: +size[0],
      height: +size[1]
    });
  });

  var input = '5;' + img + '\n';

  ps.stdin.write(input);
  ps.stdin.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.imageSizeSync"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>imageSizeSync ()](#apidoc.element.blessed.overlayimage.prototype.imageSizeSync)
- description and source-code
```javascript
imageSizeSync = function () {
  var img = this.file;

  if (OverlayImage.hasW3MDisplay === false) {
    throw new Error('W3M Image Display not available.');
  }

  if (!img) {
    throw new Error('No image.');
  }

  var buf = '';
  var input = '5;' + img + '\n';

  try {
    buf = cp.execFileSync(OverlayImage.w3mdisplay, [], {
      env: process.env,
      encoding: 'utf8',
      input: input,
      timeout: 1000
    });
  } catch (e) {
    ;
  }

  var size = buf.trim().split(/\s+/);

  return {
    raw: buf.trim(),
    width: +size[0],
    height: +size[1]
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.renderImage"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>renderImage (img, ratio, callback)](#apidoc.element.blessed.overlayimage.prototype.renderImage)
- description and source-code
```javascript
renderImage = function (img, ratio, callback) {
  var self = this;

  if (cp.execSync) {
    callback = callback || function(err, result) { return result; };
    try {
      return callback(null, this.renderImageSync(img, ratio));
    } catch (e) {
      return callback(e);
    }
  }

  if (OverlayImage.hasW3MDisplay === false) {
    if (!callback) return;
    return callback(new Error('W3M Image Display not available.'));
  }

  if (!ratio) {
    if (!callback) return;
    return callback(new Error('No ratio.'));
  }

  // clearImage unsets these:
  var _file = self.file;
  var _lastSize = self._lastSize;
  return self.clearImage(function(err) {
    if (err) return callback(err);

    self.file = _file;
    self._lastSize = _lastSize;

    var opt = {
      stdio: 'pipe',
      env: process.env,
      cwd: process.env.HOME
    };

    var ps = self.spawn(OverlayImage.w3mdisplay, [], opt, function(err, success) {
      if (!callback) return;
      return err
        ? callback(err)
        : callback(null, success);
    });

    var width = self.width * ratio.tw | 0
      , height = self.height * ratio.th | 0
      , aleft = self.aleft * ratio.tw | 0
      , atop = self.atop * ratio.th | 0;

    var input = '0;1;'
      + aleft + ';'
      + atop + ';'
      + width + ';'
      + height + ';;;;;'
      + img
      + '\n4;\n3;\n';

    self._props = {
      aleft: aleft,
      atop: atop,
      width: width,
      height: height
    };

    ps.stdin.write(input);
    ps.stdin.end();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.renderImageSync"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>renderImageSync (img, ratio)](#apidoc.element.blessed.overlayimage.prototype.renderImageSync)
- description and source-code
```javascript
renderImageSync = function (img, ratio) {
  if (OverlayImage.hasW3MDisplay === false) {
    throw new Error('W3M Image Display not available.');
  }

  if (!ratio) {
    throw new Error('No ratio.');
  }

  // clearImage unsets these:
  var _file = this.file;
  var _lastSize = this._lastSize;

  this.clearImageSync();

  this.file = _file;
  this._lastSize = _lastSize;

  var width = this.width * ratio.tw | 0
    , height = this.height * ratio.th | 0
    , aleft = this.aleft * ratio.tw | 0
    , atop = this.atop * ratio.th | 0;

  var input = '0;1;'
    + aleft + ';'
    + atop + ';'
    + width + ';'
    + height + ';;;;;'
    + img
    + '\n4;\n3;\n';

  this._props = {
    aleft: aleft,
    atop: atop,
    width: width,
    height: height
  };

  try {
    cp.execFileSync(OverlayImage.w3mdisplay, [], {
      env: process.env,
      encoding: 'utf8',
      input: input,
      timeout: 1000
    });
  } catch (e) {
    ;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.setImage"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>setImage (img, callback)](#apidoc.element.blessed.overlayimage.prototype.setImage)
- description and source-code
```javascript
setImage = function (img, callback) {
  var self = this;

  if (this._settingImage) {
    this._queue = this._queue || [];
    this._queue.push([img, callback]);
    return;
  }
  this._settingImage = true;

  var reset = function() {
    self._settingImage = false;
    self._queue = self._queue || [];
    var item = self._queue.shift();
    if (item) {
      self.setImage(item[0], item[1]);
    }
  };

  if (OverlayImage.hasW3MDisplay === false) {
    reset();
    if (!callback) return;
    return callback(new Error('W3M Image Display not available.'));
  }

  if (!img) {
    reset();
    if (!callback) return;
    return callback(new Error('No image.'));
  }

  this.file = img;

  return this.getPixelRatio(function(err, ratio) {
    if (err) {
      reset();
      if (!callback) return;
      return callback(err);
    }

    return self.renderImage(img, ratio, function(err, success) {
      if (err) {
        reset();
        if (!callback) return;
        return callback(err);
      }

      if (self.shrink || self.options.autofit) {
        delete self.shrink;
        delete self.options.shrink;
        self.options.autofit = true;
        return self.imageSize(function(err, size) {
          if (err) {
            reset();
            if (!callback) return;
            return callback(err);
          }

          if (self._lastSize
              && ratio.tw === self._lastSize.tw
              && ratio.th === self._lastSize.th
              && size.width === self._lastSize.width
              && size.height === self._lastSize.height
              && self.aleft === self._lastSize.aleft
              && self.atop === self._lastSize.atop) {
            reset();
            if (!callback) return;
            return callback(null, success);
          }

          self._lastSize = {
            tw: ratio.tw,
            th: ratio.th,
            width: size.width,
            height: size.height,
            aleft: self.aleft,
            atop: self.atop
          };

          self.position.width = size.width / ratio.tw | 0;
          self.position.height = size.height / ratio.th | 0;

          self._noImage = true;
          self.screen.render();
          self._noImage = false;

          reset();
          return self.renderImage(img, ratio, callback);
        });
      }

      reset();
      if (!callback) return;
      return callback(null, success);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.spawn"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>spawn (file, args, opt, callback)](#apidoc.element.blessed.overlayimage.prototype.spawn)
- description and source-code
```javascript
spawn = function (file, args, opt, callback) {
  var spawn = require('child_process').spawn
    , ps;

  opt = opt || {};
  ps = spawn(file, args, opt);

  ps.on('error', function(err) {
    if (!callback) return;
    return callback(err);
  });

  ps.on('exit', function(code) {
    if (!callback) return;
    if (code !== 0) return callback(new Error('Exit Code: ' + code));
    return callback(null, code === 0);
  });

  return ps;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.termSize"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>termSize (callback)](#apidoc.element.blessed.overlayimage.prototype.termSize)
- description and source-code
```javascript
termSize = function (callback) {
  var self = this;

  if (cp.execSync) {
    callback = callback || function(err, result) { return result; };
    try {
      return callback(null, this.termSizeSync());
    } catch (e) {
      return callback(e);
    }
  }

  if (OverlayImage.hasW3MDisplay === false) {
    if (!callback) return;
    return callback(new Error('W3M Image Display not available.'));
  }

  var opt = {
    stdio: 'pipe',
    env: process.env,
    cwd: process.env.HOME
  };

  var ps = this.spawn(OverlayImage.w3mdisplay, ['-test'], opt);

  var buf = '';

  ps.stdout.setEncoding('utf8');

  ps.stdout.on('data', function(data) {
    buf += data;
  });

  ps.on('error', function(err) {
    if (!callback) return;
    return callback(err);
  });

  ps.on('exit', function() {
    if (!callback) return;

    if (!buf.trim()) {
      // Bug: w3mimgdisplay will sometimes
      // output nothing. Try again:
      return self.termSize(callback);
    }

    var size = buf.trim().split(/\s+/);

    return callback(null, {
      raw: buf.trim(),
      width: +size[0],
      height: +size[1]
    });
  });

  ps.stdin.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.overlayimage.prototype.termSizeSync"></a>[function <span class="apidocSignatureSpan">blessed.overlayimage.prototype.</span>termSizeSync (_, recurse)](#apidoc.element.blessed.overlayimage.prototype.termSizeSync)
- description and source-code
```javascript
termSizeSync = function (_, recurse) {
  if (OverlayImage.hasW3MDisplay === false) {
    throw new Error('W3M Image Display not available.');
  }

  var buf = '';

  try {
    buf = cp.execFileSync(OverlayImage.w3mdisplay, ['-test'], {
      env: process.env,
      encoding: 'utf8',
      timeout: 1000
    });
  } catch (e) {
    ;
  }

  if (!buf.trim()) {
    // Bug: w3mimgdisplay will sometimes
    // output nothing. Try again:
    recurse = recurse || 0;
    if (++recurse === 5) {
      throw new Error('Term size not determined.');
    }
    return this.termSizeSync(_, recurse);
  }

  var size = buf.trim().split(/\s+/);

  return {
    raw: buf.trim(),
    width: +size[0],
    height: +size[1]
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.progressbar"></a>[module blessed.progressbar](#apidoc.module.blessed.progressbar)

#### <a name="apidoc.element.blessed.progressbar.progressbar"></a>[function <span class="apidocSignatureSpan">blessed.</span>progressbar (options)](#apidoc.element.blessed.progressbar.progressbar)
- description and source-code
```javascript
function ProgressBar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ProgressBar(options);
  }

  options = options || {};

  Input.call(this, options);

  this.filled = options.filled || 0;
  if (typeof this.filled === 'string') {
    this.filled = +this.filled.slice(0, -1);
  }
  this.value = this.filled;

  this.pch = options.pch || ' ';

  // XXX Workaround that predates the usage of 'el.ch'.
  if (options.ch) {
    this.pch = options.ch;
    this.ch = ' ';
  }
  if (options.bch) {
    this.ch = options.bch;
  }

  if (!this.style.bar) {
    this.style.bar = {};
    this.style.bar.fg = options.barFg;
    this.style.bar.bg = options.barBg;
  }

  this.orientation = options.orientation || 'horizontal';

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      var back, forward;
      if (self.orientation === 'horizontal') {
        back = ['left', 'h'];
        forward = ['right', 'l'];
      } else if (self.orientation === 'vertical') {
        back = ['down', 'j'];
        forward = ['up', 'k'];
      }
      if (key.name === back[0] || (options.vi && key.name === back[1])) {
        self.progress(-5);
        self.screen.render();
        return;
      }
      if (key.name === forward[0] || (options.vi && key.name === forward[1])) {
        self.progress(5);
        self.screen.render();
        return;
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      var x, y, m, p;
      if (!self.lpos) return;
      if (self.orientation === 'horizontal') {
        x = data.x - self.lpos.xi;
        m = (self.lpos.xl - self.lpos.xi) - self.iwidth;
        p = x / m * 100 | 0;
      } else if (self.orientation === 'vertical') {
        y = data.y - self.lpos.yi;
        m = (self.lpos.yl - self.lpos.yi) - self.iheight;
        p = y / m * 100 | 0;
      }
      self.setProgress(p);
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.progressbar.prototype"></a>[module blessed.progressbar.prototype](#apidoc.module.blessed.progressbar.prototype)

#### <a name="apidoc.element.blessed.progressbar.prototype.progress"></a>[function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>progress (filled)](#apidoc.element.blessed.progressbar.prototype.progress)
- description and source-code
```javascript
progress = function (filled) {
  this.filled += filled;
  if (this.filled < 0) this.filled = 0;
  else if (this.filled > 100) this.filled = 100;
  if (this.filled === 100) {
    this.emit('complete');
  }
  this.value = this.filled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.progressbar.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>render ()](#apidoc.element.blessed.progressbar.prototype.render)
- description and source-code
```javascript
render = function () {
  var ret = this._render();
  if (!ret) return;

  var xi = ret.xi
    , xl = ret.xl
    , yi = ret.yi
    , yl = ret.yl
    , dattr;

  if (this.border) xi++, yi++, xl--, yl--;

  if (this.orientation === 'horizontal') {
    xl = xi + ((xl - xi) * (this.filled / 100)) | 0;
  } else if (this.orientation === 'vertical') {
    yi = yi + ((yl - yi) - (((yl - yi) * (this.filled / 100)) | 0));
  }

  dattr = this.sattr(this.style.bar);

  this.screen.fillRegion(dattr, this.pch, xi, xl, yi, yl);

  if (this.content) {
    var line = this.screen.lines[yi];
    for (var i = 0; i < this.content.length; i++) {
      line[xi + i][1] = this.content[i];
    }
    line.dirty = true;
  }

  return ret;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.progressbar.prototype.reset"></a>[function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>reset ()](#apidoc.element.blessed.progressbar.prototype.reset)
- description and source-code
```javascript
reset = function () {
  this.emit('reset');
  this.filled = 0;
  this.value = this.filled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.progressbar.prototype.setProgress"></a>[function <span class="apidocSignatureSpan">blessed.progressbar.prototype.</span>setProgress (filled)](#apidoc.element.blessed.progressbar.prototype.setProgress)
- description and source-code
```javascript
setProgress = function (filled) {
  this.filled = 0;
  this.progress(filled);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.prompt"></a>[module blessed.prompt](#apidoc.module.blessed.prompt)

#### <a name="apidoc.element.blessed.prompt.prompt"></a>[function <span class="apidocSignatureSpan">blessed.</span>prompt (options)](#apidoc.element.blessed.prompt.prompt)
- description and source-code
```javascript
function Prompt(options) {
  if (!(this instanceof Node)) {
    return new Prompt(options);
  }

  options = options || {};

  options.hidden = true;

  Box.call(this, options);

  this._.input = new Textbox({
    parent: this,
    top: 3,
    height: 1,
    left: 2,
    right: 2,
    bg: 'black'
  });

  this._.okay = new Button({
    parent: this,
    top: 5,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    parent: this,
    top: 5,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.prompt.prototype"></a>[module blessed.prompt.prototype](#apidoc.module.blessed.prompt.prototype)

#### <a name="apidoc.element.blessed.prompt.prototype.input"></a>[function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>input (text, value, callback)](#apidoc.element.blessed.prompt.prototype.input)
- description and source-code
```javascript
input = function (text, value, callback) {
  var self = this;
  var okay, cancel;

  if (!callback) {
    callback = value;
    value = '';
  }

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.show();
  this.setContent(' ' + text);

  this._.input.value = value;

  this.screen.saveFocus();

  this._.okay.on('press', okay = function() {
    self._.input.submit();
  });

  this._.cancel.on('press', cancel = function() {
    self._.input.cancel();
  });

  this._.input.readInput(function(err, data) {
    self.hide();
    self.screen.restoreFocus();
    self._.okay.removeListener('press', okay);
    self._.cancel.removeListener('press', cancel);
    return callback(err, data);
  });

  this.screen.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.prompt.prototype.readInput"></a>[function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>readInput (text, value, callback)](#apidoc.element.blessed.prompt.prototype.readInput)
- description and source-code
```javascript
readInput = function (text, value, callback) {
  var self = this;
  var okay, cancel;

  if (!callback) {
    callback = value;
    value = '';
  }

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.show();
  this.setContent(' ' + text);

  this._.input.value = value;

  this.screen.saveFocus();

  this._.okay.on('press', okay = function() {
    self._.input.submit();
  });

  this._.cancel.on('press', cancel = function() {
    self._.input.cancel();
  });

  this._.input.readInput(function(err, data) {
    self.hide();
    self.screen.restoreFocus();
    self._.okay.removeListener('press', okay);
    self._.cancel.removeListener('press', cancel);
    return callback(err, data);
  });

  this.screen.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.prompt.prototype.setInput"></a>[function <span class="apidocSignatureSpan">blessed.prompt.prototype.</span>setInput (text, value, callback)](#apidoc.element.blessed.prompt.prototype.setInput)
- description and source-code
```javascript
setInput = function (text, value, callback) {
  var self = this;
  var okay, cancel;

  if (!callback) {
    callback = value;
    value = '';
  }

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.show();
  this.setContent(' ' + text);

  this._.input.value = value;

  this.screen.saveFocus();

  this._.okay.on('press', okay = function() {
    self._.input.submit();
  });

  this._.cancel.on('press', cancel = function() {
    self._.input.cancel();
  });

  this._.input.readInput(function(err, data) {
    self.hide();
    self.screen.restoreFocus();
    self._.okay.removeListener('press', okay);
    self._.cancel.removeListener('press', cancel);
    return callback(err, data);
  });

  this.screen.render();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.question"></a>[module blessed.question](#apidoc.module.blessed.question)

#### <a name="apidoc.element.blessed.question.question"></a>[function <span class="apidocSignatureSpan">blessed.</span>question (options)](#apidoc.element.blessed.question.question)
- description and source-code
```javascript
function Question(options) {
  if (!(this instanceof Node)) {
    return new Question(options);
  }

  options = options || {};
  options.hidden = true;

  Box.call(this, options);

  this._.okay = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.question.prototype"></a>[module blessed.question.prototype](#apidoc.module.blessed.question.prototype)

#### <a name="apidoc.element.blessed.question.prototype.ask"></a>[function <span class="apidocSignatureSpan">blessed.question.prototype.</span>ask (text, callback)](#apidoc.element.blessed.question.prototype.ask)
- description and source-code
```javascript
ask = function (text, callback) {
  var self = this;
  var press, okay, cancel;

  // Keep above:
  // var parent = this.parent;
  // this.detach();
  // parent.append(this);

  this.show();
  this.setContent(' ' + text);

  this.onScreenEvent('keypress', press = function(ch, key) {
    if (key.name === 'mouse') return;
    if (key.name !== 'enter'
        && key.name !== 'escape'
        && key.name !== 'q'
        && key.name !== 'y'
        && key.name !== 'n') {
      return;
    }
    done(null, key.name === 'enter' || key.name === 'y');
  });

  this._.okay.on('press', okay = function() {
    done(null, true);
  });

  this._.cancel.on('press', cancel = function() {
    done(null, false);
  });

  this.screen.saveFocus();
  this.focus();

  function done(err, data) {
    self.hide();
    self.screen.restoreFocus();
    self.removeScreenEvent('keypress', press);
    self._.okay.removeListener('press', okay);
    self._.cancel.removeListener('press', cancel);
    return callback(err, data);
  }

  this.screen.render();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.radiobutton"></a>[module blessed.radiobutton](#apidoc.module.blessed.radiobutton)

#### <a name="apidoc.element.blessed.radiobutton.radiobutton"></a>[function <span class="apidocSignatureSpan">blessed.</span>radiobutton (options)](#apidoc.element.blessed.radiobutton.radiobutton)
- description and source-code
```javascript
function RadioButton(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new RadioButton(options);
  }

  options = options || {};

  Checkbox.call(this, options);

  this.on('check', function() {
    var el = self;
    while (el = el.parent) {
      if (el.type === 'radio-set'
          || el.type === 'form') break;
    }
    el = el || self.parent;
    el.forDescendants(function(el) {
      if (el.type !== 'radio-button' || el === self) {
        return;
      }
      el.uncheck();
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.radiobutton.prototype"></a>[module blessed.radiobutton.prototype](#apidoc.module.blessed.radiobutton.prototype)

#### <a name="apidoc.element.blessed.radiobutton.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.radiobutton.prototype.</span>render ()](#apidoc.element.blessed.radiobutton.prototype.render)
- description and source-code
```javascript
render = function () {
  this.clearPos(true);
  this.setContent('(' + (this.checked ? '*' : ' ') + ') ' + this.text, true);
  return this._render();
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.radiobutton.prototype.toggle"></a>[function <span class="apidocSignatureSpan">blessed.radiobutton.prototype.</span>toggle ()](#apidoc.element.blessed.radiobutton.prototype.toggle)
- description and source-code
```javascript
toggle = function () {
  if (this.checked) return;
  this.checked = this.value = true;
  this.emit('check');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.scrollablebox"></a>[module blessed.scrollablebox](#apidoc.module.blessed.scrollablebox)

#### <a name="apidoc.element.blessed.scrollablebox.scrollablebox"></a>[function <span class="apidocSignatureSpan">blessed.</span>scrollablebox (options)](#apidoc.element.blessed.scrollablebox.scrollablebox)
- description and source-code
```javascript
function ScrollableBox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ScrollableBox(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.scrollable === false) {
    return this;
  }

  this.scrollable = true;
  this.childOffset = 0;
  this.childBase = 0;
  this.baseLimit = options.baseLimit || Infinity;
  this.alwaysScroll = options.alwaysScroll;

  this.scrollbar = options.scrollbar;
  if (this.scrollbar) {
    this.scrollbar.ch = this.scrollbar.ch || ' ';
    this.style.scrollbar = this.style.scrollbar || this.scrollbar.style;
    if (!this.style.scrollbar) {
      this.style.scrollbar = {};
      this.style.scrollbar.fg = this.scrollbar.fg;
      this.style.scrollbar.bg = this.scrollbar.bg;
      this.style.scrollbar.bold = this.scrollbar.bold;
      this.style.scrollbar.underline = this.scrollbar.underline;
      this.style.scrollbar.inverse = this.scrollbar.inverse;
      this.style.scrollbar.invisible = this.scrollbar.invisible;
    }
    //this.scrollbar.style = this.style.scrollbar;
    if (this.track || this.scrollbar.track) {
      this.track = this.scrollbar.track || this.track;
      this.style.track = this.style.scrollbar.track || this.style.track;
      this.track.ch = this.track.ch || ' ';
      this.style.track = this.style.track || this.track.style;
      if (!this.style.track) {
        this.style.track = {};
        this.style.track.fg = this.track.fg;
        this.style.track.bg = this.track.bg;
        this.style.track.bold = this.track.bold;
        this.style.track.underline = this.track.underline;
        this.style.track.inverse = this.track.inverse;
        this.style.track.invisible = this.track.invisible;
      }
      this.track.style = this.style.track;
    }
    // Allow controlling of the scrollbar via the mouse:
    if (options.mouse) {
      this.on('mousedown', function(data) {
        if (self._scrollingBar) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          return;
        }
        var x = data.x - self.aleft;
        var y = data.y - self.atop;
        if (x === self.width - self.iright - 1) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          var perc = (y - self.itop) / (self.height - self.iheight);
          self.setScrollPerc(perc * 100 | 0);
          self.screen.render();
          var smd, smu;
          self._scrollingBar = true;
          self.onScreenEvent('mousedown', smd = function(data) {
            var y = data.y - self.atop;
            var perc = y / self.height;
            self.setScrollPerc(perc * 100 | 0);
            self.screen.render();
          });
          // If mouseup occurs out of the window, no mouseup event fires, and
          // scrollbar will drag again on mousedown until another mouseup
          // occurs.
          self.onScreenEvent('mouseup', smu = function() {
            self._scrollingBar = false;
            self.removeScreenEvent('mousedown', smd);
            self.removeScreenEvent('mouseup', smu);
          });
        }
      });
    }
  }

  if (options.mouse) {
    this.on('wheeldown', function() {
      self.scroll(self.height / 2 | 0 || 1);
      self.screen.render();
    });
    this.on('wheelup', function() {
      self.scroll(-(self.height / 2 | 0) || -1);
      self.screen.render();
    });
  }

  if (options.keys && !options.ignoreKeys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.scroll(-1);
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.scroll(1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.scroll(-(self.height / 2 | 0) || -1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.scroll( ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.scrollablebox.prototype"></a>[module blessed.scrollablebox.prototype](#apidoc.module.blessed.scrollablebox.prototype)

#### <a name="apidoc.element.blessed.scrollablebox.prototype._recalculateIndex"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>_recalculateIndex ()](#apidoc.element.blessed.scrollablebox.prototype._recalculateIndex)
- description and source-code
```javascript
_recalculateIndex = function () {
  var max, emax;

  if (this.detached || !this.scrollable) {
    return 0;
  }

  // XXX
  // max = this.getScrollHeight() - (this.height - this.iheight);

  max = this._clines.length - (this.height - this.iheight);
  if (max < 0) max = 0;
  emax = this._scrollBottom() - (this.height - this.iheight);
  if (emax < 0) emax = 0;

  this.childBase = Math.min(this.childBase, Math.max(emax, max));

  if (this.childBase < 0) {
    this.childBase = 0;
  } else if (this.childBase > this.baseLimit) {
    this.childBase = this.baseLimit;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype._scrollBottom"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>_scrollBottom ()](#apidoc.element.blessed.scrollablebox.prototype._scrollBottom)
- description and source-code
```javascript
_scrollBottom = function () {
  if (!this.scrollable) return 0;

  // We could just calculate the children, but we can
  // optimize for lists by just returning the items.length.
  if (this._isList) {
    return this.items ? this.items.length : 0;
  }

  if (this.lpos && this.lpos._scrollBottom) {
    return this.lpos._scrollBottom;
  }

  var bottom = this.children.reduce(function(current, el) {
    // el.height alone does not calculate the shrunken height, we need to use
    // getCoords. A shrunken box inside a scrollable element will not grow any
    // larger than the scrollable element's context regardless of how much
    // content is in the shrunken box, unless we do this (call getCoords
    // without the scrollable calculation):
    // See: $ node test/widget-shrink-fail-2.js
    if (!el.detached) {
      var lpos = el._getCoords(false, true);
      if (lpos) {
        return Math.max(current, el.rtop + (lpos.yl - lpos.yi));
      }
    }
    return Math.max(current, el.rtop + el.height);
  }, 0);

  // XXX Use this? Makes .getScrollHeight() useless!
  // if (bottom < this._clines.length) bottom = this._clines.length;

  if (this.lpos) this.lpos._scrollBottom = bottom;

  return bottom;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.getScroll"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScroll ()](#apidoc.element.blessed.scrollablebox.prototype.getScroll)
- description and source-code
```javascript
getScroll = function () {
  return this.childBase + this.childOffset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.getScrollHeight"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScrollHeight ()](#apidoc.element.blessed.scrollablebox.prototype.getScrollHeight)
- description and source-code
```javascript
getScrollHeight = function () {
  return Math.max(this._clines.length, this._scrollBottom());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.getScrollPerc"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>getScrollPerc (s)](#apidoc.element.blessed.scrollablebox.prototype.getScrollPerc)
- description and source-code
```javascript
getScrollPerc = function (s) {
  var pos = this.lpos || this._getCoords();
  if (!pos) return s ? -1 : 0;

  var height = (pos.yl - pos.yi) - this.iheight
    , i = this.getScrollHeight()
    , p;

  if (height < i) {
    if (this.alwaysScroll) {
      p = this.childBase / (i - height);
    } else {
      p = (this.childBase + this.childOffset) / (i - 1);
    }
    return p * 100;
  }

  return s ? -1 : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.resetScroll"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>resetScroll ()](#apidoc.element.blessed.scrollablebox.prototype.resetScroll)
- description and source-code
```javascript
resetScroll = function () {
  if (!this.scrollable) return;
  this.childOffset = 0;
  this.childBase = 0;
  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.scroll"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>scroll (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.scroll)
- description and source-code
```javascript
scroll = function (offset, always) {
  if (!this.scrollable) return;

  if (this.detached) return;

  // Handle scrolling.
  var visible = this.height - this.iheight
    , base = this.childBase
    , d
    , p
    , t
    , b
    , max
    , emax;

  if (this.alwaysScroll || always) {
    // Semi-workaround
    this.childOffset = offset > 0
      ? visible - 1 + offset
      : offset;
  } else {
    this.childOffset += offset;
  }

  if (this.childOffset > visible - 1) {
    d = this.childOffset - (visible - 1);
    this.childOffset -= d;
    this.childBase += d;
  } else if (this.childOffset < 0) {
    d = this.childOffset;
    this.childOffset += -d;
    this.childBase += d;
  }

  if (this.childBase < 0) {
    this.childBase = 0;
  } else if (this.childBase > this.baseLimit) {
    this.childBase = this.baseLimit;
  }

  // Find max "bottom" value for
  // content and descendant elements.
  // Scroll the content if necessary.
  if (this.childBase === base) {
    return this.emit('scroll');
  }

  // When scrolling text, we want to be able to handle SGR codes as well as line
  // feeds. This allows us to take preformatted text output from other programs
  // and put it in a scrollable text box.
  this.parseContent();

  // XXX
  // max = this.getScrollHeight() - (this.height - this.iheight);

  max = this._clines.length - (this.height - this.iheight);
  if (max < 0) max = 0;
  emax = this._scrollBottom() - (this.height - this.iheight);
  if (emax < 0) emax = 0;

  this.childBase = Math.min(this.childBase, Math.max(emax, max));

  if (this.childBase < 0) {
    this.childBase = 0;
  } else if (this.childBase > this.baseLimit) {
    this.childBase = this.baseLimit;
  }

  // Optimize scrolling with CSR + IL/DL.
  p = this.lpos;
  // Only really need _getCoords() if we want
  // to allow nestable scrolling elements...
  // or if we **really** want shrinkable
  // scrolling elements.
  // p = this._getCoords();
  if (p && this.childBase !== base && this.screen.cleanSides(this)) {
    t = p.yi + this.itop;
    b = p.yl - this.ibottom - 1;
    d = this.childBase - base;

    if (d > 0 && d < visible) {
      // scrolled down
      this.screen.deleteLine(d, t, t, b);
    } else if (d < 0 && -d < visible) {
      // scrolled up
      d = -d;
      this.screen.insertLine(d, t, t, b);
    }
  }

  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.scrollTo"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>scrollTo (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.scrollTo)
- description and source-code
```javascript
scrollTo = function (offset, always) {
  // XXX
  // At first, this appeared to account for the first new calculation of childBase:
  this.scroll(0);
  return this.scroll(offset - (this.childBase + this.childOffset), always);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.setScroll"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>setScroll (offset, always)](#apidoc.element.blessed.scrollablebox.prototype.setScroll)
- description and source-code
```javascript
setScroll = function (offset, always) {
  // XXX
  // At first, this appeared to account for the first new calculation of childBase:
  this.scroll(0);
  return this.scroll(offset - (this.childBase + this.childOffset), always);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.scrollablebox.prototype.setScrollPerc"></a>[function <span class="apidocSignatureSpan">blessed.scrollablebox.prototype.</span>setScrollPerc (i)](#apidoc.element.blessed.scrollablebox.prototype.setScrollPerc)
- description and source-code
```javascript
setScrollPerc = function (i) {
  // XXX
  // var m = this.getScrollHeight();
  var m = Math.max(this._clines.length, this._scrollBottom());
  return this.scrollTo((i / 100) * m | 0);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.table"></a>[module blessed.table](#apidoc.module.blessed.table)

#### <a name="apidoc.element.blessed.table.table"></a>[function <span class="apidocSignatureSpan">blessed.</span>table (options)](#apidoc.element.blessed.table.table)
- description and source-code
```javascript
function Table(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Table(options);
  }

  options = options || {};
  options.shrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  options.align = options.align || 'center';

  // Regular tables do not get custom height (this would
  // require extra padding). Maybe add in the future.
  delete options.height;

  Box.call(this, options);

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setContent('');
    self.setData(self.rows);
  });

  this.on('resize', function() {
    self.setContent('');
    self.setData(self.rows);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.table.prototype"></a>[module blessed.table.prototype](#apidoc.module.blessed.table.prototype)

#### <a name="apidoc.element.blessed.table.prototype._calculateMaxes"></a>[function <span class="apidocSignatureSpan">blessed.table.prototype.</span>_calculateMaxes ()](#apidoc.element.blessed.table.prototype._calculateMaxes)
- description and source-code
```javascript
_calculateMaxes = function () {
  var self = this;
  var maxes = [];

  if (this.detached) return;

  this.rows = this.rows || [];

  this.rows.forEach(function(row) {
    row.forEach(function(cell, i) {
      var clen = self.strWidth(cell);
      if (!maxes[i] || maxes[i] < clen) {
        maxes[i] = clen;
      }
    });
  });

  var total = maxes.reduce(function(total, max) {
    return total + max;
  }, 0);
  total += maxes.length + 1;

  // XXX There might be an issue with resizing where on the first resize event
  // width appears to be less than total if it's a percentage or left/right
  // combination.
  if (this.width < total) {
    delete this.position.width;
  }

  if (this.position.width != null) {
    var missing = this.width - total;
    var w = missing / maxes.length | 0;
    var wr = missing % maxes.length;
    maxes = maxes.map(function(max, i) {
      if (i === maxes.length - 1) {
        return max + w + wr;
      }
      return max + w;
    });
  } else {
    maxes = maxes.map(function(max) {
      return max + self.pad;
    });
  }

  return this._maxes = maxes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.table.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.table.prototype.</span>render ()](#apidoc.element.blessed.table.prototype.render)
- description and source-code
```javascript
render = function () {
  var self = this;

  var coords = this._render();
  if (!coords) return;

  this._calculateMaxes();

  if (!this._maxes) return coords;

  var lines = this.screen.lines
    , xi = coords.xi
    , yi = coords.yi
    , rx
    , ry
    , i;

  var dattr = this.sattr(this.style)
    , hattr = this.sattr(this.style.header)
    , cattr = this.sattr(this.style.cell)
    , battr = this.sattr(this.style.border);

  var width = coords.xl - coords.xi - this.iright
    , height = coords.yl - coords.yi - this.ibottom;

  // Apply attributes to header cells and cells.
  for (var y = this.itop; y < height; y++) {
    if (!lines[yi + y]) break;
    for (var x = this.ileft; x < width; x++) {
      if (!lines[yi + y][xi + x]) break;
      // Check to see if it's not the default attr. Allows for tags:
      if (lines[yi + y][xi + x][0] !== dattr) continue;
      if (y === this.itop) {
        lines[yi + y][xi + x][0] = hattr;
      } else {
        lines[yi + y][xi + x][0] = cattr;
      }
      lines[yi + y].dirty = true;
    }
  }

  if (!this.border || this.options.noCellBorders) return coords;

  // Draw border with correct angles.
  ry = 0;
  for (i = 0; i < self.rows.length + 1; i++) {
    if (!lines[yi + ry]) break;
    rx = 0;
    self._maxes.forEach(function(max, i) {
      rx += max;
      if (i === 0) {
        if (!lines[yi + ry][xi + 0]) return;
        // left side
        if (ry === 0) {
          // top
          lines[yi + ry][xi + 0][0] = battr;
          // lines[yi + ry][xi + 0][1] = '\u250c'; // '┌'
        } else if (ry / 2 === self.rows.length) {
          // bottom
          lines[yi + ry][xi + 0][0] = battr;
          // lines[yi + ry][xi + 0][1] = '\u2514'; // '└'
        } else {
          // middle
          lines[yi + ry][xi + 0][0] = battr;
          lines[yi + ry][xi + 0][1] = '\u251c'; // '├'
          // XXX If we alter iwidth and ileft for no borders - nothing should be written here
          if (!self.border.left) {
            lines[yi + ry][xi + 0][1] = '\u2500'; // '─'
          }
        }
        lines[yi + ry].dirty = true;
      } else if (i === self._maxes.length - 1) {
        if (!lines[yi + ry][xi + rx + 1]) return;
        // right side
        if (ry === 0) {
          // top
          rx++;
          lines[yi + ry][xi + rx][0] = battr;
          // lines[yi + ry][xi + rx][1] = '\u2510'; // '┐'
        } else if (ry / 2 === self.rows.length) {
          // bottom
          rx++;
          lines[yi + ry][xi + rx][0] = battr;
          // lines[yi + ry][xi + rx][1] = '\u2518'; // '┘'
        } else {
          // middle
          rx++;
          lines[yi + ry][xi + rx][0] = battr;
          lines[yi + ry][xi + rx][1] = '\u2524'; // '┤'
          // XXX If we alter iwidth and iright for no borders - nothing should be written here
          if (!self.border.right) {
            lines[yi + ry][xi + rx][1] = '\u2500'; // '─'
          }
        }
        lines[yi + ry].dirty = true;
        return;
      }
      if (!lines[yi + ry][xi + rx + 1]) return;
      // center
      if (ry === 0) {
        // top
        rx++;
        lines[yi + ry][xi + rx][0] = battr;
        lines[yi + ry][xi + rx][1] = '\u252c'; // '┬'
        // XXX If we alter iheight and itop for no borders - nothing should be written here
        if (!self.border.top) {
          lines[yi + ry][xi + rx][1] = '\u2502'; // '│'
        }
      } else if (ry / 2 === self.rows.length) {
        // bottom
        rx++;
        lines[yi + ry][xi + rx][0] = battr;
        lines[yi + ry][xi + rx][1] = '\u2534'; // '┴'
        // XXX If we alter iheight and ibottom for no borders - nothing should be written here
        if (!self.border.bottom) {
          lines[yi + ry][xi + rx][1] = '\u2502'; // '│'
        }
      } else {
        // middle
        if (self.options.fillCellBorders) {
          var lbg = (ry <= 2 ? hattr : cattr) & 0x1ff;
          rx++;
          lines[yi + ry][xi + rx][0] = (battr & ~0x1ff) | lbg;
        } else {
          rx++;
          lines[yi + ry][xi + rx][0] = battr;
        }
        lines[yi + ry ...
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.table.prototype.setData"></a>[function <span class="apidocSignatureSpan">blessed.table.prototype.</span>setData (rows)](#apidoc.element.blessed.table.prototype.setData)
- description and source-code
```javascript
setData = function (rows) {
  var self = this
    , text = ''
    , align = this.align;

  this.rows = rows || [];

  this._calculateMaxes();

  if (!this._maxes) return;

  this.rows.forEach(function(row, i) {
    var isFooter = i === self.rows.length - 1;
    row.forEach(function(cell, i) {
      var width = self._maxes[i];
      var clen = self.strWidth(cell);

      if (i !== 0) {
        text += ' ';
      }

      while (clen < width) {
        if (align === 'center') {
          cell = ' ' + cell + ' ';
          clen += 2;
        } else if (align === 'left') {
          cell = cell + ' ';
          clen += 1;
        } else if (align === 'right') {
          cell = ' ' + cell;
          clen += 1;
        }
      }

      if (clen > width) {
        if (align === 'center') {
          cell = cell.substring(1);
          clen--;
        } else if (align === 'left') {
          cell = cell.slice(0, -1);
          clen--;
        } else if (align === 'right') {
          cell = cell.substring(1);
          clen--;
        }
      }

      text += cell;
    });
    if (!isFooter) {
      text += '\n\n';
    }
  });

  delete this.align;
  this.setContent(text);
  this.align = align;
}
```
- example usage
```shell
...
- Inherits all from List.

##### Methods:

- Inherits all from List.
- __setRows/setData(rows)__ - Set rows in table. Array of arrays of strings.
''' js
  table.setData([
    [ 'Animals',  'Foods'  ],
    [ 'Elephant', 'Apple'  ],
    [ 'Bird',     'Orange' ]
  ]);
'''
...
```

#### <a name="apidoc.element.blessed.table.prototype.setRows"></a>[function <span class="apidocSignatureSpan">blessed.table.prototype.</span>setRows (rows)](#apidoc.element.blessed.table.prototype.setRows)
- description and source-code
```javascript
setRows = function (rows) {
  var self = this
    , text = ''
    , align = this.align;

  this.rows = rows || [];

  this._calculateMaxes();

  if (!this._maxes) return;

  this.rows.forEach(function(row, i) {
    var isFooter = i === self.rows.length - 1;
    row.forEach(function(cell, i) {
      var width = self._maxes[i];
      var clen = self.strWidth(cell);

      if (i !== 0) {
        text += ' ';
      }

      while (clen < width) {
        if (align === 'center') {
          cell = ' ' + cell + ' ';
          clen += 2;
        } else if (align === 'left') {
          cell = cell + ' ';
          clen += 1;
        } else if (align === 'right') {
          cell = ' ' + cell;
          clen += 1;
        }
      }

      if (clen > width) {
        if (align === 'center') {
          cell = cell.substring(1);
          clen--;
        } else if (align === 'left') {
          cell = cell.slice(0, -1);
          clen--;
        } else if (align === 'right') {
          cell = cell.substring(1);
          clen--;
        }
      }

      text += cell;
    });
    if (!isFooter) {
      text += '\n\n';
    }
  });

  delete this.align;
  this.setContent(text);
  this.align = align;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.terminal"></a>[module blessed.terminal](#apidoc.module.blessed.terminal)

#### <a name="apidoc.element.blessed.terminal.terminal"></a>[function <span class="apidocSignatureSpan">blessed.</span>terminal (options)](#apidoc.element.blessed.terminal.terminal)
- description and source-code
```javascript
function Terminal(options) {
  if (!(this instanceof Node)) {
    return new Terminal(options);
  }

  options = options || {};
  options.scrollable = false;

  Box.call(this, options);

  // XXX Workaround for all motion
  if (this.screen.program.tmux && this.screen.program.tmuxVersion >= 2) {
    this.screen.program.enableMouse();
  }

  this.handler = options.handler;
  this.shell = options.shell || process.env.SHELL || 'sh';
  this.args = options.args || [];

  this.cursor = this.options.cursor;
  this.cursorBlink = this.options.cursorBlink;
  this.screenKeys = this.options.screenKeys;

  this.style = this.style || {};
  this.style.bg = this.style.bg || 'default';
  this.style.fg = this.style.fg || 'default';

  this.termName = options.terminal
    || options.term
    || process.env.TERM
    || 'xterm';

  this.bootstrap();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.terminal.prototype"></a>[module blessed.terminal.prototype](#apidoc.module.blessed.terminal.prototype)

#### <a name="apidoc.element.blessed.terminal.prototype._isMouse"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>_isMouse (buf)](#apidoc.element.blessed.terminal.prototype._isMouse)
- description and source-code
```javascript
_isMouse = function (buf) {
  var s = buf;
  if (Buffer.isBuffer(s)) {
    if (s[0] > 127 && s[1] === undefined) {
      s[0] -= 128;
      s = '\x1b' + s.toString('utf-8');
    } else {
      s = s.toString('utf-8');
    }
  }
  return (buf[0] === 0x1b && buf[1] === 0x5b && buf[2] === 0x4d)
    || /^\x1b\[M([\x00\u0020-\uffff]{3})/.test(s)
    || /^\x1b\[(\d+;\d+;\d+)M/.test(s)
    || /^\x1b\[<(\d+;\d+;\d+)([mM])/.test(s)
    || /^\x1b\[<(\d+;\d+;\d+;\d+)&w/.test(s)
    || /^\x1b\[24([0135])~\[(\d+),(\d+)\]\r/.test(s)
    || /^\x1b\[(O|I)/.test(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.bootstrap"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>bootstrap ()](#apidoc.element.blessed.terminal.prototype.bootstrap)
- description and source-code
```javascript
bootstrap = function () {
  var self = this;

  var element = {
    // window
    get document() { return element; },
    navigator: { userAgent: 'node.js' },

    // document
    get defaultView() { return element; },
    get documentElement() { return element; },
    createElement: function() { return element; },

    // element
    get ownerDocument() { return element; },
    addEventListener: function() {},
    removeEventListener: function() {},
    getElementsByTagName: function() { return [element]; },
    getElementById: function() { return element; },
    parentNode: null,
    offsetParent: null,
    appendChild: function() {},
    removeChild: function() {},
    setAttribute: function() {},
    getAttribute: function() {},
    style: {},
    focus: function() {},
    blur: function() {},
    console: console
  };

  element.parentNode = element;
  element.offsetParent = element;

  this.term = require('term.js')({
    termName: this.termName,
    cols: this.width - this.iwidth,
    rows: this.height - this.iheight,
    context: element,
    document: element,
    body: element,
    parent: element,
    cursorBlink: this.cursorBlink,
    screenKeys: this.screenKeys
  });

  this.term.refresh = function() {
    self.screen.render();
  };

  this.term.keyDown = function() {};
  this.term.keyPress = function() {};

  this.term.open(element);

  // Emits key sequences in html-land.
  // Technically not necessary here.
  // In reality if we wanted to be neat, we would overwrite the keyDown and
  // keyPress methods with our own node.js-keys->terminal-keys methods, but
  // since all the keys are already coming in as escape sequences, we can just
  // send the input directly to the handler/socket (see below).
  // this.term.on('data', function(data) {
  //   self.handler(data);
  // });

  // Incoming keys and mouse inputs.
  // NOTE: Cannot pass mouse events - coordinates will be off!
  this.screen.program.input.on('data', this._onData = function(data) {
    if (self.screen.focused === self && !self._isMouse(data)) {
      self.handler(data);
    }
  });

  this.onScreenEvent('mouse', function(data) {
    if (self.screen.focused !== self) return;

    if (data.x < self.aleft + self.ileft) return;
    if (data.y < self.atop + self.itop) return;
    if (data.x > self.aleft - self.ileft + self.width) return;
    if (data.y > self.atop - self.itop + self.height) return;

    if (self.term.x10Mouse
        || self.term.vt200Mouse
        || self.term.normalMouse
        || self.term.mouseEvents
        || self.term.utfMouse
        || self.term.sgrMouse
        || self.term.urxvtMouse) {
      ;
    } else {
      return;
    }

    var b = data.raw[0]
      , x = data.x - self.aleft
      , y = data.y - self.atop
      , s;

    if (self.term.urxvtMouse) {
      if (self.screen.program.sgrMouse) {
        b += 32;
      }
      s = '\x1b[' + b + ';' + (x + 32) + ';' + (y + 32) + 'M';
    } else if (self.term.sgrMouse) {
      if (!self.screen.program.sgrMouse) {
        b -= 32;
      }
      s = '\x1b[<' + b + ';' + x + ';' + y
        + (data.action === 'mousedown' ? 'M' : 'm');
    } else {
      if (self.screen.program.sgrMouse) {
        b += 32;
      }
      s = '\x1b[M'
        + String.fromCharCode(b)
        + String.fromCharCode(x + 32)
        + String.fromCharCode(y + 32);
    }

    self.handler(s);
  });

  this.on('focus', function() {
    self.term.focus();
  });

  this.on('blur', function() {
    self.term.blur();
  });

  this.term.on('title', function(title) {
    self.title = title;
    self.emit('title', title);
  });

  this.term.on('passthrough', function(data) {
    self.screen.program.flush();
    self.screen.program._owrite(data);
  });

  this.on('resize', function() {
    nextTick(function() {
      self.term.resize(self.width - self.iwidth, self.height - self.iheight);
    });
  });

  this.once('render', function() {
    self.term.resize(self.width - self.iwidth, self.height - self.iheight);
  });

  this.on('destroy', function() {
    self.kill();
    self.screen.program.input.removeListener('data', ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.getScroll"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScroll ()](#apidoc.element.blessed.terminal.prototype.getScroll)
- description and source-code
```javascript
getScroll = function () {
  return this.term.ydisp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.getScrollHeight"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScrollHeight ()](#apidoc.element.blessed.terminal.prototype.getScrollHeight)
- description and source-code
```javascript
getScrollHeight = function () {
  return this.term.rows - 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.getScrollPerc"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>getScrollPerc ()](#apidoc.element.blessed.terminal.prototype.getScrollPerc)
- description and source-code
```javascript
getScrollPerc = function () {
  return (this.term.ydisp / this.term.ybase) * 100;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.kill"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>kill ()](#apidoc.element.blessed.terminal.prototype.kill)
- description and source-code
```javascript
kill = function () {
  if (this.pty) {
    this.pty.destroy();
    this.pty.kill();
  }
  this.term.refresh = function() {};
  this.term.write('\x1b[H\x1b[J');
  if (this.term._blink) {
    clearInterval(this.term._blink);
  }
  this.term.destroy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>render ()](#apidoc.element.blessed.terminal.prototype.render)
- description and source-code
```javascript
render = function () {
  var ret = this._render();
  if (!ret) return;

  this.dattr = this.sattr(this.style);

  var xi = ret.xi + this.ileft
    , xl = ret.xl - this.iright
    , yi = ret.yi + this.itop
    , yl = ret.yl - this.ibottom
    , cursor;

  var scrollback = this.term.lines.length - (yl - yi);

  for (var y = Math.max(yi, 0); y < yl; y++) {
    var line = this.screen.lines[y];
    if (!line || !this.term.lines[scrollback + y - yi]) break;

    if (y === yi + this.term.y
        && this.term.cursorState
        && this.screen.focused === this
        && (this.term.ydisp === this.term.ybase || this.term.selectMode)
        && !this.term.cursorHidden) {
      cursor = xi + this.term.x;
    } else {
      cursor = -1;
    }

    for (var x = Math.max(xi, 0); x < xl; x++) {
      if (!line[x] || !this.term.lines[scrollback + y - yi][x - xi]) break;

      line[x][0] = this.term.lines[scrollback + y - yi][x - xi][0];

      if (x === cursor) {
        if (this.cursor === 'line') {
          line[x][0] = this.dattr;
          line[x][1] = '\u2502';
          continue;
        } else if (this.cursor === 'underline') {
          line[x][0] = this.dattr | (2 << 18);
        } else if (this.cursor === 'block' || !this.cursor) {
          line[x][0] = this.dattr | (8 << 18);
        }
      }

      line[x][1] = this.term.lines[scrollback + y - yi][x - xi][1];

      // default foreground = 257
      if (((line[x][0] >> 9) & 0x1ff) === 257) {
        line[x][0] &= ~(0x1ff << 9);
        line[x][0] |= ((this.dattr >> 9) & 0x1ff) << 9;
      }

      // default background = 256
      if ((line[x][0] & 0x1ff) === 256) {
        line[x][0] &= ~0x1ff;
        line[x][0] |= this.dattr & 0x1ff;
      }
    }

    line.dirty = true;
  }

  return ret;
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.terminal.prototype.resetScroll"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>resetScroll ()](#apidoc.element.blessed.terminal.prototype.resetScroll)
- description and source-code
```javascript
resetScroll = function () {
  this.term.ydisp = 0;
  this.term.ybase = 0;
  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.screenshot"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>screenshot (xi, xl, yi, yl)](#apidoc.element.blessed.terminal.prototype.screenshot)
- description and source-code
```javascript
screenshot = function (xi, xl, yi, yl) {
  xi = 0 + (xi || 0);
  if (xl != null) {
    xl = 0 + (xl || 0);
  } else {
    xl = this.term.lines[0].length;
  }
  yi = 0 + (yi || 0);
  if (yl != null) {
    yl = 0 + (yl || 0);
  } else {
    yl = this.term.lines.length;
  }
  return this.screen.screenshot(xi, xl, yi, yl, this.term);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.scroll"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>scroll (offset)](#apidoc.element.blessed.terminal.prototype.scroll)
- description and source-code
```javascript
scroll = function (offset) {
  this.term.scrollDisp(offset);
  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.scrollTo"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>scrollTo (offset)](#apidoc.element.blessed.terminal.prototype.scrollTo)
- description and source-code
```javascript
scrollTo = function (offset) {
  this.term.ydisp = offset;
  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.setScroll"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>setScroll (offset)](#apidoc.element.blessed.terminal.prototype.setScroll)
- description and source-code
```javascript
setScroll = function (offset) {
  this.term.ydisp = offset;
  return this.emit('scroll');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.setScrollPerc"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>setScrollPerc (i)](#apidoc.element.blessed.terminal.prototype.setScrollPerc)
- description and source-code
```javascript
setScrollPerc = function (i) {
  return this.setScroll((i / 100) * this.term.ybase | 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.terminal.prototype.write"></a>[function <span class="apidocSignatureSpan">blessed.terminal.prototype.</span>write (data)](#apidoc.element.blessed.terminal.prototype.write)
- description and source-code
```javascript
write = function (data) {
  return this.term.write(data);
}
```
- example usage
```shell
...
var blessed = require('blessed');

var tput = blessed.tput({
  terminal: 'xterm-256color',
  extended: true
});

process.stdout.write(tput.setaf(4) + 'Hello' + tput.sgr0() + '\n');
'''

To play around with it on the command line, it works just like tput:

''' bash
$ tput.js setaf 2
$ tput.js sgr0
...
```



# <a name="apidoc.module.blessed.textarea"></a>[module blessed.textarea](#apidoc.module.blessed.textarea)

#### <a name="apidoc.element.blessed.textarea.textarea"></a>[function <span class="apidocSignatureSpan">blessed.</span>textarea (options)](#apidoc.element.blessed.textarea.textarea)
- description and source-code
```javascript
function Textarea(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Textarea(options);
  }

  options = options || {};

  options.scrollable = options.scrollable !== false;

  Input.call(this, options);

  this.screen._listenKeys(this);

  this.value = options.value || '';

  this.__updateCursor = this._updateCursor.bind(this);
  this.on('resize', this.__updateCursor);
  this.on('move', this.__updateCursor);

  if (options.inputOnFocus) {
    this.on('focus', this.readInput.bind(this, null));
  }

  if (!options.inputOnFocus && options.keys) {
    this.on('keypress', function(ch, key) {
      if (self._reading) return;
      if (key.name === 'enter' || (options.vi && key.name === 'i')) {
        return self.readInput();
      }
      if (key.name === 'e') {
        return self.readEditor();
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      if (self._reading) return;
      if (data.button !== 'right') return;
      self.readEditor();
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.textarea.prototype"></a>[module blessed.textarea.prototype](#apidoc.module.blessed.textarea.prototype)

#### <a name="apidoc.element.blessed.textarea.prototype._listener"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_listener (ch, key)](#apidoc.element.blessed.textarea.prototype._listener)
- description and source-code
```javascript
_listener = function (ch, key) {
  var done = this._done
    , value = this.value;

  if (key.name === 'return') return;
  if (key.name === 'enter') {
    ch = '\n';
  }

  // TODO: Handle directional keys.
  if (key.name === 'left' || key.name === 'right'
      || key.name === 'up' || key.name === 'down') {
    ;
  }

  if (this.options.keys && key.ctrl && key.name === 'e') {
    return this.readEditor();
  }

  // TODO: Optimize typing by writing directly
  // to the screen and screen buffer here.
  if (key.name === 'escape') {
    done(null, null);
  } else if (key.name === 'backspace') {
    if (this.value.length) {
      if (this.screen.fullUnicode) {
        if (unicode.isSurrogate(this.value, this.value.length - 2)) {
        // || unicode.isCombining(this.value, this.value.length - 1)) {
          this.value = this.value.slice(0, -2);
        } else {
          this.value = this.value.slice(0, -1);
        }
      } else {
        this.value = this.value.slice(0, -1);
      }
    }
  } else if (ch) {
    if (!/^[\x00-\x08\x0b-\x0c\x0e-\x1f\x7f]$/.test(ch)) {
      this.value += ch;
    }
  }

  if (this.value !== value) {
    this.screen.render();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype._typeScroll"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_typeScroll ()](#apidoc.element.blessed.textarea.prototype._typeScroll)
- description and source-code
```javascript
_typeScroll = function () {
  // XXX Workaround
  var height = this.height - this.iheight;
  if (this._clines.length - this.childBase > height) {
    this.scroll(this._clines.length);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype._updateCursor"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>_updateCursor (get)](#apidoc.element.blessed.textarea.prototype._updateCursor)
- description and source-code
```javascript
_updateCursor = function (get) {
  if (this.screen.focused !== this) {
    return;
  }

  var lpos = get ? this.lpos : this._getCoords();
  if (!lpos) return;

  var last = this._clines[this._clines.length - 1]
    , program = this.screen.program
    , line
    , cx
    , cy;

  // Stop a situation where the textarea begins scrolling
  // and the last cline appears to always be empty from the
  // _typeScroll '+ '\n'' thing.
  // Maybe not necessary anymore?
  if (last === '' && this.value[this.value.length - 1] !== '\n') {
    last = this._clines[this._clines.length - 2] || '';
  }

  line = Math.min(
    this._clines.length - 1 - (this.childBase || 0),
    (lpos.yl - lpos.yi) - this.iheight - 1);

  // When calling clearValue() on a full textarea with a border, the first
  // argument in the above Math.min call ends up being -2. Make sure we stay
  // positive.
  line = Math.max(0, line);

  cy = lpos.yi + this.itop + line;
  cx = lpos.xi + this.ileft + this.strWidth(last);

  // XXX Not sure, but this may still sometimes
  // cause problems when leaving editor.
  if (cy === program.y && cx === program.x) {
    return;
  }

  if (cy === program.y) {
    if (cx > program.x) {
      program.cuf(cx - program.x);
    } else if (cx < program.x) {
      program.cub(program.x - cx);
    }
  } else if (cx === program.x) {
    if (cy > program.y) {
      program.cud(cy - program.y);
    } else if (cy < program.y) {
      program.cuu(program.y - cy);
    }
  } else {
    program.cup(cy, cx);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.cancel"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>cancel ()](#apidoc.element.blessed.textarea.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  if (!this.__listener) return;
  return this.__listener('\x1b', { name: 'escape' });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.clearInput"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>clearInput ()](#apidoc.element.blessed.textarea.prototype.clearInput)
- description and source-code
```javascript
clearInput = function () {
  return this.setValue('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.clearValue"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>clearValue ()](#apidoc.element.blessed.textarea.prototype.clearValue)
- description and source-code
```javascript
clearValue = function () {
  return this.setValue('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.editor"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>editor (callback)](#apidoc.element.blessed.textarea.prototype.editor)
- description and source-code
```javascript
editor = function (callback) {
  var self = this;

  if (this._reading) {
    var _cb = this._callback
      , cb = callback;

    this._done('stop');

    callback = function(err, value) {
      if (_cb) _cb(err, value);
      if (cb) cb(err, value);
    };
  }

  if (!callback) {
    callback = function() {};
  }

  return this.screen.readEditor({ value: this.value }, function(err, value) {
    if (err) {
      if (err.message === 'Unsuccessful.') {
        self.screen.render();
        return self.readInput(callback);
      }
      self.screen.render();
      self.readInput(callback);
      return callback(err);
    }
    self.setValue(value);
    self.screen.render();
    return self.readInput(callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.getValue"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>getValue ()](#apidoc.element.blessed.textarea.prototype.getValue)
- description and source-code
```javascript
getValue = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.input"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>input (callback)](#apidoc.element.blessed.textarea.prototype.input)
- description and source-code
```javascript
input = function (callback) {
  var self = this
    , focused = this.screen.focused === this;

  if (this._reading) return;
  this._reading = true;

  this._callback = callback;

  if (!focused) {
    this.screen.saveFocus();
    this.focus();
  }

  this.screen.grabKeys = true;

  this._updateCursor();
  this.screen.program.showCursor();
  //this.screen.program.sgr('normal');

  this._done = function fn(err, value) {
    if (!self._reading) return;

    if (fn.done) return;
    fn.done = true;

    self._reading = false;

    delete self._callback;
    delete self._done;

    self.removeListener('keypress', self.__listener);
    delete self.__listener;

    self.removeListener('blur', self.__done);
    delete self.__done;

    self.screen.program.hideCursor();
    self.screen.grabKeys = false;

    if (!focused) {
      self.screen.restoreFocus();
    }

    if (self.options.inputOnFocus) {
      self.screen.rewindFocus();
    }

    // Ugly
    if (err === 'stop') return;

    if (err) {
      self.emit('error', err);
    } else if (value != null) {
      self.emit('submit', value);
    } else {
      self.emit('cancel', value);
    }
    self.emit('action', value);

    if (!callback) return;

    return err
      ? callback(err)
      : callback(null, value);
  };

  // Put this in a nextTick so the current
  // key event doesn't trigger any keys input.
  nextTick(function() {
    self.__listener = self._listener.bind(self);
    self.on('keypress', self.__listener);
  });

  this.__done = this._done.bind(this, null, null);
  this.on('blur', this.__done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.readEditor"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>readEditor (callback)](#apidoc.element.blessed.textarea.prototype.readEditor)
- description and source-code
```javascript
readEditor = function (callback) {
  var self = this;

  if (this._reading) {
    var _cb = this._callback
      , cb = callback;

    this._done('stop');

    callback = function(err, value) {
      if (_cb) _cb(err, value);
      if (cb) cb(err, value);
    };
  }

  if (!callback) {
    callback = function() {};
  }

  return this.screen.readEditor({ value: this.value }, function(err, value) {
    if (err) {
      if (err.message === 'Unsuccessful.') {
        self.screen.render();
        return self.readInput(callback);
      }
      self.screen.render();
      self.readInput(callback);
      return callback(err);
    }
    self.setValue(value);
    self.screen.render();
    return self.readInput(callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.readInput"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>readInput (callback)](#apidoc.element.blessed.textarea.prototype.readInput)
- description and source-code
```javascript
readInput = function (callback) {
  var self = this
    , focused = this.screen.focused === this;

  if (this._reading) return;
  this._reading = true;

  this._callback = callback;

  if (!focused) {
    this.screen.saveFocus();
    this.focus();
  }

  this.screen.grabKeys = true;

  this._updateCursor();
  this.screen.program.showCursor();
  //this.screen.program.sgr('normal');

  this._done = function fn(err, value) {
    if (!self._reading) return;

    if (fn.done) return;
    fn.done = true;

    self._reading = false;

    delete self._callback;
    delete self._done;

    self.removeListener('keypress', self.__listener);
    delete self.__listener;

    self.removeListener('blur', self.__done);
    delete self.__done;

    self.screen.program.hideCursor();
    self.screen.grabKeys = false;

    if (!focused) {
      self.screen.restoreFocus();
    }

    if (self.options.inputOnFocus) {
      self.screen.rewindFocus();
    }

    // Ugly
    if (err === 'stop') return;

    if (err) {
      self.emit('error', err);
    } else if (value != null) {
      self.emit('submit', value);
    } else {
      self.emit('cancel', value);
    }
    self.emit('action', value);

    if (!callback) return;

    return err
      ? callback(err)
      : callback(null, value);
  };

  // Put this in a nextTick so the current
  // key event doesn't trigger any keys input.
  nextTick(function() {
    self.__listener = self._listener.bind(self);
    self.on('keypress', self.__listener);
  });

  this.__done = this._done.bind(this, null, null);
  this.on('blur', this.__done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.render"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>render ()](#apidoc.element.blessed.textarea.prototype.render)
- description and source-code
```javascript
render = function () {
  this.setValue();
  return this._render();
}
```
- example usage
```shell
...
file: __dirname + '/my-program-icon.png',
search: false
});

// If our box is clicked, change the content.
box.on('click', function(data) {
box.setContent('{center}Some different {red-fg}content{/red-fg}.{/center}');
screen.render();
});

// If box is focused, handle 'enter'/'return' and give us some more content.
box.key('enter', function(ch, key) {
box.setContent('{right}Even different {black-fg}content{/black-fg}.{/right}\n');
box.setLine(1, 'bar');
box.insertLine(1, 'foo');
...
```

#### <a name="apidoc.element.blessed.textarea.prototype.setEditor"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setEditor (callback)](#apidoc.element.blessed.textarea.prototype.setEditor)
- description and source-code
```javascript
setEditor = function (callback) {
  var self = this;

  if (this._reading) {
    var _cb = this._callback
      , cb = callback;

    this._done('stop');

    callback = function(err, value) {
      if (_cb) _cb(err, value);
      if (cb) cb(err, value);
    };
  }

  if (!callback) {
    callback = function() {};
  }

  return this.screen.readEditor({ value: this.value }, function(err, value) {
    if (err) {
      if (err.message === 'Unsuccessful.') {
        self.screen.render();
        return self.readInput(callback);
      }
      self.screen.render();
      self.readInput(callback);
      return callback(err);
    }
    self.setValue(value);
    self.screen.render();
    return self.readInput(callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.setInput"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setInput (callback)](#apidoc.element.blessed.textarea.prototype.setInput)
- description and source-code
```javascript
setInput = function (callback) {
  var self = this
    , focused = this.screen.focused === this;

  if (this._reading) return;
  this._reading = true;

  this._callback = callback;

  if (!focused) {
    this.screen.saveFocus();
    this.focus();
  }

  this.screen.grabKeys = true;

  this._updateCursor();
  this.screen.program.showCursor();
  //this.screen.program.sgr('normal');

  this._done = function fn(err, value) {
    if (!self._reading) return;

    if (fn.done) return;
    fn.done = true;

    self._reading = false;

    delete self._callback;
    delete self._done;

    self.removeListener('keypress', self.__listener);
    delete self.__listener;

    self.removeListener('blur', self.__done);
    delete self.__done;

    self.screen.program.hideCursor();
    self.screen.grabKeys = false;

    if (!focused) {
      self.screen.restoreFocus();
    }

    if (self.options.inputOnFocus) {
      self.screen.rewindFocus();
    }

    // Ugly
    if (err === 'stop') return;

    if (err) {
      self.emit('error', err);
    } else if (value != null) {
      self.emit('submit', value);
    } else {
      self.emit('cancel', value);
    }
    self.emit('action', value);

    if (!callback) return;

    return err
      ? callback(err)
      : callback(null, value);
  };

  // Put this in a nextTick so the current
  // key event doesn't trigger any keys input.
  nextTick(function() {
    self.__listener = self._listener.bind(self);
    self.on('keypress', self.__listener);
  });

  this.__done = this._done.bind(this, null, null);
  this.on('blur', this.__done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.setValue"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>setValue (value)](#apidoc.element.blessed.textarea.prototype.setValue)
- description and source-code
```javascript
setValue = function (value) {
  if (value == null) {
    value = this.value;
  }
  if (this._value !== value) {
    this.value = value;
    this._value = value;
    this.setContent(this.value);
    this._typeScroll();
    this._updateCursor();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textarea.prototype.submit"></a>[function <span class="apidocSignatureSpan">blessed.textarea.prototype.</span>submit ()](#apidoc.element.blessed.textarea.prototype.submit)
- description and source-code
```javascript
submit = function () {
  if (!this.__listener) return;
  return this.__listener('\x1b', { name: 'escape' });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.textbox"></a>[module blessed.textbox](#apidoc.module.blessed.textbox)

#### <a name="apidoc.element.blessed.textbox.textbox"></a>[function <span class="apidocSignatureSpan">blessed.</span>textbox (options)](#apidoc.element.blessed.textbox.textbox)
- description and source-code
```javascript
function Textbox(options) {
  if (!(this instanceof Node)) {
    return new Textbox(options);
  }

  options = options || {};

  options.scrollable = false;

  Textarea.call(this, options);

  this.secret = options.secret;
  this.censor = options.censor;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.textbox.prototype"></a>[module blessed.textbox.prototype](#apidoc.module.blessed.textbox.prototype)

#### <a name="apidoc.element.blessed.textbox.prototype.__olistener"></a>[function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>__olistener (ch, key)](#apidoc.element.blessed.textbox.prototype.__olistener)
- description and source-code
```javascript
__olistener = function (ch, key) {
  var done = this._done
    , value = this.value;

  if (key.name === 'return') return;
  if (key.name === 'enter') {
    ch = '\n';
  }

  // TODO: Handle directional keys.
  if (key.name === 'left' || key.name === 'right'
      || key.name === 'up' || key.name === 'down') {
    ;
  }

  if (this.options.keys && key.ctrl && key.name === 'e') {
    return this.readEditor();
  }

  // TODO: Optimize typing by writing directly
  // to the screen and screen buffer here.
  if (key.name === 'escape') {
    done(null, null);
  } else if (key.name === 'backspace') {
    if (this.value.length) {
      if (this.screen.fullUnicode) {
        if (unicode.isSurrogate(this.value, this.value.length - 2)) {
        // || unicode.isCombining(this.value, this.value.length - 1)) {
          this.value = this.value.slice(0, -2);
        } else {
          this.value = this.value.slice(0, -1);
        }
      } else {
        this.value = this.value.slice(0, -1);
      }
    }
  } else if (ch) {
    if (!/^[\x00-\x08\x0b-\x0c\x0e-\x1f\x7f]$/.test(ch)) {
      this.value += ch;
    }
  }

  if (this.value !== value) {
    this.screen.render();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textbox.prototype._listener"></a>[function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>_listener (ch, key)](#apidoc.element.blessed.textbox.prototype._listener)
- description and source-code
```javascript
_listener = function (ch, key) {
  if (key.name === 'enter') {
    this._done(null, this.value);
    return;
  }
  return this.__olistener(ch, key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textbox.prototype.setValue"></a>[function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>setValue (value)](#apidoc.element.blessed.textbox.prototype.setValue)
- description and source-code
```javascript
setValue = function (value) {
  var visible, val;
  if (value == null) {
    value = this.value;
  }
  if (this._value !== value) {
    value = value.replace(/\n/g, '');
    this.value = value;
    this._value = value;
    if (this.secret) {
      this.setContent('');
    } else if (this.censor) {
      this.setContent(Array(this.value.length + 1).join('*'));
    } else {
      visible = -(this.width - this.iwidth - 1);
      val = this.value.replace(/\t/g, this.screen.tabc);
      this.setContent(val.slice(visible));
    }
    this._updateCursor();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.textbox.prototype.submit"></a>[function <span class="apidocSignatureSpan">blessed.textbox.prototype.</span>submit ()](#apidoc.element.blessed.textbox.prototype.submit)
- description and source-code
```javascript
submit = function () {
  if (!this.__listener) return;
  return this.__listener('\r', { name: 'enter' });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.unicode"></a>[module blessed.unicode](#apidoc.module.blessed.unicode)

#### <a name="apidoc.element.blessed.unicode.charWidth"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>charWidth (str, i)](#apidoc.element.blessed.unicode.charWidth)
- description and source-code
```javascript
charWidth = function (str, i) {
  var point = typeof str !== 'number'
    ? exports.codePointAt(str, i || 0)
    : str;

  // nul
  if (point === 0) return 0;

  // tab
  if (point === 0x09) {
    if (!exports.blessed) {
      exports.blessed = require('../');
    }
    return exports.blessed.screen.global
      ? exports.blessed.screen.global.tabc.length
      : 8;
  }

  // 8-bit control characters (2-width according to unicode??)
  if (point < 32 || (point >= 0x7f && point < 0xa0)) {
    return 0;
  }

  // search table of non-spacing characters
  // is ucs combining or C0/C1 control character
  if (exports.combining[point]) {
    return 0;
  }

  // check for double-wide
  // if (point >= 0x1100
  //     && (point <= 0x115f // Hangul Jamo init. consonants
  //     || point === 0x2329 || point === 0x232a
  //     || (point >= 0x2e80 && point <= 0xa4cf
  //     && point !== 0x303f) // CJK ... Yi
  //     || (point >= 0xac00 && point <= 0xd7a3) // Hangul Syllables
  //     || (point >= 0xf900 && point <= 0xfaff) // CJK Compatibility Ideographs
  //     || (point >= 0xfe10 && point <= 0xfe19) // Vertical forms
  //     || (point >= 0xfe30 && point <= 0xfe6f) // CJK Compatibility Forms
  //     || (point >= 0xff00 && point <= 0xff60) // Fullwidth Forms
  //     || (point >= 0xffe0 && point <= 0xffe6)
  //     || (point >= 0x20000 && point <= 0x2fffd)
  //     || (point >= 0x30000 && point <= 0x3fffd))) {
  //   return 2;
  // }

  // check for double-wide
  if ((0x3000 === point)
      || (0xFF01 <= point && point <= 0xFF60)
      || (0xFFE0 <= point && point <= 0xFFE6)) {
    return 2;
  }

  if ((0x1100 <= point && point <= 0x115F)
      || (0x11A3 <= point && point <= 0x11A7)
      || (0x11FA <= point && point <= 0x11FF)
      || (0x2329 <= point && point <= 0x232A)
      || (0x2E80 <= point && point <= 0x2E99)
      || (0x2E9B <= point && point <= 0x2EF3)
      || (0x2F00 <= point && point <= 0x2FD5)
      || (0x2FF0 <= point && point <= 0x2FFB)
      || (0x3001 <= point && point <= 0x303E)
      || (0x3041 <= point && point <= 0x3096)
      || (0x3099 <= point && point <= 0x30FF)
      || (0x3105 <= point && point <= 0x312D)
      || (0x3131 <= point && point <= 0x318E)
      || (0x3190 <= point && point <= 0x31BA)
      || (0x31C0 <= point && point <= 0x31E3)
      || (0x31F0 <= point && point <= 0x321E)
      || (0x3220 <= point && point <= 0x3247)
      || (0x3250 <= point && point <= 0x32FE)
      || (0x3300 <= point && point <= 0x4DBF)
      || (0x4E00 <= point && point <= 0xA48C)
      || (0xA490 <= point && point <= 0xA4C6)
      || (0xA960 <= point && point <= 0xA97C)
      || (0xAC00 <= point && point <= 0xD7A3)
      || (0xD7B0 <= point && point <= 0xD7C6)
      || (0xD7CB <= point && point <= 0xD7FB)
      || (0xF900 <= point && point <= 0xFAFF)
      || (0xFE10 <= point && point <= 0xFE19)
      || (0xFE30 <= point && point <= 0xFE52)
      || (0xFE54 <= point && point <= 0xFE66)
      || (0xFE68 <= point && point <= 0xFE6B)
      || (0x1B000 <= point && point <= 0x1B001)
      || (0x1F200 <= point && point <= 0x1F202)
      || (0x1F210 <= point && point <= 0x1F23A)
      || (0x1F240 <= point && point <= 0x1F248)
      || (0x1F250 <= point && point <= 0x1F251)
      || (0x20000 <= point && point <= 0x2F73F)
      || (0x2B740 <= point && point <= 0x2FFFD)
      || (0x30000 <= point && point <= 0x3FFFD)) {
    return 2;
  }

  // CJK Ambiguous
  // http://www.unicode.org/reports/tr11/
  // http://www.unicode.org/reports/tr11/#Ambiguous
  if (process.env.NCURSES_CJK_WIDTH) {
    if ((0x00A1 === point)
        || (0x00A4 === point)
        || (0x00A7 <= point && point <= 0x00A8)
        || (0x00AA === point)
        || (0x00AD <= point && point <= 0x00AE)
        || (0x00B0 <= point && point <= 0x00B4)
        || (0x00B6 <= point && point <= 0x00BA)
        || (0x00BC <= point && point <= 0x00BF)
        || (0x00C6 === point)
        || (0x00D0 === point)
        || (0x00D7 <= point && point <= 0x00D8)
        || (0x00DE <= point && point <= 0x00E1)
        || (0x00E6 === point)
        || (0x00E8 <= point && point <= 0x ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.unicode.codePointAt"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>codePointAt (str, position)](#apidoc.element.blessed.unicode.codePointAt)
- description and source-code
```javascript
codePointAt = function (str, position) {
  if (str == null) {
    throw TypeError();
  }
  var string = String(str);
  if (string.codePointAt) {
    return string.codePointAt(position);
  }
  var size = string.length;
  // 'ToInteger'
  var index = position ? Number(position) : 0;
  if (index !== index) { // better 'isNaN'
    index = 0;
  }
  // Account for out-of-bounds indices:
  if (index < 0 || index >= size) {
    return undefined;
  }
  // Get the first code unit
  var first = string.charCodeAt(index);
  var second;
  if ( // check if it’s the start of a surrogate pair
    first >= 0xD800 && first <= 0xDBFF && // high surrogate
    size > index + 1 // there is a next code unit
  ) {
    second = string.charCodeAt(index + 1);
    if (second >= 0xDC00 && second <= 0xDFFF) { // low surrogate
      // http://mathiasbynens.be/notes/javascript-encoding#surrogate-formulae
      return (first - 0xD800) * 0x400 + second - 0xDC00 + 0x10000;
    }
  }
  return first;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.unicode.fromCodePoint"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>fromCodePoint ()](#apidoc.element.blessed.unicode.fromCodePoint)
- description and source-code
```javascript
fromCodePoint = function () {
  if (String.fromCodePoint) {
    return String.fromCodePoint.apply(String, arguments);
  }
  var MAX_SIZE = 0x4000;
  var codeUnits = [];
  var highSurrogate;
  var lowSurrogate;
  var index = -1;
  var length = arguments.length;
  if (!length) {
    return '';
  }
  var result = '';
  while (++index < length) {
    var codePoint = Number(arguments[index]);
    if (
      !isFinite(codePoint) ||       // 'NaN', '+Infinity', or '-Infinity'
      codePoint < 0 ||              // not a valid Unicode code point
      codePoint > 0x10FFFF ||       // not a valid Unicode code point
      floor(codePoint) !== codePoint // not an integer
    ) {
      throw RangeError('Invalid code point: ' + codePoint);
    }
    if (codePoint <= 0xFFFF) { // BMP code point
      codeUnits.push(codePoint);
    } else { // Astral code point; split in surrogate halves
      // http://mathiasbynens.be/notes/javascript-encoding#surrogate-formulae
      codePoint -= 0x10000;
      highSurrogate = (codePoint >> 10) + 0xD800;
      lowSurrogate = (codePoint % 0x400) + 0xDC00;
      codeUnits.push(highSurrogate, lowSurrogate);
    }
    if (index + 1 === length || codeUnits.length > MAX_SIZE) {
      result += stringFromCharCode.apply(null, codeUnits);
      codeUnits.length = 0;
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.unicode.isCombining"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>isCombining (str, i)](#apidoc.element.blessed.unicode.isCombining)
- description and source-code
```javascript
isCombining = function (str, i) {
  var point = typeof str !== 'number'
    ? exports.codePointAt(str, i || 0)
    : str;
  return exports.combining[point] === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.unicode.isSurrogate"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>isSurrogate (str, i)](#apidoc.element.blessed.unicode.isSurrogate)
- description and source-code
```javascript
isSurrogate = function (str, i) {
  var point = typeof str !== 'number'
    ? exports.codePointAt(str, i || 0)
    : str;
  return point > 0x00ffff;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.unicode.strWidth"></a>[function <span class="apidocSignatureSpan">blessed.unicode.</span>strWidth (str)](#apidoc.element.blessed.unicode.strWidth)
- description and source-code
```javascript
strWidth = function (str) {
  var width = 0;
  for (var i = 0; i < str.length; i++) {
    width += exports.charWidth(str, i);
    if (exports.isSurrogate(str, i)) i++;
  }
  return width;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.video"></a>[module blessed.video](#apidoc.module.blessed.video)

#### <a name="apidoc.element.blessed.video.video"></a>[function <span class="apidocSignatureSpan">blessed.</span>video (options)](#apidoc.element.blessed.video.video)
- description and source-code
```javascript
function Video(options) {
  var self = this
    , shell
    , args;

  if (!(this instanceof Node)) {
    return new Video(options);
  }

  options = options || {};

  Box.call(this, options);

  if (this.exists('mplayer')) {
    shell = 'mplayer';
    args = ['-vo', 'caca', '-quiet', options.file];
  } else if (this.exists('mpv')) {
    shell = 'mpv';
    args = ['--vo', 'caca', '--really-quiet', options.file];
  } else {
    this.parseTags = true;
    this.setContent('{red-fg}{bold}Error:{/bold}'
      + ' mplayer or mpv not installed.{/red-fg}');
    return this;
  }

  var opts = {
    parent: this,
    left: 0,
    top: 0,
    width: this.width - this.iwidth,
    height: this.height - this.iheight,
    shell: shell,
    args: args.slice()
  };

  this.now = Date.now() / 1000 | 0;
  this.start = opts.start || 0;
  if (this.start) {
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', this.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', this.start + '');
    }
  }

  var DISPLAY = process.env.DISPLAY;
  delete process.env.DISPLAY;
  this.tty = new Terminal(opts);
  process.env.DISPLAY = DISPLAY;

  this.on('click', function() {
    self.tty.pty.write('p');
  });

  // mplayer/mpv cannot resize itself in the terminal, so we have
  // to restart it at the correct start time.
  this.on('resize', function() {
    self.tty.destroy();

    var opts = {
      parent: self,
      left: 0,
      top: 0,
      width: self.width - self.iwidth,
      height: self.height - self.iheight,
      shell: shell,
      args: args.slice()
    };

    var watched = (Date.now() / 1000 | 0) - self.now;
    self.now = Date.now() / 1000 | 0;
    self.start += watched;
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', self.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', self.start + '');
    }

    var DISPLAY = process.env.DISPLAY;
    delete process.env.DISPLAY;
    self.tty = new Terminal(opts);
    process.env.DISPLAY = DISPLAY;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.video.prototype"></a>[module blessed.video.prototype](#apidoc.module.blessed.video.prototype)

#### <a name="apidoc.element.blessed.video.prototype.exists"></a>[function <span class="apidocSignatureSpan">blessed.video.prototype.</span>exists (program)](#apidoc.element.blessed.video.prototype.exists)
- description and source-code
```javascript
exists = function (program) {
  try {
    return !!+cp.execSync('type '
      + program + ' > /dev/null 2> /dev/null'
      + ' && echo 1', { encoding: 'utf8' }).trim();
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blessed.widget"></a>[module blessed.widget](#apidoc.module.blessed.widget)

#### <a name="apidoc.element.blessed.widget.ANSIImage"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ANSIImage (options)](#apidoc.element.blessed.widget.ANSIImage)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.BigText"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>BigText (options)](#apidoc.element.blessed.widget.BigText)
- description and source-code
```javascript
function BigText(options) {
  if (!(this instanceof Node)) {
    return new BigText(options);
  }
  options = options || {};
  options.font = options.font
    || __dirname + '/../../usr/fonts/ter-u14n.json';
  options.fontBold = options.font
    || __dirname + '/../../usr/fonts/ter-u14b.json';
  this.fch = options.fch;
  this.ratio = {};
  this.font = this.loadFont(options.font);
  this.fontBold = this.loadFont(options.font);
  Box.call(this, options);
  if (this.style.bold) {
    this.font = this.fontBold;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Box"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Box (options)](#apidoc.element.blessed.widget.Box)
- description and source-code
```javascript
function Box(options) {
  if (!(this instanceof Node)) {
    return new Box(options);
  }
  options = options || {};
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Button"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Button (options)](#apidoc.element.blessed.widget.Button)
- description and source-code
```javascript
function Button(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Button(options);
  }

  options = options || {};

  if (options.autoFocus == null) {
    options.autoFocus = false;
  }

  Input.call(this, options);

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      return self.press();
    }
  });

  if (this.options.mouse) {
    this.on('click', function() {
      return self.press();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Checkbox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Checkbox (options)](#apidoc.element.blessed.widget.Checkbox)
- description and source-code
```javascript
function Checkbox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Checkbox(options);
  }

  options = options || {};

  Input.call(this, options);

  this.text = options.content || options.text || '';
  this.checked = this.value = options.checked || false;

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      self.toggle();
      self.screen.render();
    }
  });

  if (options.mouse) {
    this.on('click', function() {
      self.toggle();
      self.screen.render();
    });
  }

  this.on('focus', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    self.screen.program.lsaveCursor('checkbox');
    self.screen.program.cup(lpos.yi, lpos.xi + 1);
    self.screen.program.showCursor();
  });

  this.on('blur', function() {
    self.screen.program.lrestoreCursor('checkbox', true);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Element"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Element (options)](#apidoc.element.blessed.widget.Element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.FileManager"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>FileManager (options)](#apidoc.element.blessed.widget.FileManager)
- description and source-code
```javascript
function FileManager(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new FileManager(options);
  }

  options = options || {};
  options.parseTags = true;
  // options.label = ' {blue-fg}%path{/blue-fg} ';

  List.call(this, options);

  this.cwd = options.cwd || process.cwd();
  this.file = this.cwd;
  this.value = this.cwd;

  if (options.label && ~options.label.indexOf('%path')) {
    this._label.setContent(options.label.replace('%path', this.cwd));
  }

  this.on('select', function(item) {
    var value = item.content.replace(/\{[^{}]+\}/g, '').replace(/@$/, '')
      , file = path.resolve(self.cwd, value);

    return fs.stat(file, function(err, stat) {
      if (err) {
        return self.emit('error', err, file);
      }
      self.file = file;
      self.value = file;
      if (stat.isDirectory()) {
        self.emit('cd', file, self.cwd);
        self.cwd = file;
        if (options.label && ~options.label.indexOf('%path')) {
          self._label.setContent(options.label.replace('%path', file));
        }
        self.refresh();
      } else {
        self.emit('file', file);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Form"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Form (options)](#apidoc.element.blessed.widget.Form)
- description and source-code
```javascript
function Form(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Form(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  Box.call(this, options);

  if (options.keys) {
    this.screen._listenKeys(this);
    this.on('element keypress', function(el, ch, key) {
      if ((key.name === 'tab' && !key.shift)
          || (el.type === 'textbox' && options.autoNext && key.name === 'enter')
          || key.name === 'down'
          || (options.vi && key.name === 'j')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'j') return;
          if (key.name === 'tab') {
            // Workaround, since we can't stop the tab from being added.
            el.emit('keypress', null, { name: 'backspace' });
          }
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusNext();
        return;
      }

      if ((key.name === 'tab' && key.shift)
          || key.name === 'up'
          || (options.vi && key.name === 'k')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'k') return;
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusPrevious();
        return;
      }

      if (key.name === 'escape') {
        self.focus();
        return;
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Image"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Image (options)](#apidoc.element.blessed.widget.Image)
- description and source-code
```javascript
function Image(options) {
  if (!(this instanceof Node)) {
    return new Image(options);
  }

  options = options || {};
  options.type = options.itype || options.type || 'ansi';

  Box.call(this, options);

  if (options.type === 'ansi' && this.type !== 'ansiimage') {
    var ANSIImage = require('./ansiimage');
    Object.getOwnPropertyNames(ANSIImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ANSIImage.prototype, key));
    }, this);
    ANSIImage.call(this, options);
    return this;
  }

  if (options.type === 'overlay' && this.type !== 'overlayimage') {
    var OverlayImage = require('./overlayimage');
    Object.getOwnPropertyNames(OverlayImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(OverlayImage.prototype, key));
    }, this);
    OverlayImage.call(this, options);
    return this;
  }

  throw new Error(''type' must either be 'ansi' or 'overlay'.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Input"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Input (options)](#apidoc.element.blessed.widget.Input)
- description and source-code
```javascript
function Input(options) {
  if (!(this instanceof Node)) {
    return new Input(options);
  }
  options = options || {};
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Layout"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Layout (options)](#apidoc.element.blessed.widget.Layout)
- description and source-code
```javascript
function Layout(options) {
  if (!(this instanceof Node)) {
    return new Layout(options);
  }

  options = options || {};

  if ((options.width == null
      && (options.left == null && options.right == null))
      || (options.height == null
      && (options.top == null && options.bottom == null))) {
    throw new Error(''Layout' must have a width and height!');
  }

  options.layout = options.layout || 'inline';

  Element.call(this, options);

  if (options.renderer) {
    this.renderer = options.renderer;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Line"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Line (options)](#apidoc.element.blessed.widget.Line)
- description and source-code
```javascript
function Line(options) {
  if (!(this instanceof Node)) {
    return new Line(options);
  }

  options = options || {};

  var orientation = options.orientation || 'vertical';
  delete options.orientation;

  if (orientation === 'vertical') {
    options.width = 1;
  } else {
    options.height = 1;
  }

  Box.call(this, options);

  this.ch = !options.type || options.type === 'line'
    ? orientation === 'horizontal' ? '─' : '│'
    : options.ch || ' ';

  this.border = {
    type: 'bg',
    __proto__: this
  };

  this.style.border = this.style;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.List"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>List (options)](#apidoc.element.blessed.widget.List)
- description and source-code
```javascript
function List(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new List(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  // Possibly put this here: this.items = [];
  options.scrollable = true;
  Box.call(this, options);

  this.value = '';
  this.items = [];
  this.ritems = [];
  this.selected = 0;
  this._isList = true;

  if (!this.style.selected) {
    this.style.selected = {};
    this.style.selected.bg = options.selectedBg;
    this.style.selected.fg = options.selectedFg;
    this.style.selected.bold = options.selectedBold;
    this.style.selected.underline = options.selectedUnderline;
    this.style.selected.blink = options.selectedBlink;
    this.style.selected.inverse = options.selectedInverse;
    this.style.selected.invisible = options.selectedInvisible;
  }

  if (!this.style.item) {
    this.style.item = {};
    this.style.item.bg = options.itemBg;
    this.style.item.fg = options.itemFg;
    this.style.item.bold = options.itemBold;
    this.style.item.underline = options.itemUnderline;
    this.style.item.blink = options.itemBlink;
    this.style.item.inverse = options.itemInverse;
    this.style.item.invisible = options.itemInvisible;
  }

  // Legacy: for apps written before the addition of item attributes.
  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    if (self.style[name] != null && self.style.item[name] == null) {
      self.style.item[name] = self.style[name];
    }
  });

  if (this.options.itemHoverBg) {
    this.options.itemHoverEffects = { bg: this.options.itemHoverBg };
  }

  if (this.options.itemHoverEffects) {
    this.style.item.hover = this.options.itemHoverEffects;
  }

  if (this.options.itemFocusEffects) {
    this.style.item.focus = this.options.itemFocusEffects;
  }

  this.interactive = options.interactive !== false;

  this.mouse = options.mouse || false;

  if (options.items) {
    this.ritems = options.items;
    options.items.forEach(this.add.bind(this));
  }

  this.select(0);

  if (options.mouse) {
    this.screen._listenMouse(this);
    this.on('element wheeldown', function() {
      self.select(self.selected + 2);
      self.screen.render();
    });
    this.on('element wheelup', function() {
      self.select(self.selected - 2);
      self.screen.render();
    });
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.up();
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.down();
        self.screen.render();
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'l' && !key.shift)) {
        self.enterSelected();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.cancelSelected();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.move(-((self.height - self.iheight) / 2) | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.move((self.height - self.iheight) / 2 | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'b' && key.ctrl) {
        self.move(-(self.height - self.iheight));
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'f' && key.ctrl) {
        self.move(self.height - self.iheight);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'h' && key.shift) {
        self.move(self.childBase - self.selected);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'm' && key.shift) {
        // TODO: Maybe use Math.min(this.items.length,
        // ... for calculating visible items elsewhere.
        var visible = Math.min(
          self.height - self.iheight,
          self.items.length) / 2 | 0;
        self.move(sel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ListBar"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ListBar (options)](#apidoc.element.blessed.widget.ListBar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ListTable"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ListTable (options)](#apidoc.element.blessed.widget.ListTable)
- description and source-code
```javascript
function ListTable(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ListTable(options);
  }

  options = options || {};
  options.shrink = true;
  options.normalShrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  this.__align = options.align || 'center';
  delete options.align;

  options.style.selected = options.style.cell.selected;
  options.style.item = options.style.cell;

  List.call(this, options);

  this._header = new Box({
    parent: this,
    left: this.screen.autoPadding ? 0 : this.ileft,
    top: 0,
    width: 'shrink',
    height: 1,
    style: options.style.header,
    tags: options.parseTags || options.tags
  });

  this.on('scroll', function() {
    self._header.setFront();
    self._header.rtop = self.childBase;
    if (!self.screen.autoPadding) {
      self._header.rtop = self.childBase + (self.border ? 1 : 0);
    }
  });

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setData(self.rows);
  });

  this.on('resize', function() {
    var selected = self.selected;
    self.setData(self.rows);
    self.select(selected);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Listbar"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Listbar (options)](#apidoc.element.blessed.widget.Listbar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Loading"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Loading (options)](#apidoc.element.blessed.widget.Loading)
- description and source-code
```javascript
function Loading(options) {
  if (!(this instanceof Node)) {
    return new Loading(options);
  }

  options = options || {};

  Box.call(this, options);

  this._.icon = new Text({
    parent: this,
    align: 'center',
    top: 2,
    left: 1,
    right: 1,
    height: 1,
    content: '|'
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Log"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Log (options)](#apidoc.element.blessed.widget.Log)
- description and source-code
```javascript
function Log(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Log(options);
  }

  options = options || {};

  ScrollableText.call(this, options);

  this.scrollback = options.scrollback != null
    ? options.scrollback
    : Infinity;
  this.scrollOnInput = options.scrollOnInput;

  this.on('set content', function() {
    if (!self._userScrolled || self.scrollOnInput) {
      nextTick(function() {
        self.setScrollPerc(100);
        self._userScrolled = false;
        self.screen.render();
      });
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Message"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Message (options)](#apidoc.element.blessed.widget.Message)
- description and source-code
```javascript
function Message(options) {
  if (!(this instanceof Node)) {
    return new Message(options);
  }

  options = options || {};
  options.tags = true;

  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Node"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Node (options)](#apidoc.element.blessed.widget.Node)
- description and source-code
```javascript
function Node(options) {
  var self = this;
  var Screen = require('./screen');

  if (!(this instanceof Node)) {
    return new Node(options);
  }

  EventEmitter.call(this);

  options = options || {};
  this.options = options;

  this.screen = this.screen || options.screen;

  if (!this.screen) {
    if (this.type === 'screen') {
      this.screen = this;
    } else if (Screen.total === 1) {
      this.screen = Screen.global;
    } else if (options.parent) {
      this.screen = options.parent;
      while (this.screen && this.screen.type !== 'screen') {
        this.screen = this.screen.parent;
      }
    } else if (Screen.total) {
      // This _should_ work in most cases as long as the element is appended
      // synchronously after the screen's creation. Throw error if not.
      this.screen = Screen.instances[Screen.instances.length - 1];
      process.nextTick(function() {
        if (!self.parent) {
          throw new Error('Element (' + self.type + ')'
            + ' was not appended synchronously after the'
            + ' screen\'s creation. Please set a 'parent''
            + ' or 'screen' option in the element\'s constructor'
            + ' if you are going to use multiple screens and'
            + ' append the element later.');
        }
      });
    } else {
      throw new Error('No active screen.');
    }
  }

  this.parent = options.parent || null;
  this.children = [];
  this.$ = this._ = this.data = {};
  this.uid = Node.uid++;
  this.index = this.index != null ? this.index : -1;

  if (this.type !== 'screen') {
    this.detached = true;
  }

  if (this.parent) {
    this.parent.append(this);
  }

  (options.children || []).forEach(this.append.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.OverlayImage"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>OverlayImage (options)](#apidoc.element.blessed.widget.OverlayImage)
- description and source-code
```javascript
function OverlayImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new OverlayImage(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.w3m) {
    OverlayImage.w3mdisplay = options.w3m;
  }

  if (OverlayImage.hasW3MDisplay == null) {
    if (fs.existsSync(OverlayImage.w3mdisplay)) {
      OverlayImage.hasW3MDisplay = true;
    } else if (options.search !== false) {
      var file = helpers.findFile('/usr', 'w3mimgdisplay')
              || helpers.findFile('/lib', 'w3mimgdisplay')
              || helpers.findFile('/bin', 'w3mimgdisplay');
      if (file) {
        OverlayImage.hasW3MDisplay = true;
        OverlayImage.w3mdisplay = file;
      } else {
        OverlayImage.hasW3MDisplay = false;
      }
    }
  }

  this.on('hide', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('show', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.on('detach', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('attach', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.onScreenEvent('resize', function() {
    self._needsRatio = true;
  });

  // Get images to overlap properly. Maybe not worth it:
  // this.onScreenEvent('render', function() {
  //   self.screen.program.flush();
  //   if (!self._noImage) return;
  //   function display(el, next) {
  //     if (el.type === 'w3mimage' && el.file) {
  //       el.setImage(el.file, next);
  //     } else {
  //       next();
  //     }
  //   }
  //   function done(el) {
  //     el.children.forEach(recurse);
  //   }
  //   function recurse(el) {
  //     display(el, function() {
  //       var pending = el.children.length;
  //       el.children.forEach(function(el) {
  //         display(el, function() {
  //           if (!--pending) done(el);
  //         });
  //       });
  //     });
  //   }
  //   recurse(self.screen);
  // });

  this.onScreenEvent('render', function() {
    self.screen.program.flush();
    if (!self._noImage) {
      self.setImage(self.file);
    }
  });

  if (this.options.file || this.options.img) {
    this.setImage(this.options.file || this.options.img);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.PNG"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>PNG (options)](#apidoc.element.blessed.widget.PNG)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ProgressBar"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ProgressBar (options)](#apidoc.element.blessed.widget.ProgressBar)
- description and source-code
```javascript
function ProgressBar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ProgressBar(options);
  }

  options = options || {};

  Input.call(this, options);

  this.filled = options.filled || 0;
  if (typeof this.filled === 'string') {
    this.filled = +this.filled.slice(0, -1);
  }
  this.value = this.filled;

  this.pch = options.pch || ' ';

  // XXX Workaround that predates the usage of 'el.ch'.
  if (options.ch) {
    this.pch = options.ch;
    this.ch = ' ';
  }
  if (options.bch) {
    this.ch = options.bch;
  }

  if (!this.style.bar) {
    this.style.bar = {};
    this.style.bar.fg = options.barFg;
    this.style.bar.bg = options.barBg;
  }

  this.orientation = options.orientation || 'horizontal';

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      var back, forward;
      if (self.orientation === 'horizontal') {
        back = ['left', 'h'];
        forward = ['right', 'l'];
      } else if (self.orientation === 'vertical') {
        back = ['down', 'j'];
        forward = ['up', 'k'];
      }
      if (key.name === back[0] || (options.vi && key.name === back[1])) {
        self.progress(-5);
        self.screen.render();
        return;
      }
      if (key.name === forward[0] || (options.vi && key.name === forward[1])) {
        self.progress(5);
        self.screen.render();
        return;
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      var x, y, m, p;
      if (!self.lpos) return;
      if (self.orientation === 'horizontal') {
        x = data.x - self.lpos.xi;
        m = (self.lpos.xl - self.lpos.xi) - self.iwidth;
        p = x / m * 100 | 0;
      } else if (self.orientation === 'vertical') {
        y = data.y - self.lpos.yi;
        m = (self.lpos.yl - self.lpos.yi) - self.iheight;
        p = y / m * 100 | 0;
      }
      self.setProgress(p);
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Prompt"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Prompt (options)](#apidoc.element.blessed.widget.Prompt)
- description and source-code
```javascript
function Prompt(options) {
  if (!(this instanceof Node)) {
    return new Prompt(options);
  }

  options = options || {};

  options.hidden = true;

  Box.call(this, options);

  this._.input = new Textbox({
    parent: this,
    top: 3,
    height: 1,
    left: 2,
    right: 2,
    bg: 'black'
  });

  this._.okay = new Button({
    parent: this,
    top: 5,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    parent: this,
    top: 5,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Question"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Question (options)](#apidoc.element.blessed.widget.Question)
- description and source-code
```javascript
function Question(options) {
  if (!(this instanceof Node)) {
    return new Question(options);
  }

  options = options || {};
  options.hidden = true;

  Box.call(this, options);

  this._.okay = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.RadioButton"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>RadioButton (options)](#apidoc.element.blessed.widget.RadioButton)
- description and source-code
```javascript
function RadioButton(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new RadioButton(options);
  }

  options = options || {};

  Checkbox.call(this, options);

  this.on('check', function() {
    var el = self;
    while (el = el.parent) {
      if (el.type === 'radio-set'
          || el.type === 'form') break;
    }
    el = el || self.parent;
    el.forDescendants(function(el) {
      if (el.type !== 'radio-button' || el === self) {
        return;
      }
      el.uncheck();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.RadioSet"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>RadioSet (options)](#apidoc.element.blessed.widget.RadioSet)
- description and source-code
```javascript
function RadioSet(options) {
  if (!(this instanceof Node)) {
    return new RadioSet(options);
  }
  options = options || {};
  // Possibly inherit parent's style.
  // options.style = this.parent.style;
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Screen"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Screen (options)](#apidoc.element.blessed.widget.Screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ScrollableBox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ScrollableBox (options)](#apidoc.element.blessed.widget.ScrollableBox)
- description and source-code
```javascript
function ScrollableBox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ScrollableBox(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.scrollable === false) {
    return this;
  }

  this.scrollable = true;
  this.childOffset = 0;
  this.childBase = 0;
  this.baseLimit = options.baseLimit || Infinity;
  this.alwaysScroll = options.alwaysScroll;

  this.scrollbar = options.scrollbar;
  if (this.scrollbar) {
    this.scrollbar.ch = this.scrollbar.ch || ' ';
    this.style.scrollbar = this.style.scrollbar || this.scrollbar.style;
    if (!this.style.scrollbar) {
      this.style.scrollbar = {};
      this.style.scrollbar.fg = this.scrollbar.fg;
      this.style.scrollbar.bg = this.scrollbar.bg;
      this.style.scrollbar.bold = this.scrollbar.bold;
      this.style.scrollbar.underline = this.scrollbar.underline;
      this.style.scrollbar.inverse = this.scrollbar.inverse;
      this.style.scrollbar.invisible = this.scrollbar.invisible;
    }
    //this.scrollbar.style = this.style.scrollbar;
    if (this.track || this.scrollbar.track) {
      this.track = this.scrollbar.track || this.track;
      this.style.track = this.style.scrollbar.track || this.style.track;
      this.track.ch = this.track.ch || ' ';
      this.style.track = this.style.track || this.track.style;
      if (!this.style.track) {
        this.style.track = {};
        this.style.track.fg = this.track.fg;
        this.style.track.bg = this.track.bg;
        this.style.track.bold = this.track.bold;
        this.style.track.underline = this.track.underline;
        this.style.track.inverse = this.track.inverse;
        this.style.track.invisible = this.track.invisible;
      }
      this.track.style = this.style.track;
    }
    // Allow controlling of the scrollbar via the mouse:
    if (options.mouse) {
      this.on('mousedown', function(data) {
        if (self._scrollingBar) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          return;
        }
        var x = data.x - self.aleft;
        var y = data.y - self.atop;
        if (x === self.width - self.iright - 1) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          var perc = (y - self.itop) / (self.height - self.iheight);
          self.setScrollPerc(perc * 100 | 0);
          self.screen.render();
          var smd, smu;
          self._scrollingBar = true;
          self.onScreenEvent('mousedown', smd = function(data) {
            var y = data.y - self.atop;
            var perc = y / self.height;
            self.setScrollPerc(perc * 100 | 0);
            self.screen.render();
          });
          // If mouseup occurs out of the window, no mouseup event fires, and
          // scrollbar will drag again on mousedown until another mouseup
          // occurs.
          self.onScreenEvent('mouseup', smu = function() {
            self._scrollingBar = false;
            self.removeScreenEvent('mousedown', smd);
            self.removeScreenEvent('mouseup', smu);
          });
        }
      });
    }
  }

  if (options.mouse) {
    this.on('wheeldown', function() {
      self.scroll(self.height / 2 | 0 || 1);
      self.screen.render();
    });
    this.on('wheelup', function() {
      self.scroll(-(self.height / 2 | 0) || -1);
      self.screen.render();
    });
  }

  if (options.keys && !options.ignoreKeys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.scroll(-1);
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.scroll(1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.scroll(-(self.height / 2 | 0) || -1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.scroll( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ScrollableText"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ScrollableText (options)](#apidoc.element.blessed.widget.ScrollableText)
- description and source-code
```javascript
function ScrollableText(options) {
  if (!(this instanceof Node)) {
    return new ScrollableText(options);
  }
  options = options || {};
  options.alwaysScroll = true;
  ScrollableBox.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Table"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Table (options)](#apidoc.element.blessed.widget.Table)
- description and source-code
```javascript
function Table(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Table(options);
  }

  options = options || {};
  options.shrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  options.align = options.align || 'center';

  // Regular tables do not get custom height (this would
  // require extra padding). Maybe add in the future.
  delete options.height;

  Box.call(this, options);

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setContent('');
    self.setData(self.rows);
  });

  this.on('resize', function() {
    self.setContent('');
    self.setData(self.rows);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Terminal"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Terminal (options)](#apidoc.element.blessed.widget.Terminal)
- description and source-code
```javascript
function Terminal(options) {
  if (!(this instanceof Node)) {
    return new Terminal(options);
  }

  options = options || {};
  options.scrollable = false;

  Box.call(this, options);

  // XXX Workaround for all motion
  if (this.screen.program.tmux && this.screen.program.tmuxVersion >= 2) {
    this.screen.program.enableMouse();
  }

  this.handler = options.handler;
  this.shell = options.shell || process.env.SHELL || 'sh';
  this.args = options.args || [];

  this.cursor = this.options.cursor;
  this.cursorBlink = this.options.cursorBlink;
  this.screenKeys = this.options.screenKeys;

  this.style = this.style || {};
  this.style.bg = this.style.bg || 'default';
  this.style.fg = this.style.fg || 'default';

  this.termName = options.terminal
    || options.term
    || process.env.TERM
    || 'xterm';

  this.bootstrap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Text"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Text (options)](#apidoc.element.blessed.widget.Text)
- description and source-code
```javascript
function Text(options) {
  if (!(this instanceof Node)) {
    return new Text(options);
  }
  options = options || {};
  options.shrink = true;
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Textarea"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Textarea (options)](#apidoc.element.blessed.widget.Textarea)
- description and source-code
```javascript
function Textarea(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Textarea(options);
  }

  options = options || {};

  options.scrollable = options.scrollable !== false;

  Input.call(this, options);

  this.screen._listenKeys(this);

  this.value = options.value || '';

  this.__updateCursor = this._updateCursor.bind(this);
  this.on('resize', this.__updateCursor);
  this.on('move', this.__updateCursor);

  if (options.inputOnFocus) {
    this.on('focus', this.readInput.bind(this, null));
  }

  if (!options.inputOnFocus && options.keys) {
    this.on('keypress', function(ch, key) {
      if (self._reading) return;
      if (key.name === 'enter' || (options.vi && key.name === 'i')) {
        return self.readInput();
      }
      if (key.name === 'e') {
        return self.readEditor();
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      if (self._reading) return;
      if (data.button !== 'right') return;
      self.readEditor();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Textbox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Textbox (options)](#apidoc.element.blessed.widget.Textbox)
- description and source-code
```javascript
function Textbox(options) {
  if (!(this instanceof Node)) {
    return new Textbox(options);
  }

  options = options || {};

  options.scrollable = false;

  Textarea.call(this, options);

  this.secret = options.secret;
  this.censor = options.censor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.Video"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>Video (options)](#apidoc.element.blessed.widget.Video)
- description and source-code
```javascript
function Video(options) {
  var self = this
    , shell
    , args;

  if (!(this instanceof Node)) {
    return new Video(options);
  }

  options = options || {};

  Box.call(this, options);

  if (this.exists('mplayer')) {
    shell = 'mplayer';
    args = ['-vo', 'caca', '-quiet', options.file];
  } else if (this.exists('mpv')) {
    shell = 'mpv';
    args = ['--vo', 'caca', '--really-quiet', options.file];
  } else {
    this.parseTags = true;
    this.setContent('{red-fg}{bold}Error:{/bold}'
      + ' mplayer or mpv not installed.{/red-fg}');
    return this;
  }

  var opts = {
    parent: this,
    left: 0,
    top: 0,
    width: this.width - this.iwidth,
    height: this.height - this.iheight,
    shell: shell,
    args: args.slice()
  };

  this.now = Date.now() / 1000 | 0;
  this.start = opts.start || 0;
  if (this.start) {
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', this.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', this.start + '');
    }
  }

  var DISPLAY = process.env.DISPLAY;
  delete process.env.DISPLAY;
  this.tty = new Terminal(opts);
  process.env.DISPLAY = DISPLAY;

  this.on('click', function() {
    self.tty.pty.write('p');
  });

  // mplayer/mpv cannot resize itself in the terminal, so we have
  // to restart it at the correct start time.
  this.on('resize', function() {
    self.tty.destroy();

    var opts = {
      parent: self,
      left: 0,
      top: 0,
      width: self.width - self.iwidth,
      height: self.height - self.iheight,
      shell: shell,
      args: args.slice()
    };

    var watched = (Date.now() / 1000 | 0) - self.now;
    self.now = Date.now() / 1000 | 0;
    self.start += watched;
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', self.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', self.start + '');
    }

    var DISPLAY = process.env.DISPLAY;
    delete process.env.DISPLAY;
    self.tty = new Terminal(opts);
    process.env.DISPLAY = DISPLAY;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.ansiimage"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>ansiimage (options)](#apidoc.element.blessed.widget.ansiimage)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.bigtext"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>bigtext (options)](#apidoc.element.blessed.widget.bigtext)
- description and source-code
```javascript
function BigText(options) {
  if (!(this instanceof Node)) {
    return new BigText(options);
  }
  options = options || {};
  options.font = options.font
    || __dirname + '/../../usr/fonts/ter-u14n.json';
  options.fontBold = options.font
    || __dirname + '/../../usr/fonts/ter-u14b.json';
  this.fch = options.fch;
  this.ratio = {};
  this.font = this.loadFont(options.font);
  this.fontBold = this.loadFont(options.font);
  Box.call(this, options);
  if (this.style.bold) {
    this.font = this.fontBold;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.box"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>box (options)](#apidoc.element.blessed.widget.box)
- description and source-code
```javascript
function Box(options) {
  if (!(this instanceof Node)) {
    return new Box(options);
  }
  options = options || {};
  Element.call(this, options);
}
```
- example usage
```shell
...
var screen = blessed.screen({
smartCSR: true
});

screen.title = 'my window title';

// Create a box perfectly centered horizontally and vertically.
var box = blessed.box({
top: 'center',
left: 'center',
width: '50%',
height: '50%',
content: 'Hello {bold}world{/bold}!',
tags: true,
border: {
...
```

#### <a name="apidoc.element.blessed.widget.button"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>button (options)](#apidoc.element.blessed.widget.button)
- description and source-code
```javascript
function Button(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Button(options);
  }

  options = options || {};

  if (options.autoFocus == null) {
    options.autoFocus = false;
  }

  Input.call(this, options);

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      return self.press();
    }
  });

  if (this.options.mouse) {
    this.on('click', function() {
      return self.press();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.checkbox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>checkbox (options)](#apidoc.element.blessed.widget.checkbox)
- description and source-code
```javascript
function Checkbox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Checkbox(options);
  }

  options = options || {};

  Input.call(this, options);

  this.text = options.content || options.text || '';
  this.checked = this.value = options.checked || false;

  this.on('keypress', function(ch, key) {
    if (key.name === 'enter' || key.name === 'space') {
      self.toggle();
      self.screen.render();
    }
  });

  if (options.mouse) {
    this.on('click', function() {
      self.toggle();
      self.screen.render();
    });
  }

  this.on('focus', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    self.screen.program.lsaveCursor('checkbox');
    self.screen.program.cup(lpos.yi, lpos.xi + 1);
    self.screen.program.showCursor();
  });

  this.on('blur', function() {
    self.screen.program.lrestoreCursor('checkbox', true);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.element"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>element (options)](#apidoc.element.blessed.widget.element)
- description and source-code
```javascript
function Element(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Element(options);
  }

  options = options || {};

  // Workaround to get a 'scrollable' option.
  if (options.scrollable && !this._ignore && this.type !== 'scrollable-box') {
    var ScrollableBox = require('./scrollablebox');
    Object.getOwnPropertyNames(ScrollableBox.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ScrollableBox.prototype, key));
    }, this);
    this._ignore = true;
    ScrollableBox.call(this, options);
    delete this._ignore;
    return this;
  }

  Node.call(this, options);

  this.name = options.name;

  options.position = options.position || {
    left: options.left,
    right: options.right,
    top: options.top,
    bottom: options.bottom,
    width: options.width,
    height: options.height
  };

  if (options.position.width === 'shrink'
      || options.position.height === 'shrink') {
    if (options.position.width === 'shrink') {
      delete options.position.width;
    }
    if (options.position.height === 'shrink') {
      delete options.position.height;
    }
    options.shrink = true;
  }

  this.position = options.position;

  this.noOverflow = options.noOverflow;
  this.dockBorders = options.dockBorders;
  this.shadow = options.shadow;

  this.style = options.style;

  if (!this.style) {
    this.style = {};
    this.style.fg = options.fg;
    this.style.bg = options.bg;
    this.style.bold = options.bold;
    this.style.underline = options.underline;
    this.style.blink = options.blink;
    this.style.inverse = options.inverse;
    this.style.invisible = options.invisible;
    this.style.transparent = options.transparent;
  }

  this.hidden = options.hidden || false;
  this.fixed = options.fixed || false;
  this.align = options.align || 'left';
  this.valign = options.valign || 'top';
  this.wrap = options.wrap !== false;
  this.shrink = options.shrink;
  this.fixed = options.fixed;
  this.ch = options.ch || ' ';

  if (typeof options.padding === 'number' || !options.padding) {
    options.padding = {
      left: options.padding,
      top: options.padding,
      right: options.padding,
      bottom: options.padding
    };
  }

  this.padding = {
    left: options.padding.left || 0,
    top: options.padding.top || 0,
    right: options.padding.right || 0,
    bottom: options.padding.bottom || 0
  };

  this.border = options.border;
  if (this.border) {
    if (typeof this.border === 'string') {
      this.border = { type: this.border };
    }
    this.border.type = this.border.type || 'bg';
    if (this.border.type === 'ascii') this.border.type = 'line';
    this.border.ch = this.border.ch || ' ';
    this.style.border = this.style.border || this.border.style;
    if (!this.style.border) {
      this.style.border = {};
      this.style.border.fg = this.border.fg;
      this.style.border.bg = this.border.bg;
    }
    //this.border.style = this.style.border;
    if (this.border.left == null) this.border.left = true;
    if (this.border.top == null) this.border.top = true;
    if (this.border.right == null) this.border.right = true;
    if (this.border.bottom == null) this.border.bottom = true;
  }

  // if (options.mouse || options.clickable) {
  if (options.clickable) {
    this.screen._listenMouse(this);
  }

  if (options.input || options.keyable) {
    this.screen._listenKeys(this);
  }

  this.parseTags = options.parseTags || options.tags;

  this.setContent(options.content || '', true);

  if (options.label) {
    this.setLabel(options.label);
  }

  if (options.hoverText) {
    this.setHover(options.hoverText);
  }

  // TODO: Possibly move this to Node for onScreenEvent('mouse', ...).
  this.on('newListener', function fn(type) {
    // type = type.split(' ').slice(1).join(' ');
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      | ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.filemanager"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>filemanager (options)](#apidoc.element.blessed.widget.filemanager)
- description and source-code
```javascript
function FileManager(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new FileManager(options);
  }

  options = options || {};
  options.parseTags = true;
  // options.label = ' {blue-fg}%path{/blue-fg} ';

  List.call(this, options);

  this.cwd = options.cwd || process.cwd();
  this.file = this.cwd;
  this.value = this.cwd;

  if (options.label && ~options.label.indexOf('%path')) {
    this._label.setContent(options.label.replace('%path', this.cwd));
  }

  this.on('select', function(item) {
    var value = item.content.replace(/\{[^{}]+\}/g, '').replace(/@$/, '')
      , file = path.resolve(self.cwd, value);

    return fs.stat(file, function(err, stat) {
      if (err) {
        return self.emit('error', err, file);
      }
      self.file = file;
      self.value = file;
      if (stat.isDirectory()) {
        self.emit('cd', file, self.cwd);
        self.cwd = file;
        if (options.label && ~options.label.indexOf('%path')) {
          self._label.setContent(options.label.replace('%path', file));
        }
        self.refresh();
      } else {
        self.emit('file', file);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.form"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>form (options)](#apidoc.element.blessed.widget.form)
- description and source-code
```javascript
function Form(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Form(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  Box.call(this, options);

  if (options.keys) {
    this.screen._listenKeys(this);
    this.on('element keypress', function(el, ch, key) {
      if ((key.name === 'tab' && !key.shift)
          || (el.type === 'textbox' && options.autoNext && key.name === 'enter')
          || key.name === 'down'
          || (options.vi && key.name === 'j')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'j') return;
          if (key.name === 'tab') {
            // Workaround, since we can't stop the tab from being added.
            el.emit('keypress', null, { name: 'backspace' });
          }
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusNext();
        return;
      }

      if ((key.name === 'tab' && key.shift)
          || key.name === 'up'
          || (options.vi && key.name === 'k')) {
        if (el.type === 'textbox' || el.type === 'textarea') {
          if (key.name === 'k') return;
          el.emit('keypress', '\x1b', { name: 'escape' });
        }
        self.focusPrevious();
        return;
      }

      if (key.name === 'escape') {
        self.focus();
        return;
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.image"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>image (options)](#apidoc.element.blessed.widget.image)
- description and source-code
```javascript
function Image(options) {
  if (!(this instanceof Node)) {
    return new Image(options);
  }

  options = options || {};
  options.type = options.itype || options.type || 'ansi';

  Box.call(this, options);

  if (options.type === 'ansi' && this.type !== 'ansiimage') {
    var ANSIImage = require('./ansiimage');
    Object.getOwnPropertyNames(ANSIImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(ANSIImage.prototype, key));
    }, this);
    ANSIImage.call(this, options);
    return this;
  }

  if (options.type === 'overlay' && this.type !== 'overlayimage') {
    var OverlayImage = require('./overlayimage');
    Object.getOwnPropertyNames(OverlayImage.prototype).forEach(function(key) {
      if (key === 'type') return;
      Object.defineProperty(this, key,
        Object.getOwnPropertyDescriptor(OverlayImage.prototype, key));
    }, this);
    OverlayImage.call(this, options);
    return this;
  }

  throw new Error(''type' must either be 'ansi' or 'overlay'.');
}
```
- example usage
```shell
...
}
});

// Append our box to the screen.
screen.append(box);

// Add a png icon to the box
var icon = blessed.image({
parent: box,
top: 0,
left: 0,
type: 'overlay',
width: 'shrink',
height: 'shrink',
file: __dirname + '/my-program-icon.png',
...
```

#### <a name="apidoc.element.blessed.widget.input"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>input (options)](#apidoc.element.blessed.widget.input)
- description and source-code
```javascript
function Input(options) {
  if (!(this instanceof Node)) {
    return new Input(options);
  }
  options = options || {};
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.layout"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>layout (options)](#apidoc.element.blessed.widget.layout)
- description and source-code
```javascript
function Layout(options) {
  if (!(this instanceof Node)) {
    return new Layout(options);
  }

  options = options || {};

  if ((options.width == null
      && (options.left == null && options.right == null))
      || (options.height == null
      && (options.top == null && options.bottom == null))) {
    throw new Error(''Layout' must have a width and height!');
  }

  options.layout = options.layout || 'inline';

  Element.call(this, options);

  if (options.renderer) {
    this.renderer = options.renderer;
  }
}
```
- example usage
```shell
...

Here is an example of how to provide a renderer. Note that this is also the
default renderer if none is provided. This renderer will render each child as
though they were 'display: inline-block;' in CSS, as if there were a
dynamically sized horizontal grid from left to right.

''' js
var layout = blessed.layout({
parent: screen,
top: 'center',
left: 'center',
width: '50%',
height: '50%',
border: 'line',
style: {
...
```

#### <a name="apidoc.element.blessed.widget.line"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>line (options)](#apidoc.element.blessed.widget.line)
- description and source-code
```javascript
function Line(options) {
  if (!(this instanceof Node)) {
    return new Line(options);
  }

  options = options || {};

  var orientation = options.orientation || 'vertical';
  delete options.orientation;

  if (orientation === 'vertical') {
    options.width = 1;
  } else {
    options.height = 1;
  }

  Box.call(this, options);

  this.ch = !options.type || options.type === 'line'
    ? orientation === 'horizontal' ? '─' : '│'
    : options.ch || ' ';

  this.border = {
    type: 'bg',
    __proto__: this
  };

  this.style.border = this.style;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.list"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>list (options)](#apidoc.element.blessed.widget.list)
- description and source-code
```javascript
function List(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new List(options);
  }

  options = options || {};

  options.ignoreKeys = true;
  // Possibly put this here: this.items = [];
  options.scrollable = true;
  Box.call(this, options);

  this.value = '';
  this.items = [];
  this.ritems = [];
  this.selected = 0;
  this._isList = true;

  if (!this.style.selected) {
    this.style.selected = {};
    this.style.selected.bg = options.selectedBg;
    this.style.selected.fg = options.selectedFg;
    this.style.selected.bold = options.selectedBold;
    this.style.selected.underline = options.selectedUnderline;
    this.style.selected.blink = options.selectedBlink;
    this.style.selected.inverse = options.selectedInverse;
    this.style.selected.invisible = options.selectedInvisible;
  }

  if (!this.style.item) {
    this.style.item = {};
    this.style.item.bg = options.itemBg;
    this.style.item.fg = options.itemFg;
    this.style.item.bold = options.itemBold;
    this.style.item.underline = options.itemUnderline;
    this.style.item.blink = options.itemBlink;
    this.style.item.inverse = options.itemInverse;
    this.style.item.invisible = options.itemInvisible;
  }

  // Legacy: for apps written before the addition of item attributes.
  ['bg', 'fg', 'bold', 'underline',
   'blink', 'inverse', 'invisible'].forEach(function(name) {
    if (self.style[name] != null && self.style.item[name] == null) {
      self.style.item[name] = self.style[name];
    }
  });

  if (this.options.itemHoverBg) {
    this.options.itemHoverEffects = { bg: this.options.itemHoverBg };
  }

  if (this.options.itemHoverEffects) {
    this.style.item.hover = this.options.itemHoverEffects;
  }

  if (this.options.itemFocusEffects) {
    this.style.item.focus = this.options.itemFocusEffects;
  }

  this.interactive = options.interactive !== false;

  this.mouse = options.mouse || false;

  if (options.items) {
    this.ritems = options.items;
    options.items.forEach(this.add.bind(this));
  }

  this.select(0);

  if (options.mouse) {
    this.screen._listenMouse(this);
    this.on('element wheeldown', function() {
      self.select(self.selected + 2);
      self.screen.render();
    });
    this.on('element wheelup', function() {
      self.select(self.selected - 2);
      self.screen.render();
    });
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.up();
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.down();
        self.screen.render();
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'l' && !key.shift)) {
        self.enterSelected();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.cancelSelected();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.move(-((self.height - self.iheight) / 2) | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.move((self.height - self.iheight) / 2 | 0);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'b' && key.ctrl) {
        self.move(-(self.height - self.iheight));
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'f' && key.ctrl) {
        self.move(self.height - self.iheight);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'h' && key.shift) {
        self.move(self.childBase - self.selected);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'm' && key.shift) {
        // TODO: Maybe use Math.min(this.items.length,
        // ... for calculating visible items elsewhere.
        var visible = Math.min(
          self.height - self.iheight,
          self.items.length) / 2 | 0;
        self.move(sel ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.listbar"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>listbar (options)](#apidoc.element.blessed.widget.listbar)
- description and source-code
```javascript
function Listbar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Listbar(options);
  }

  options = options || {};

  this.items = [];
  this.ritems = [];
  this.commands = [];

  this.leftBase = 0;
  this.leftOffset = 0;

  this.mouse = options.mouse || false;

  Box.call(this, options);

  if (!this.style.selected) {
    this.style.selected = {};
  }

  if (!this.style.item) {
    this.style.item = {};
  }

  if (options.commands || options.items) {
    this.setItems(options.commands || options.items);
  }

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'left'
          || (options.vi && key.name === 'h')
          || (key.shift && key.name === 'tab')) {
        self.moveLeft();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'right'
          || (options.vi && key.name === 'l')
          || key.name === 'tab') {
        self.moveRight();
        self.screen.render();
        // Stop propagation if we're in a form.
        if (key.name === 'tab') return false;
        return;
      }
      if (key.name === 'enter'
          || (options.vi && key.name === 'k' && !key.shift)) {
        self.emit('action', self.items[self.selected], self.selected);
        self.emit('select', self.items[self.selected], self.selected);
        var item = self.items[self.selected];
        if (item._.cmd.callback) {
          item._.cmd.callback();
        }
        self.screen.render();
        return;
      }
      if (key.name === 'escape' || (options.vi && key.name === 'q')) {
        self.emit('action');
        self.emit('cancel');
        return;
      }
    });
  }

  if (options.autoCommandKeys) {
    this.onScreenEvent('keypress', function(ch) {
      if (/^[0-9]$/.test(ch)) {
        var i = +ch - 1;
        if (!~i) i = 9;
        return self.selectTab(i);
      }
    });
  }

  this.on('focus', function() {
    self.select(self.selected);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.listtable"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>listtable (options)](#apidoc.element.blessed.widget.listtable)
- description and source-code
```javascript
function ListTable(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ListTable(options);
  }

  options = options || {};
  options.shrink = true;
  options.normalShrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  this.__align = options.align || 'center';
  delete options.align;

  options.style.selected = options.style.cell.selected;
  options.style.item = options.style.cell;

  List.call(this, options);

  this._header = new Box({
    parent: this,
    left: this.screen.autoPadding ? 0 : this.ileft,
    top: 0,
    width: 'shrink',
    height: 1,
    style: options.style.header,
    tags: options.parseTags || options.tags
  });

  this.on('scroll', function() {
    self._header.setFront();
    self._header.rtop = self.childBase;
    if (!self.screen.autoPadding) {
      self._header.rtop = self.childBase + (self.border ? 1 : 0);
    }
  });

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setData(self.rows);
  });

  this.on('resize', function() {
    var selected = self.selected;
    self.setData(self.rows);
    self.select(selected);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.loading"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>loading (options)](#apidoc.element.blessed.widget.loading)
- description and source-code
```javascript
function Loading(options) {
  if (!(this instanceof Node)) {
    return new Loading(options);
  }

  options = options || {};

  Box.call(this, options);

  this._.icon = new Text({
    parent: this,
    align: 'center',
    top: 2,
    left: 1,
    right: 1,
    height: 1,
    content: '|'
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.log"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>log (options)](#apidoc.element.blessed.widget.log)
- description and source-code
```javascript
function Log(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Log(options);
  }

  options = options || {};

  ScrollableText.call(this, options);

  this.scrollback = options.scrollback != null
    ? options.scrollback
    : Infinity;
  this.scrollOnInput = options.scrollOnInput;

  this.on('set content', function() {
    if (!self._userScrolled || self.scrollOnInput) {
      nextTick(function() {
        self.setScrollPerc(100);
        self._userScrolled = false;
        self.screen.render();
      });
    }
  });
}
```
- example usage
```shell
...
  left: '45%+1',
  ...
'''

To access the calculated offsets, relative to the parent:

''' js
console.log(box.left);
console.log(box.top);
'''

To access the calculated offsets, absolute (relative to the screen):

''' js
console.log(box.aleft);
...
```

#### <a name="apidoc.element.blessed.widget.message"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>message (options)](#apidoc.element.blessed.widget.message)
- description and source-code
```javascript
function Message(options) {
  if (!(this instanceof Node)) {
    return new Message(options);
  }

  options = options || {};
  options.tags = true;

  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.node"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>node (options)](#apidoc.element.blessed.widget.node)
- description and source-code
```javascript
function Node(options) {
  var self = this;
  var Screen = require('./screen');

  if (!(this instanceof Node)) {
    return new Node(options);
  }

  EventEmitter.call(this);

  options = options || {};
  this.options = options;

  this.screen = this.screen || options.screen;

  if (!this.screen) {
    if (this.type === 'screen') {
      this.screen = this;
    } else if (Screen.total === 1) {
      this.screen = Screen.global;
    } else if (options.parent) {
      this.screen = options.parent;
      while (this.screen && this.screen.type !== 'screen') {
        this.screen = this.screen.parent;
      }
    } else if (Screen.total) {
      // This _should_ work in most cases as long as the element is appended
      // synchronously after the screen's creation. Throw error if not.
      this.screen = Screen.instances[Screen.instances.length - 1];
      process.nextTick(function() {
        if (!self.parent) {
          throw new Error('Element (' + self.type + ')'
            + ' was not appended synchronously after the'
            + ' screen\'s creation. Please set a 'parent''
            + ' or 'screen' option in the element\'s constructor'
            + ' if you are going to use multiple screens and'
            + ' append the element later.');
        }
      });
    } else {
      throw new Error('No active screen.');
    }
  }

  this.parent = options.parent || null;
  this.children = [];
  this.$ = this._ = this.data = {};
  this.uid = Node.uid++;
  this.index = this.index != null ? this.index : -1;

  if (this.type !== 'screen') {
    this.detached = true;
  }

  if (this.parent) {
    this.parent.append(this);
  }

  (options.children || []).forEach(this.append.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.overlayimage"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>overlayimage (options)](#apidoc.element.blessed.widget.overlayimage)
- description and source-code
```javascript
function OverlayImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new OverlayImage(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.w3m) {
    OverlayImage.w3mdisplay = options.w3m;
  }

  if (OverlayImage.hasW3MDisplay == null) {
    if (fs.existsSync(OverlayImage.w3mdisplay)) {
      OverlayImage.hasW3MDisplay = true;
    } else if (options.search !== false) {
      var file = helpers.findFile('/usr', 'w3mimgdisplay')
              || helpers.findFile('/lib', 'w3mimgdisplay')
              || helpers.findFile('/bin', 'w3mimgdisplay');
      if (file) {
        OverlayImage.hasW3MDisplay = true;
        OverlayImage.w3mdisplay = file;
      } else {
        OverlayImage.hasW3MDisplay = false;
      }
    }
  }

  this.on('hide', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('show', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.on('detach', function() {
    self._lastFile = self.file;
    self.clearImage();
  });

  this.on('attach', function() {
    if (!self._lastFile) return;
    self.setImage(self._lastFile);
  });

  this.onScreenEvent('resize', function() {
    self._needsRatio = true;
  });

  // Get images to overlap properly. Maybe not worth it:
  // this.onScreenEvent('render', function() {
  //   self.screen.program.flush();
  //   if (!self._noImage) return;
  //   function display(el, next) {
  //     if (el.type === 'w3mimage' && el.file) {
  //       el.setImage(el.file, next);
  //     } else {
  //       next();
  //     }
  //   }
  //   function done(el) {
  //     el.children.forEach(recurse);
  //   }
  //   function recurse(el) {
  //     display(el, function() {
  //       var pending = el.children.length;
  //       el.children.forEach(function(el) {
  //         display(el, function() {
  //           if (!--pending) done(el);
  //         });
  //       });
  //     });
  //   }
  //   recurse(self.screen);
  // });

  this.onScreenEvent('render', function() {
    self.screen.program.flush();
    if (!self._noImage) {
      self.setImage(self.file);
    }
  });

  if (this.options.file || this.options.img) {
    this.setImage(this.options.file || this.options.img);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.png"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>png (options)](#apidoc.element.blessed.widget.png)
- description and source-code
```javascript
function ANSIImage(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ANSIImage(options);
  }

  options = options || {};
  options.shrink = true;

  Box.call(this, options);

  this.scale = this.options.scale || 1.0;
  this.options.animate = this.options.animate !== false;
  this._noFill = true;

  if (this.options.file) {
    this.setImage(this.options.file);
  }

  this.screen.on('prerender', function() {
    var lpos = self.lpos;
    if (!lpos) return;
    // prevent image from blending with itself if there are alpha channels
    self.screen.clearRegion(lpos.xi, lpos.xl, lpos.yi, lpos.yl);
  });

  this.on('destroy', function() {
    self.stop();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.progressbar"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>progressbar (options)](#apidoc.element.blessed.widget.progressbar)
- description and source-code
```javascript
function ProgressBar(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ProgressBar(options);
  }

  options = options || {};

  Input.call(this, options);

  this.filled = options.filled || 0;
  if (typeof this.filled === 'string') {
    this.filled = +this.filled.slice(0, -1);
  }
  this.value = this.filled;

  this.pch = options.pch || ' ';

  // XXX Workaround that predates the usage of 'el.ch'.
  if (options.ch) {
    this.pch = options.ch;
    this.ch = ' ';
  }
  if (options.bch) {
    this.ch = options.bch;
  }

  if (!this.style.bar) {
    this.style.bar = {};
    this.style.bar.fg = options.barFg;
    this.style.bar.bg = options.barBg;
  }

  this.orientation = options.orientation || 'horizontal';

  if (options.keys) {
    this.on('keypress', function(ch, key) {
      var back, forward;
      if (self.orientation === 'horizontal') {
        back = ['left', 'h'];
        forward = ['right', 'l'];
      } else if (self.orientation === 'vertical') {
        back = ['down', 'j'];
        forward = ['up', 'k'];
      }
      if (key.name === back[0] || (options.vi && key.name === back[1])) {
        self.progress(-5);
        self.screen.render();
        return;
      }
      if (key.name === forward[0] || (options.vi && key.name === forward[1])) {
        self.progress(5);
        self.screen.render();
        return;
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      var x, y, m, p;
      if (!self.lpos) return;
      if (self.orientation === 'horizontal') {
        x = data.x - self.lpos.xi;
        m = (self.lpos.xl - self.lpos.xi) - self.iwidth;
        p = x / m * 100 | 0;
      } else if (self.orientation === 'vertical') {
        y = data.y - self.lpos.yi;
        m = (self.lpos.yl - self.lpos.yi) - self.iheight;
        p = y / m * 100 | 0;
      }
      self.setProgress(p);
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.prompt"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>prompt (options)](#apidoc.element.blessed.widget.prompt)
- description and source-code
```javascript
function Prompt(options) {
  if (!(this instanceof Node)) {
    return new Prompt(options);
  }

  options = options || {};

  options.hidden = true;

  Box.call(this, options);

  this._.input = new Textbox({
    parent: this,
    top: 3,
    height: 1,
    left: 2,
    right: 2,
    bg: 'black'
  });

  this._.okay = new Button({
    parent: this,
    top: 5,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    parent: this,
    top: 5,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.question"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>question (options)](#apidoc.element.blessed.widget.question)
- description and source-code
```javascript
function Question(options) {
  if (!(this instanceof Node)) {
    return new Question(options);
  }

  options = options || {};
  options.hidden = true;

  Box.call(this, options);

  this._.okay = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    left: 2,
    width: 6,
    content: 'Okay',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });

  this._.cancel = new Button({
    screen: this.screen,
    parent: this,
    top: 2,
    height: 1,
    shrink: true,
    left: 10,
    width: 8,
    content: 'Cancel',
    align: 'center',
    bg: 'black',
    hoverBg: 'blue',
    autoFocus: false,
    mouse: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.radiobutton"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>radiobutton (options)](#apidoc.element.blessed.widget.radiobutton)
- description and source-code
```javascript
function RadioButton(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new RadioButton(options);
  }

  options = options || {};

  Checkbox.call(this, options);

  this.on('check', function() {
    var el = self;
    while (el = el.parent) {
      if (el.type === 'radio-set'
          || el.type === 'form') break;
    }
    el = el || self.parent;
    el.forDescendants(function(el) {
      if (el.type !== 'radio-button' || el === self) {
        return;
      }
      el.uncheck();
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.radioset"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>radioset (options)](#apidoc.element.blessed.widget.radioset)
- description and source-code
```javascript
function RadioSet(options) {
  if (!(this instanceof Node)) {
    return new RadioSet(options);
  }
  options = options || {};
  // Possibly inherit parent's style.
  // options.style = this.parent.style;
  Box.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.screen"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>screen (options)](#apidoc.element.blessed.widget.screen)
- description and source-code
```javascript
function Screen(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Screen(options);
  }

  Screen.bind(this);

  options = options || {};
  if (options.rsety && options.listen) {
    options = { program: options };
  }

  this.program = options.program;

  if (!this.program) {
    this.program = program({
      input: options.input,
      output: options.output,
      log: options.log,
      debug: options.debug,
      dump: options.dump,
      terminal: options.terminal || options.term,
      resizeTimeout: options.resizeTimeout,
      forceUnicode: options.forceUnicode,
      tput: true,
      buffer: true,
      zero: true
    });
  } else {
    this.program.setupTput();
    this.program.useBuffer = true;
    this.program.zero = true;
    this.program.options.resizeTimeout = options.resizeTimeout;
    if (options.forceUnicode != null) {
      this.program.tput.features.unicode = options.forceUnicode;
      this.program.tput.unicode = options.forceUnicode;
    }
  }

  this.tput = this.program.tput;

  Node.call(this, options);

  this.autoPadding = options.autoPadding !== false;
  this.tabc = Array((options.tabSize || 4) + 1).join(' ');
  this.dockBorders = options.dockBorders;

  this.ignoreLocked = options.ignoreLocked || [];

  this._unicode = this.tput.unicode || this.tput.numbers.U8 === 1;
  this.fullUnicode = this.options.fullUnicode && this._unicode;

  this.dattr = ((0 << 18) | (0x1ff << 9)) | 0x1ff;

  this.renders = 0;
  this.position = {
    left: this.left = this.aleft = this.rleft = 0,
    right: this.right = this.aright = this.rright = 0,
    top: this.top = this.atop = this.rtop = 0,
    bottom: this.bottom = this.abottom = this.rbottom = 0,
    get height() { return self.height; },
    get width() { return self.width; }
  };

  this.ileft = 0;
  this.itop = 0;
  this.iright = 0;
  this.ibottom = 0;
  this.iheight = 0;
  this.iwidth = 0;

  this.padding = {
    left: 0,
    top: 0,
    right: 0,
    bottom: 0
  };

  this.hover = null;
  this.history = [];
  this.clickable = [];
  this.keyable = [];
  this.grabKeys = false;
  this.lockKeys = false;
  this.focused;
  this._buf = '';

  this._ci = -1;

  if (options.title) {
    this.title = options.title;
  }

  options.cursor = options.cursor || {
    artificial: options.artificialCursor,
    shape: options.cursorShape,
    blink: options.cursorBlink,
    color: options.cursorColor
  };

  this.cursor = {
    artificial: options.cursor.artificial || false,
    shape: options.cursor.shape || 'block',
    blink: options.cursor.blink || false,
    color: options.cursor.color || null,
    _set: false,
    _state: 1,
    _hidden: true
  };

  this.program.on('resize', function() {
    self.alloc();
    self.render();
    (function emit(el) {
      el.emit('resize');
      el.children.forEach(emit);
    })(self);
  });

  this.program.on('focus', function() {
    self.emit('focus');
  });

  this.program.on('blur', function() {
    self.emit('blur');
  });

  this.program.on('warning', function(text) {
    self.emit('warning', text);
  });

  this.on('newListener', function fn(type) {
    if (type === 'keypress' || type.indexOf('key ') === 0 || type === 'mouse') {
      if (type === 'keypress' || type.indexOf('key ') === 0) self._listenKeys();
      if (type === 'mouse') self._listenMouse();
    }
    if (type === 'mouse'
      || type === 'click'
      || type === 'mouseover'
      || type === 'mouseout'
      || type === 'mousedown'
      || type === 'mouseup'
      || type === 'mousewheel'
      || type === 'wheeldown'
      || type === 'wheelup'
      || type === 'mousemove') {
      self._listenMouse();
    }
  });

  this.setMaxListeners(Infinity);

  this.enter();

  this.postEnter();
}
```
- example usage
```shell
...
'blessed.screen' option. This will enable CSR when scrolling text in elements
or when manipulating lines.

''' js
var blessed = require('blessed');

// Create a screen object.
var screen = blessed.screen({
  smartCSR: true
});

screen.title = 'my window title';

// Create a box perfectly centered horizontally and vertically.
var box = blessed.box({
...
```

#### <a name="apidoc.element.blessed.widget.scrollablebox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>scrollablebox (options)](#apidoc.element.blessed.widget.scrollablebox)
- description and source-code
```javascript
function ScrollableBox(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new ScrollableBox(options);
  }

  options = options || {};

  Box.call(this, options);

  if (options.scrollable === false) {
    return this;
  }

  this.scrollable = true;
  this.childOffset = 0;
  this.childBase = 0;
  this.baseLimit = options.baseLimit || Infinity;
  this.alwaysScroll = options.alwaysScroll;

  this.scrollbar = options.scrollbar;
  if (this.scrollbar) {
    this.scrollbar.ch = this.scrollbar.ch || ' ';
    this.style.scrollbar = this.style.scrollbar || this.scrollbar.style;
    if (!this.style.scrollbar) {
      this.style.scrollbar = {};
      this.style.scrollbar.fg = this.scrollbar.fg;
      this.style.scrollbar.bg = this.scrollbar.bg;
      this.style.scrollbar.bold = this.scrollbar.bold;
      this.style.scrollbar.underline = this.scrollbar.underline;
      this.style.scrollbar.inverse = this.scrollbar.inverse;
      this.style.scrollbar.invisible = this.scrollbar.invisible;
    }
    //this.scrollbar.style = this.style.scrollbar;
    if (this.track || this.scrollbar.track) {
      this.track = this.scrollbar.track || this.track;
      this.style.track = this.style.scrollbar.track || this.style.track;
      this.track.ch = this.track.ch || ' ';
      this.style.track = this.style.track || this.track.style;
      if (!this.style.track) {
        this.style.track = {};
        this.style.track.fg = this.track.fg;
        this.style.track.bg = this.track.bg;
        this.style.track.bold = this.track.bold;
        this.style.track.underline = this.track.underline;
        this.style.track.inverse = this.track.inverse;
        this.style.track.invisible = this.track.invisible;
      }
      this.track.style = this.style.track;
    }
    // Allow controlling of the scrollbar via the mouse:
    if (options.mouse) {
      this.on('mousedown', function(data) {
        if (self._scrollingBar) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          return;
        }
        var x = data.x - self.aleft;
        var y = data.y - self.atop;
        if (x === self.width - self.iright - 1) {
          // Do not allow dragging on the scrollbar:
          delete self.screen._dragging;
          delete self._drag;
          var perc = (y - self.itop) / (self.height - self.iheight);
          self.setScrollPerc(perc * 100 | 0);
          self.screen.render();
          var smd, smu;
          self._scrollingBar = true;
          self.onScreenEvent('mousedown', smd = function(data) {
            var y = data.y - self.atop;
            var perc = y / self.height;
            self.setScrollPerc(perc * 100 | 0);
            self.screen.render();
          });
          // If mouseup occurs out of the window, no mouseup event fires, and
          // scrollbar will drag again on mousedown until another mouseup
          // occurs.
          self.onScreenEvent('mouseup', smu = function() {
            self._scrollingBar = false;
            self.removeScreenEvent('mousedown', smd);
            self.removeScreenEvent('mouseup', smu);
          });
        }
      });
    }
  }

  if (options.mouse) {
    this.on('wheeldown', function() {
      self.scroll(self.height / 2 | 0 || 1);
      self.screen.render();
    });
    this.on('wheelup', function() {
      self.scroll(-(self.height / 2 | 0) || -1);
      self.screen.render();
    });
  }

  if (options.keys && !options.ignoreKeys) {
    this.on('keypress', function(ch, key) {
      if (key.name === 'up' || (options.vi && key.name === 'k')) {
        self.scroll(-1);
        self.screen.render();
        return;
      }
      if (key.name === 'down' || (options.vi && key.name === 'j')) {
        self.scroll(1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'u' && key.ctrl) {
        self.scroll(-(self.height / 2 | 0) || -1);
        self.screen.render();
        return;
      }
      if (options.vi && key.name === 'd' && key.ctrl) {
        self.scroll( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.scrollabletext"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>scrollabletext (options)](#apidoc.element.blessed.widget.scrollabletext)
- description and source-code
```javascript
function ScrollableText(options) {
  if (!(this instanceof Node)) {
    return new ScrollableText(options);
  }
  options = options || {};
  options.alwaysScroll = true;
  ScrollableBox.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.table"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>table (options)](#apidoc.element.blessed.widget.table)
- description and source-code
```javascript
function Table(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Table(options);
  }

  options = options || {};
  options.shrink = true;
  options.style = options.style || {};
  options.style.border = options.style.border || {};
  options.style.header = options.style.header || {};
  options.style.cell = options.style.cell || {};
  options.align = options.align || 'center';

  // Regular tables do not get custom height (this would
  // require extra padding). Maybe add in the future.
  delete options.height;

  Box.call(this, options);

  this.pad = options.pad != null
    ? options.pad
    : 2;

  this.setData(options.rows || options.data);

  this.on('attach', function() {
    self.setContent('');
    self.setData(self.rows);
  });

  this.on('resize', function() {
    self.setContent('');
    self.setData(self.rows);
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.terminal"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>terminal (options)](#apidoc.element.blessed.widget.terminal)
- description and source-code
```javascript
function Terminal(options) {
  if (!(this instanceof Node)) {
    return new Terminal(options);
  }

  options = options || {};
  options.scrollable = false;

  Box.call(this, options);

  // XXX Workaround for all motion
  if (this.screen.program.tmux && this.screen.program.tmuxVersion >= 2) {
    this.screen.program.enableMouse();
  }

  this.handler = options.handler;
  this.shell = options.shell || process.env.SHELL || 'sh';
  this.args = options.args || [];

  this.cursor = this.options.cursor;
  this.cursorBlink = this.options.cursorBlink;
  this.screenKeys = this.options.screenKeys;

  this.style = this.style || {};
  this.style.bg = this.style.bg || 'default';
  this.style.fg = this.style.fg || 'default';

  this.termName = options.terminal
    || options.term
    || process.env.TERM
    || 'xterm';

  this.bootstrap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.text"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>text (options)](#apidoc.element.blessed.widget.text)
- description and source-code
```javascript
function Text(options) {
  if (!(this instanceof Node)) {
    return new Text(options);
  }
  options = options || {};
  options.shrink = true;
  Element.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.textarea"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>textarea (options)](#apidoc.element.blessed.widget.textarea)
- description and source-code
```javascript
function Textarea(options) {
  var self = this;

  if (!(this instanceof Node)) {
    return new Textarea(options);
  }

  options = options || {};

  options.scrollable = options.scrollable !== false;

  Input.call(this, options);

  this.screen._listenKeys(this);

  this.value = options.value || '';

  this.__updateCursor = this._updateCursor.bind(this);
  this.on('resize', this.__updateCursor);
  this.on('move', this.__updateCursor);

  if (options.inputOnFocus) {
    this.on('focus', this.readInput.bind(this, null));
  }

  if (!options.inputOnFocus && options.keys) {
    this.on('keypress', function(ch, key) {
      if (self._reading) return;
      if (key.name === 'enter' || (options.vi && key.name === 'i')) {
        return self.readInput();
      }
      if (key.name === 'e') {
        return self.readEditor();
      }
    });
  }

  if (options.mouse) {
    this.on('click', function(data) {
      if (self._reading) return;
      if (data.button !== 'right') return;
      self.readEditor();
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.textbox"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>textbox (options)](#apidoc.element.blessed.widget.textbox)
- description and source-code
```javascript
function Textbox(options) {
  if (!(this instanceof Node)) {
    return new Textbox(options);
  }

  options = options || {};

  options.scrollable = false;

  Textarea.call(this, options);

  this.secret = options.secret;
  this.censor = options.censor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blessed.widget.video"></a>[function <span class="apidocSignatureSpan">blessed.widget.</span>video (options)](#apidoc.element.blessed.widget.video)
- description and source-code
```javascript
function Video(options) {
  var self = this
    , shell
    , args;

  if (!(this instanceof Node)) {
    return new Video(options);
  }

  options = options || {};

  Box.call(this, options);

  if (this.exists('mplayer')) {
    shell = 'mplayer';
    args = ['-vo', 'caca', '-quiet', options.file];
  } else if (this.exists('mpv')) {
    shell = 'mpv';
    args = ['--vo', 'caca', '--really-quiet', options.file];
  } else {
    this.parseTags = true;
    this.setContent('{red-fg}{bold}Error:{/bold}'
      + ' mplayer or mpv not installed.{/red-fg}');
    return this;
  }

  var opts = {
    parent: this,
    left: 0,
    top: 0,
    width: this.width - this.iwidth,
    height: this.height - this.iheight,
    shell: shell,
    args: args.slice()
  };

  this.now = Date.now() / 1000 | 0;
  this.start = opts.start || 0;
  if (this.start) {
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', this.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', this.start + '');
    }
  }

  var DISPLAY = process.env.DISPLAY;
  delete process.env.DISPLAY;
  this.tty = new Terminal(opts);
  process.env.DISPLAY = DISPLAY;

  this.on('click', function() {
    self.tty.pty.write('p');
  });

  // mplayer/mpv cannot resize itself in the terminal, so we have
  // to restart it at the correct start time.
  this.on('resize', function() {
    self.tty.destroy();

    var opts = {
      parent: self,
      left: 0,
      top: 0,
      width: self.width - self.iwidth,
      height: self.height - self.iheight,
      shell: shell,
      args: args.slice()
    };

    var watched = (Date.now() / 1000 | 0) - self.now;
    self.now = Date.now() / 1000 | 0;
    self.start += watched;
    if (shell === 'mplayer') {
      opts.args.unshift('-ss', self.start + '');
    } else if (shell === 'mpv') {
      opts.args.unshift('--start', self.start + '');
    }

    var DISPLAY = process.env.DISPLAY;
    delete process.env.DISPLAY;
    self.tty = new Terminal(opts);
    process.env.DISPLAY = DISPLAY;
    self.screen.render();
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
