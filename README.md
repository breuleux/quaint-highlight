
quaint-highlight
================

Highlight code in Quaint markup using [highlight.js](https://highlightjs.org/).


## Install

    quaint --setup highlight

Follow the instructions.


## Sample configuration

This configuration entry must be added in the `plugins` field of
`quaint.json`:

```json
"highlight": {
  "theme": "agate",
  "defaultBlock": "javascript",
  "defaultInline": "javascript",
  "operatorBlock": "&",
  "operatorInline": "`"
}
```


Options
-------

**`operatorBlock`** (default: `"&"`) - define the operator for block
highlighting.

**`operatorInline`** (default: ``"`"``) - define the operator for
inline highlighting.

**`defaultLanguage`** (default: null) - define the language to use for
highlighting by default. This is useful if most of your code blocks
are in a specific language. By default, there is no highlighting.
Note that this will highlight both code blocks *and* inline code.

**`defaultBlock`** (default: null) - define the language to use for
highlighting by default for *code blocks*.

**`defaultInline`** (default: null) - define the language to use for
highlighting by default for *inline code*.

**`installPlugins`** (default: null) - a function that will be called
on the `highlight.js` instance. You can configure it, add languages,
and so on.

**`theme`** (default: `"default"`) - the theme to use. See
[here](https://highlightjs.org/static/demo/) for a demo of the themes.

You can also use a custom theme if you wish. If the theme name ends
with `.css`, `quaint-highlight` will assume it is a path to the css
file to use.

