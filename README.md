# tool-funjs

![](https://img.shields.io/badge/%20download-340-brightgreen.svg)
![](https://img.shields.io/npm/l/tool-funjs.svg)
![](https://img.shields.io/github/stars/CrazyMrYan/tool-funjs?style=social.svg)



# 快速上手
## 安装
```shell
npm install tool-funjs
```
### 全局注册（在main.js文件里注册）

```javascript
import tooljs from 'tool-funjs';
Vue.prototype.tooljs = tooljs;
```
### 局部注册（在你所使用的vue里注册）

```javascript
import tooljs from 'tool-funjs';
```
## 例子
```javascript
// isStatic：检测数据是不是除了symbol外的原始数据
this.tooljs.$isStatic('str')// true
```

#### 目录

```javascript
1、isStatic：检测数据是不是除了symbol外的原始数据

2、isPrimitive：检测数据是不是原始数据

3、isObject：判断数据是不是引用类型的数据 (例如： arrays, functions, objects, regexes, new Number(0),以及 new String(''))

4、isObjectLike：检查 value 是否是 类对象。 如果一个值是类对象，那么它不应该是 null，而且 typeof 后的结果是 "object"

5、getRawType：获取数据类型，返回结果为 Number、String、Object、Array等

6、isPlainObject：判断数据是不是Object类型的数据

7、isArray：判断数据是不是数组类型的数据

8、isRegExp：判断数据是不是正则对象

9、isDate：判断数据是不是时间对象

10、isNative：判断 value 是不是浏览器内置函数内置函数toString后的主体代码块为 [native code] ，而非内置函数则为相关代码，所以非内置函数可以进行拷贝(toString后掐头去尾再由Function转)

11、isFunction：检查 value 是不是函数

12、isLength：检查 value 是否为有效的类数组长度

13、isArrayLike：检查 value 是否是类数组,如果一个值被认为是类数组，那么它不是一个函数，并且value.length是个整数，大于等于 0，小于或等于 Number.MAX_SAFE_INTEGER。这里字符串也将被当作类数组

14、exitFullscreen：退出全屏

15、toFullScreen：开启全屏

16、downloadFile：base64数据导出文件，文件下载

17、GetUrlParam：获取Url参数，返回一个对象

18、getPropByPath：根据字符串路径获取对象属性 : 'obj[0].count'

19、dateStrForma：将指定字符串由一种时间格式转化为另一种

20、dateFormater：格式化时间

21、repeat：生成一个重复的字符串，有n个str组成，可修改为填充为数组等

```
