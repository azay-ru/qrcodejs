# QRCode.js
QRCode.js is javascript library for making QRCode. QRCode.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCode.js has no dependencies.

## Basic Usages
```
<div id="qrcode"></div>
<script>
   new QRCode(document.getElementById("qrcode"), "http://jindo.dev.naver.com/collie");
</script>
```

or with some options

```
<div id="qrcode"></div>
<script>
let qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "Some text to encode to QR",
	width: 128,
	height: 128,
	colorDark : "#000",
	colorLight : "#fff",
	correctLevel : QRCode.CorrectLevel.L
});
</script>
```

and you can use some methods

```
qrcode.clear(); // clear the code.
qrcode.makeCode("http://naver.com"); // make another code.
```

## Browser Compatibility
IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## To-do
Refactoring to modern JS style

## License
MIT License

## Thanks
Special tranks to original author [davidshimjs](https://github.com/davidshimjs)