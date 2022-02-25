# HIGHLIGHTJS-MIRC

highlight.js syntax definition for mIRC Scripting Language.

For more about highlight.js, see https://highlightjs.org/

For more about mIRC Scripting Language, see https://mirc.com/


## Usage

Simply include the `highlight.js` script package in your webpage or node app, load up this module and apply it to `hljs`.

If you're not using a build system and just want to embed this in your webpage:

```html
<script type="text/javascript" src="/path/to/highlight.pack.js"></script>
<script type="text/javascript" src="/path/to/highlightjs-mirc/mirc.js"></script>
<script type="text/javascript">
    hljs.registerLanguage('mirc', window.hljsDefineMIRC);
    hljs.highlightAll();
</script>
```

If you're using webpack / rollup / browserify / node:
   
```javascript
var hljs = require('highlightjs');
var hljsDefineMIRC = require('highlightjs-mirc');

hljsDefineMIRC(hljs);
hljs.highlightAll();
```

## Attributions

https://github.com/highlightjs/highlightjs-solidity
