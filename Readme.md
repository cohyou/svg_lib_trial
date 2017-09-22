# SVGを扱うライブラリを探してみました

## Raphaël.js https://dmitrybaranovskiy.github.io/raphael/

前述のSnap.svgの前身となったライブラリです。Snap.svgと比べると機能が少なく制約もありますが、IE 6+/Safari 3.0+/Firefox 3.0+とレガシーな環境もサポートされています。SVGがサポートされていない古いIEでは、VML（Vector Markup Language）というSVGの元となった言語で描画されるようフォールバックが用意されています。

## snap.svg http://snapsvg.io

Snap.svgはベクターグラフィックに特化し、アニメーション機能も備え、より高度にグラフィックスを操作できるライブラリです。Snap.svgは最新のブラウザ用に設計されていますのでマスキング、クリッピング、パターン、フルグラデーション、グループ機能など最新のSVGの機能をサポートしています。Snap.svgを導入することで、より自在にSVGを扱えるようになるのではないでしょうか。
Snap.svgはAdobe Systems社が提供しているオープンソースのライブラリです。SVG DOMの操作や、アニメーション・モーフィング、マスキング・クリッピングといった様々な高度な機能を簡潔に提供してくれます。SVGライブラリといえば「Raphaël.js」が代表格としてありましたが、Snap.svgはその後継として同じ作者（Dmitry Baranovskiy氏）によって開発されています。

## svg.js http://svgjs.com
### jQueryライクな操作

svg.jsはjQueryライクに操作できるSVGライブラリです。圧縮時は約53kb程度と軽量になっています。このサイズでベクターグラフィックスのすべての機能とイベントによる描画、アニメーションなどを備えています。jQueryに慣れていれば、SVGが簡単に扱えることでしょう。

SVG.jsはSVGの仕様を網羅しつつ、軽量かつ高速に動作することを謳っているライブラリです。公式サイトではSnap.svgの何倍も早く動作すると紹介されています。こちらもチェーンメソッドが採用されており、簡潔な記述が可能です。

## Two.js https://two.js.org
### SVGとCANVAS、WEBGLを利用したい時に

インタラクティブコンテンツ制作向け

Two.js is a two-dimensional drawing api geared towards modern web browsers. It is renderer agnostic enabling the same api to draw in multiple contexts: svg, canvas, and webgl.

Two.jsはSVGの他、CanvasやWebGLを利用できるライブラリです。ベクターグラフィックをWebで使用する際の描画方法を選択するのですが、記述方法はそれぞれの描画APIをラップしているので、同様のコードで記述できます。これにより、ブラウザによって使い分ける必要がないので、クロスブラウザ対策として非常に有効なライブラリとなるでしょう。

## BonsaiJS http://bonsaijs.org
### SVGでキーフレームアニメーション

BonsaiJSはSVGレンダラーを搭載した、キーフレームアニメーションをサポートするライブラリです。パスやグループ、フィルター処理、画像描画にも対応し、モーフィングも可能です。Flashのキーフレームアニメーションの代替えを考えている場合は、利用を検討しても良さそうです。

## GraphicsJS http://www.graphicsjs.org

A lightweight JavaScript graphics library with the intuitive API, based on SVG/VML technology.

## D3.js https://d3js.org
### データビジュアライゼーションに特化

D3.js is a JavaScript library for manipulating documents based on data. D3 helps you bring data to life using HTML, SVG, and CSS. D3’s emphasis on web standards gives you the full capabilities of modern browsers without tying yourself to a proprietary framework, combining powerful visualization components and a data-driven approach to DOM manipulation.

## vivus.js https://maxwellito.github.io/vivus/
### アニメーション処理に強そう

Vivus is a lightweight JavaScript class (with no dependencies) that allows you to animate SVGs, giving them the appearence of being drawn. There are a variety of different animations available, as well as the option to create a custom script to draw your SVG in whatever way you like.
