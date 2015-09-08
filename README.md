# CSS.supports shim

## Installation
```
npm install css-supports
```

## Usage
### Without shimming (recommended)
```
import supports from 'css-supports';

supports('backdrop-filter', 'blur(20px)');
supports('(backdrop-filter: blur(20px)) or (-webkit-backdrop-filter: blur(20px))');
```

### With shimming
```
import supports from 'css-supports';
supports.shim();

CSS.supports('backdrop-filter', 'blur(20px)');
CSS.supports('(backdrop-filter: blur(20px)) or (-webkit-backdrop-filter: blur(20px))');
```

## Spec & more
https://developer.mozilla.org/en-US/docs/Web/API/CSS/supports
http://svn.webkit.org/repository/webkit/trunk/Source/WebCore/css/DOMWindowCSS.cpp
https://chromium.googlesource.com/chromium/blink/+/master/Source/core/css/DOMWindowCSS.cpp

## TODO
- Add tests

## License
Inspired by https://gist.github.com/codler/03a0995195aa2859465f  
MIT
