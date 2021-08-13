# QRCodePay.js

QRCodePay.js は、暗号通貨の支払い用 QRCode を作成するための javascript ライブラリです。デフォルトでは JPYC on Polygon Network の QR コードを出力します。QRCodePay.js は、HTML5 Canvas と DOM の table タグでクロスブラウザをサポートしています。
QRCodePay.js には依存関係はありません。

QRCodePay.js is javascript library for making QRCode. QRCodePay draw QRCode for paying with JPYC on Polygon network. QRCodePay.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCodePay.js has no dependencies.

## 基本的な使い方 / Basic Usages

```
<div id="qrcode"></div>
<script type="text/javascript">
new QRCodePay(document.getElementById("qrcode"), "100","0xafd382aCC893127D6fbb197b87453070Fc14D43d");
</script>
```

or with some options

```
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCodePay(document.getElementById("qrcode"), {
	amount: "1000",
	dest: "0xafd382aCC893127D6fbb197b87453070Fc14D43d";
	width: 128,
	height: 128,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCodePay.CorrectLevel.H
});
</script>
```

and you can use some methods

```
qrcodePay.clear(); // clear the code.
qrcodePay.makeCodePay("200","0xafd382aCC893127D6fbb197b87453070Fc14D43d"); // make another code.
```

## Browser Compatibility

IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## License

MIT License

## Contact

twitter @nuko973663
