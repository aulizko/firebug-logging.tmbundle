Overview
========
Firebug logging bundle for [textmate](http://macromates.org) editor. As a JavaScript developer, I realize that it can be rather annoying to type console.log in the project debugging phase, so that I create this bundle for myself. Hope you find it usefull too.

This bundle introduce following snippets:

Primitive logging:
------------------
type `log[tab]`
and you should receive `console.log('%CURSOR_POSITION%');`

Parametric logging:
-------------------
type `logp` 
and you should receive same snippet as above with ability to define which variable to dump into log:
`console.log('Object: %o', Object)`, where you can replace Object for whatever you want

Info-level logging
------------------
Same as primitive logging, but instead 'log' command it shell produce `console.info('%CURSOR_POSITION%');` so that firebug should add nifty icon for that log message (may be usefull with firebug output filters)

Warn-level logging
------------------
Same as above, but you should receive no 'info' command but 'warn'. 

Installation:
=============
`cd /Library/Application\ Support/TextMate/Bundles/`

`git clone git://github.com/aulizko/firebug-logging.tmbundle.git`
