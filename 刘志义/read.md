## DOM节点之间相互的属性
childNodes 所有的子节点(元素节点,文本节点,元素节点)
children 所有的子元素节点 (ie8把文本节点当做元素节点)
previousSibling 相邻的哥哥节点
previousElementSibling 相邻的哥哥元素节点
nextSibling 相邻的弟弟节点
nextElementSibling 相邻的弟弟元素节点
firstChild 第一个节点
firstElementChild 第一个元素节点
lastChild 最后一个节点
lastElementChild 最后一个元素节点
parentNode 父亲节点
父子兄弟  child Nodes next previous  Sibiling Element parent 

## 动态操作DOM元素
 - 创建DOM元素 var oDiv = document.createElement("div");
 - 创建文本节点
 - 添加某个元素 父节点.appendChild(oDiv);
 - 插入某个元素之前 父节点.insertBefore(newEle,oldEle);
 - 
 
 
 
 
 ## 操作属性的方法
 - ele.getAttribute(属性名) 获取属性
 - ele.setAttribute(属性名,属性值) 设置属性 只能通过getAttribute获取
 >自定义属性：他俩是对应的,通过setAttribute
 
 
 
 
 ## 获取元素
 - id名 document.getElemntById
 - 标记名(tagName) context.getElementsByTagName
 - 类名 context.getElementsByClassTagName
 (ie6-8不兼容)
 - name属性 document.getElementByName('text');
 > 非表单元素,通过name属性获取(ie9及以下不支持)
 
 - document.querySelector(css选择器)
 - document.querySelectorAll(css选择器)
 
 
 
 
 ## 字符串常用方法
 通过索引查找
 - charAt  通过索引找到字符
 - charCodeAt 通过索引找到
 
 转化大小写
 - toLowerCase 转化为小写
 - toUppercase 转化为大写
 
 拆分
 - split("@") 按照指定字符拆分成每一个数组
 - indexOf
 - lastIndexOf
 - 
 
 
 截取
 - substr(n,m);从索引n(包)截取m个
 - substring(n,m);从索引n截取到索引m(包前不包后)
   n>m 则n,m自动交换
   不支持负数索引
   m是负数自动转换为0
 - slice(n,m);从索引n截取到索引m(包前不包后)
    +支持负数索引 负数索引 = 负数索引+字符串的长度
    +n>m 返回 空;
    
    
 >若只传一个参数,表示
 
 
 replace 替换
 
 
 ## Date
 时间
 
 
 ## 定时器
 - setTimeout(fn,interval);间隔一段时间,再去执行方法,intervar(间隔时间)单位毫秒
 setTimeout(function(){},1000)
 
 
 
 - setInterval(fn,interval);
 
 - clearTimeout()
 - clearTnterval()
 
 
 >每次把定时器清除掉后,要把变量timer设置成为null,后期可以通过time的值来判断定时器是否清除
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 