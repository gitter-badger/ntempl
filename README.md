# ntempl

NTemplate is not a template framework, neither related with dual-binding.

## Getting Started
a basic usage is:
```html
<div id="#app">
  <div nt-id='name'>unnamed</div>
</div>
```

```js
var app = ntapp(nt_q("#app"));
app.el('name').innerText = "Artoria";
```
see, innerText is some old-fashioned thing you have already learned, natively dual-binding or non-dual-binding.

get, set and modify
```html
<div id="#app">
  <div nt-id='name'>unnamed</div>
  <input nt-id='age' nt-default='value'>
</div>
```

```js
var app = ntapp(nt_q("#app"));
app.set({name: "Hello", age: 99});
app.modify({name: x => x.toUpperCase()});
console.log(app.get({name: 1}).name); // HELLO
```

## Licence
Copyright 2017 Artoria Seiran https://github.com/Artoria    
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Other resources
[Playground](https://jsfiddle.net)   
[Repository](https://github.com/Artoria/ntempl)   
[Lens](http://hackage.haskell.org/package/lens)   


## Contribution & Feedback
[Pull Requests](https://github.com/Artoria/ntempl/pulls)   
[GMail](mailto:pochioly2008@gmail.com)   
[QQ](http://wpa.qq.com/msgrd?v=3&uin=297314126&site=qq&menu=yes)

## Donation
Donation is well accepted to encourage my spare time in this work.    
[Buy me a coffee @ WeChat](https://wx.tenpay.com/f2f?t=AQAAAJ%2FXTNaHzjztqnoG92LKMn0%3D)   
[But me a coffee @ AliPay](https://qr.alipay.com/stx00116sbiivlnndhimz82)   







