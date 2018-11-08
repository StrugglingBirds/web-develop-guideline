# 前端开发手册（完善中）
## 一、编程规约
### （一）命名风格
1. 【强制】代码命名严禁使用拼音或英文拼音混合方式，更不允许直接使用中文命名，惯例词除外。 
2. 【强制】类名使用 UpperCamelCase 风格，遵守驼峰形式。
3. 【强制】方法名、参数名、成员变量、局部变量使用 lowerCamelCase 风格，遵守驼峰形式。
4. 【强制】常量命名统一使用全部大写，原本驼峰处（单词间隔处）使用下划线隔开，力求语义表达完整。
5. 【强制】React 组件文件、对应 less、sass 文件以及外层的文件夹，统一使用 UpperCamelCase 风格，遵守驼峰形式。
6. 【强制】如果当前组件是页面组件，最外层容器（div）中的 class 写成 ``组件名-container`` 格式，如当前页面组件为 ``Home``，则最外层样式为 ``home-container``。
7. 【强制】如果当前组件是非页面组件，最外层容器（div）中的 class 写成 ``组件名-component`` 格式，如当前页面组件为 ``NavigationBar``，则最外层样式为 ``navigation-bar-component``。
8. 【强制】杜绝不规范、不通用的缩写。
9. 【强制】非类文件的直接文件夹名称，统一全部使用小写，避免 git 在同步时不同机器上目录大小写不准确区分的问题。
10. 【推荐】如果使用了设计模式，在文件名以及类名上体现出设计模式，如 RequestProxy，HumanFactory。
11. 【推荐】如果使用专门文件定义了枚举对象或者常量对象，在文件命名或者 export 出来的对象命名上予以体现，如 KeyBindEnum，ErrorCodeConstants。


### （二）常量定义
1. 【强制】如果当前环境支持 let、const，则不允许使用 var 定义变量。
2. 【强制】禁止使用魔法值，统一使用有语义的常量来代替。
3. 【强制】如果有常量类型的枚举，事先定义枚举对象，并在对象中罗列出所有的枚举常量细类。
4. 【推荐】不要在一个常量文件里面维护所有的常量，不同类别常量进行区分，如 ErrorCodeConstants，StatusCodeConstants。
5. 

### （三）控制语句
1. 【强制】

### （四）注释规约
1. 【强制】文件、类、方法的注释使用 JSDoc 注释规范，如 `` /** 注释内容 */ ``，如果是方法，补充参数和返回值说明。
2. 【强制】方法内部注释，在被注释语句上方单起一行，并使用 `` // `` 注释。方法内部需要多行注释时，使用 `` /* */ `` 注释，并注意对齐。
3. 【强制】所有组件必须有功能说明，属于全局基础组件还是特定页面组件，二次更改风险性评估，有复杂逻辑处需重点说明。
3. 【推荐】使用 `` // `` 单行注释时，在双斜杠后方预留一个空格，再书写注释语句。如 
	``` javascript
	function hello(name) {
	  // 打印 hello
	  console.log("hello, " + name)
	}
	```
4. 

### （五）代码风格
1. 【强制】类文件使用 ES6 风格来定义 class，并添加内部方法，禁止使用 function. prototype 来添加原型方法。
2. 【强制】React 组件中如果有使用 props，则在组件定义中添加 Component.propTypes，并对字段类型、是否必输、功能等相关属性进行说明。

### （六）其他

## 二、异常处理
## 三、数据打点
## 四、工程架构

