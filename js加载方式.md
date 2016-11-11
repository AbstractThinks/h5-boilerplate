## 1. 同步加载
<script src="http://yourdomain.com/script.js"></script>
同步模式，又称阻塞模式，会阻止浏览器的后续处理，停止了后续的解析，因此停止了后续的文件加载（如图像）、渲染、代码执行。

> html文件中的<script>标签中的代码或src引用的js文件中的代码是同步加载和执行的
> html文件中的<script>标签中的代码使用document.write()方式引入的js文件是异步执行的
> html文件中的<script>标签src属性所引用的js文件的代码内再使用document.write()方式引入的js文件是同步执行的
> 使用 Image 对象异步预加载 js 文件(不会被执行)

window.onload 事件会在 js 文件加载完毕才触发(即使是异步加载)
