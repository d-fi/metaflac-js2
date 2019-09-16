# metaflac-js2

A pure JavaScript implementation of the metaflac (the official FLAC tool written in C++)

> This is a tool that has just been completed, I hope to help you, and I hope we can optimize it together.

Use as module:

```
npm i metaflac-js2 --save
```

```
const Metaflac = require('metaflac-js2');
const flac = new Metaflac('/path/to/flac.flac or buffer');
flac.setTag('TITLE=My Music');
flac.save();
```

Use as cli:

Usage is basically consistent with official tools.

```
npm i metaflac-js2 -g
metaflac-js -h
```

Note: here is the official FLAC tools [doc](https://xiph.org/flac/documentation_tools_metaflac.html)

- This is a fork of [metaflac-js](https://github.com/ishowshao/metaflac-js) with minor improvements for detecting image dimensions and mime type.

#### Changelog:

- Removed `importPictureFrom`and `importPictureFromBuffer`
- Added `importPicture`


    importPicture takes either path or buffer
