## CSS Selector

#### 基本选择器

1. `p {...}` 元素选择器: 选择页面所有的p元素
2. `.cls {...}` 类选择器: 选择页面所有 `class="cls"` 的元素
3. `#someID {...}` ID选择器: 选择页面所有 `id="someID"` 的元素
4. `* {...}` 通配选择器: 选择所有元素

#### 组合选择器

1. `p.cls {...}` 选择页面所有 `class="cls"` 的p元素
2. `p#someID {...}` 选择页面所有 `id="someID"` 的p元素(理论上页面元素的id应该是唯一的)
3. `.cls1.cls2 {...}` 选择页面所有 `class="cls1 cls2"` 的元素


#### 属性选择器

1. `p[attr] {...}` 选择所有拥有属性 attr 的p元素
2. `p[attr1][attr2] {...}` 选择同时拥有属性 attr1 和 attr2 的p元素
3. `p[attr="value"] {...}` 选择属性 attr 值为 value 的p元素
4. `p[class~="cls"] {...}` 选择属性 class 值中有单词 cls 的p元素(在这里相当于`.cls`选择器, 可以选择`class="cls"`, `class="cls cls2"`, 但是不会选择 `class="cls-abc"`, 注意跟`*=`的区别)
5. `p[attr*="value"] {...}` 选择属性 attr 值中包含 value 字符串的p元素
6. `p[attr^="value"] {...}` 选择属性 attr 的值以 value 开头的p元素
7. `p[attr$="value"] {...}` 选择属性 attr 的值以 value 结尾的p元素
8. `p[attr|="value"] {...}` 选择属性 attr 的值为 value 或以 value 开头的p元素


#### 后代选择器

1. `p em {...}`
2. `p > em {...}`
3. `p + em {...}`


#### 伪类

1. `a:link {...}`
2. `a:visited {...}`
3. `a:hover {...}`
4. `a:active {...}`
5. `input:focus {...}`
6. `p:first-child {...}`
7. `*:lang(fr)  {...}`


#### 伪元素
1. `a:first-letter {...}`
2. `div:first-line {...}`
3. `div:before {...}`
4. `div:after {...}`
