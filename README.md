zenjicombo
==========

#### A resource combiner. ####

Introduction
------------

This handler is used to combine multiple files onto one, to help reduce the amount of requests done in a page, it also compresses the whole request using gzip.

Usage
-----------

For stylesheets:
```html
<link rel="stylesheet" href="/zc.php?t=css&f=test,somethingelse"/>
```
Where:
`t=css`                  sets the loader to read .css files.
`f=test,somethingelse`    to combine `test.css` with `somethingelse.css`.

For javascripts:
```html
<script src="zc.php?t=js&f=test,blablabla"></script>
```
Where:
`t=js`                    sets the loader to read .js files
`f=test,blablabla`        to combine `test.js` with `blablabla.js`

Additionaly a `debug` parameter can be sent to force it to read uncompressed files e.g.
```html
/zc.php?t=css&f=test,somethingelse&debug
```

Check the attached `test.html` for a working example.
