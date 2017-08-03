## `Color` Class

Extends [`ValueType`](ValueType.md)


Module: [cc](../modules/cc.md)
Parent Module: [cc](../modules/cc.md)




cc.Color 用于表示颜色。

它包含 RGBA 四个以浮点数保存的颜色分量，每个的值都在 0 到 255 之间。

您也可以通过使用 <a href="../modules/cc.html#method_color" class="crosslink">cc.color</a> 的便捷方法来创建一个新的 Color。

### Index

##### Properties

  - [`WHITE`](#white) `Color` 纯白色，RGBA 是 [255, 255, 255, 255]。
  - [`BLACK`](#black) `Color` 纯黑色，RGBA 是 [0, 0, 0, 255]。
  - [`TRANSPARENT`](#transparent) `Color` 透明，RGBA 是 [0, 0, 0, 0]。
  - [`GRAY`](#gray) `Color` 灰色，RGBA 是 [127.5, 127.5, 127.5]。
  - [`RED`](#red) `Color` 纯红色，RGBA 是 [255, 0, 0]。
  - [`GREEN`](#green) `Color` 纯绿色，RGBA 是 [0, 255, 0]。
  - [`BLUE`](#blue) `Color` 纯蓝色，RGBA 是 [0, 0, 255]。
  - [`YELLOW`](#yellow) `Color` 黄色，RGBA 是 [255, 235, 4]。
  - [`ORANGE`](#orange) `Color` 橙色，RGBA 是 [255, 127, 0]。
  - [`CYAN`](#cyan) `Color` 青色，RGBA 是 [0, 255, 255]。
  - [`MAGENTA`](#magenta) `Color` 洋红色（品红色），RGBA 是 [255, 0, 255]。



##### Methods

  - [`constructor`](#constructor) 
  - [`clone`](#clone) 克隆当前颜色。
  - [`equals`](#equals) 判断两个颜色是否相等。
  - [`lerp`](#lerp) 线性插值
  - [`toString`](#tostring) 转换为方便阅读的字符串。
  - [`getR`](#getr) 获取当前颜色的红色值。
  - [`setR`](#setr) 设置当前的红色值，并返回当前对象。
  - [`getG`](#getg) 获取当前颜色的绿色值。
  - [`setG`](#setg) 设置当前的绿色值，并返回当前对象。
  - [`getB`](#getb) 获取当前颜色的蓝色值。
  - [`setB`](#setb) 设置当前的蓝色值，并返回当前对象。
  - [`getA`](#geta) 获取当前颜色的透明度值。
  - [`setA`](#seta) 设置当前的透明度，并返回当前对象。
  - [`toCSS`](#tocss) 转换为 CSS 格式。
  - [`clamp`](#clamp) 限制颜色数值，在 0 到 255 之间。
  - [`fromHEX`](#fromhex) 读取 16 进制颜色。
  - [`toHEX`](#tohex) 转换为 16 进制。
  - [`toRGBValue`](#torgbvalue) 转换为 24bit 的 RGB 值。
  - [`fromHSV`](#fromhsv) 读取 HSV（色彩模型）格式。
  - [`toHSV`](#tohsv) 转换为 HSV（色彩模型）格式。
  - [`rgb2hsv`](#rgb2hsv) RGB 转换为 HSV。
  - [`hsv2rgb`](#hsv2rgb) HSV 转换为 RGB。



### Details


#### Properties


##### WHITE

> 纯白色，RGBA 是 [255, 255, 255, 255]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:77](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L77) |



##### BLACK

> 纯黑色，RGBA 是 [0, 0, 0, 255]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:85](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L85) |



##### TRANSPARENT

> 透明，RGBA 是 [0, 0, 0, 0]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:93](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L93) |



##### GRAY

> 灰色，RGBA 是 [127.5, 127.5, 127.5]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:101](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L101) |



##### RED

> 纯红色，RGBA 是 [255, 0, 0]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:109](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L109) |



##### GREEN

> 纯绿色，RGBA 是 [0, 255, 0]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:117](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L117) |



##### BLUE

> 纯蓝色，RGBA 是 [0, 0, 255]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:125](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L125) |



##### YELLOW

> 黄色，RGBA 是 [255, 235, 4]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:133](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L133) |



##### ORANGE

> 橙色，RGBA 是 [255, 127, 0]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:141](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L141) |



##### CYAN

> 青色，RGBA 是 [0, 255, 255]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:149](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L149) |



##### MAGENTA

> 洋红色（品红色），RGBA 是 [255, 0, 255]。

| meta | description |
|------|-------------|
| Type | <a href="../classes/Color.html" class="crosslink">Color</a> |
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:157](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L157) |






<!-- Method Block -->
#### Methods


##### constructor



| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:52](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L52) |

###### Parameters
- r <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> red component of the color, default value is 0.
- g <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> green component of the color, defualt value is 0.
- b <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> blue component of the color, default value is 0.
- a <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> alpha component of the color, default value is 255.


##### clone

克隆当前颜色。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:176](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L176) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 


##### Example

```js
var color = new cc.Color();
var newColor = color.clone();// Color {r: 0, g: 0, b: 0, a: 255}
```

##### equals

判断两个颜色是否相等。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:191](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L191) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Boolean" class="crosslink external" target="_blank">Boolean</a> 

###### Parameters
- other <a href="../classes/Color.html" class="crosslink">Color</a> 

##### Example

```js
var color1 = cc.Color.WHITE;
var color2 = new cc.Color(255, 255, 255);
cc.log(color1.equals(color2)); // true;
color2 = cc.Color.RED;
cc.log(color2.equals(color1)); // false;
```

##### lerp

线性插值

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:208](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L208) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- to <a href="../classes/Color.html" class="crosslink">Color</a> 
- ratio <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">number</a> the interpolation coefficient.
- out <a href="../classes/Color.html" class="crosslink">Color</a> optional, the receiving vector.

##### Example

```Not found for the example path: utils/api/engine/docs/cocos2d/core/value-types/CCColor/lerp.js

##### toString

转换为方便阅读的字符串。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:231](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L231) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 


##### Example

```js
var color = cc.Color.WHITE;
color.toString(); // "rgba(255, 255, 255, 255)"
```

##### getR

获取当前颜色的红色值。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:248](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L248) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setR

设置当前的红色值，并返回当前对象。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:257](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L257) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- red <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> the new Red component.

##### Example

```js
var color = new cc.Color();
color.setR(255); // Color {r: 255, g: 0, b: 0, a: 255}
```

##### getG

获取当前颜色的绿色值。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:271](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L271) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setG

设置当前的绿色值，并返回当前对象。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:280](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L280) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- green <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> the new Green component.

##### Example

```js
var color = new cc.Color();
color.setG(255); // Color {r: 0, g: 255, b: 0, a: 255}
```

##### getB

获取当前颜色的蓝色值。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:294](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L294) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setB

设置当前的蓝色值，并返回当前对象。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:303](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L303) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- blue <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> the new Blue component.

##### Example

```js
var color = new cc.Color();
color.setB(255); // Color {r: 0, g: 0, b: 255, a: 255}
```

##### getA

获取当前颜色的透明度值。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:317](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L317) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 



##### setA

设置当前的透明度，并返回当前对象。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:326](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L326) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- alpha <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> the new Alpha component.

##### Example

```js
var color = new cc.Color();
color.setA(0); // Color {r: 0, g: 0, b: 0, a: 0}
```

##### toCSS

转换为 CSS 格式。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:346](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L346) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- opt <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> "rgba", "rgb", "#rgb" or "#rrggbb".

##### Example

```Not found for the example path: utils/api/engine/docs/cocos2d/core/value-types/CCColor/toCSS.js

##### clamp

限制颜色数值，在 0 到 255 之间。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:375](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L375) |


##### Example

```js
var color = new cc.Color(1000, 0, 0, 255);
color.clamp();
cc.log(color); // (255, 0, 0, 255)
```

##### fromHEX

读取 16 进制颜色。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:389](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L389) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- hexString <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

##### Example

```js
var color = cc.Color.BLACK;
color.fromHEX("#FFFF33"); // Color {r: 255, g: 255, b: 51, a: 255};
```

##### toHEX

转换为 16 进制。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:409](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L409) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- fmt <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> "#rgb" or "#rrggbb".

##### Example

```js
var color = cc.Color.BLACK;
color.toHEX("#rgb");     // "000";
color.toHEX("#rrggbb");  // "000000";
```

##### toRGBValue

转换为 24bit 的 RGB 值。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:444](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L444) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 


##### Example

```js
var color = cc.Color.YELLOW;
color.toRGBValue(); // 16771844;
```

##### fromHSV

读取 HSV（色彩模型）格式。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:457](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L457) |
| Return 		 | <a href="../classes/Color.html" class="crosslink">Color</a> 

###### Parameters
- h <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- s <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- v <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 

##### Example

```js
var color = cc.Color.YELLOW;
color.fromHSV(0, 0, 1); // Color {r: 255, g: 255, b: 255, a: 255};
```

##### toHSV

转换为 HSV（色彩模型）格式。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:476](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L476) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 


##### Example

```js
var color = cc.Color.YELLOW;
color.toHSV(); // Object {h: 0.1533864541832669, s: 0.9843137254901961, v: 1};
```

##### rgb2hsv

RGB 转换为 HSV。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:504](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L504) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 

###### Parameters
- r <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> red, must be [0, 255].
- g <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> red, must be [0, 255].
- b <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> red, must be [0, 255].

##### Example

```js
cc.Color.rgb2hsv(255, 255, 255); // Object {h: 0, s: 0, v: 1};
```

##### hsv2rgb

HSV 转换为 RGB。

| meta | description |
|------|-------------|
| Defined | [https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js:538](https:/github.com/cocos-creator/engine/blob/master/cocos2d/core/value-types/CCColor.js#L538) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 

###### Parameters
- h <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- s <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 
- v <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Number" class="crosslink external" target="_blank">Number</a> 

##### Example

```js
cc.Color.hsv2rgb(0, 0, 1); // Object {r: 255, g: 255, b: 255};
```

