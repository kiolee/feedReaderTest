# 订阅器jasmine测试说明

1. 直接运行index.html，可以看到全部绿色通过

2. 修改allFeeds数据，把任意一个url或name设置成空值，刷新index.html，可以看到测试用例check allFeeds报错

3. 修改index.html的body class，使其不等于'menu-hidden'，刷新index.html，menu默认显示，可以看到测试用例The menu报错

4. 注释app.js的$('body').toggleClass('menu-hidden')，刷新index.html，可以看到测试用例icon click报错，点击不显示菜单

5. 修改allfeeds数据第一个对象的Url为无效的url，刷新index.html，可以看到测试用例Initial Entries报错，loadfeed得不到正常数据

6. 修改allfeeds数据第二个对象的url为无敌的url，刷新index.html，可以看到测试用例New Feed Selection报错，读取新源得不到数据
