require-lcs IEcompatible
=======================

前端加载、编译literateCoffeeScript, [require-cs IEcompatible](cutsin/require-cs)的副本，仅修改扩展名为.coffee.md、.literate

## Example

page:
```html
<script>
var require = {
	paths: {
		lcs: 'https://github.com/cutsin/require-lcs/blob/master/require-lcs.js'
	}
}</script>
<script data-main="lcs!app/main" src="//static.abc.com/j/pub/require/2.1.14.js"></script>
```
app/main.coffee.md:
```coffeescript
require [
	'lcs!common/baseModel'
], ->
  console.log 'yeah~'
```
