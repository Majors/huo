接口涉及跨域，所以你需要把url.js里面的地址重新设置一下

-基于 sessionStorage.getItem('uuid')是否有值， 来做用户是否已登录的判断，已登录会直接跳转已登录页面, 未登录会跳到登录页面， 业务逻辑在routes.js中, 暂时默认跳到个人页面

-在utils目录下添加web.js，抽象一个handleRes来统一处理返回数据的格式化， 在头部引用， 做法参考Person/index.js 的头部


-车长车型建议后台接口合并成一个接口，
－车长车型有bug， 其他这个类型的值为零， 出来的值有bug， 并不是[0, 8], 而是[8], 零被隐藏了，需要hack
