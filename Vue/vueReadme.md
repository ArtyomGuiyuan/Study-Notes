## Vue指令
### v-html 
* 更新元素的innerHTML 
* 注意:内容按普通 HTML 插入 不会作为 Vue 模板进行编译

### v-bind
* 缩写 :
* 可把某个属性修改为动态 直接调用数据对象的值

### v-on
* 缩写 @
* 给元素绑定事件

### v-for
* 基于源数据多次渲染元素或模板块。此指令之值，必须使用特定语法    alias in expression ，为当前遍历的元素提供别名
* 建议v-for 都应该有一个key属性

### v-show
* 根据表达式之真假值，切换元素的 display CSS 属性。

* 当条件变化时该指令触发过渡效果。

### v-if / v-else / v-else-if
* 条件渲染

### v-if 和 v-show
* v-if是“真正”的条件渲染，因为它会确保在切换过程中条件块内的事件监听器和子组件适当地被销毁和重建。同时它也是惰性的：如果在初始渲染时条件为假，则什么也不做——直到条件第一次变为真时，才会开始渲染条件块。
* v-show不管初始条件是什么，元素总是会被渲染，并且只是简单地基于 CSS 进行切换。
* 因此，如果需要非常频繁地切换，则使用 v-show 较好；如果在运行时条件很少改变，则使用 v-if 较好。





## 修饰符