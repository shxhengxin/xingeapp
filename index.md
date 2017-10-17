### 核心代码分析(index.html)

#### 定义页面载入事件，基本语法
```
apiready = function(){} //相当于window.onload
```
#### $api对象
```
//根据元素的id获取元素
dom对象 = $api.byId('元素的id属性值');
以上代码就相当于document.getElementById('id');
```

#### 实现状态栏沉浸效果
```angular2html
$api.fixStatusBar(header);
```
#### $api.offset获取dom元素的位置
```angular2html
$api.offset(dom元素).w;//获取元素的宽度
$api.offset(dom元素).h;//获取元素的高度
```

#### 获取window窗体信息
```angular2html
api.winWidth  //获取窗体的宽度
api.winHeight //获取窗体的高度
```
#### 打开frame框架
```angular2html
api.openFrame({}) //打开新的框架
其中只有一个参数，要求是一个Json对象，参数如下：
name:框架名称
url : 打开的链接地址
bounces：是否可以拖动
rect:要求参数是一个json对象，主要设置框架的宽高以及横纵坐标
```

### 分析main.html代码