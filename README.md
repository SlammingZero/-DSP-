##极赛DSP

这是本人在公司做的一个后台管理系统项目

业务逻辑：因为在国内人们比较难访问到谷歌，所以公司跟谷歌合作，借用Google的ads广告系统技术，合作研发了一款适合在国内使用的投放广告后台系统，投放广告通过添加相应关键字，提高SEO抓取，提高搜查点击率。

 

**技术栈 ：Vue-element-admin + Vue-cli +Vuex + Axios + Vue-router + Echarts +babel+Git**

 

###项目目录 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/one.png) 

###项目视图Views 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/two.png) 



###项目API（根据接口文档按分类功能封装成一个个方法，使用时注册调用即刻） 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/three.png) 

###项目公告组件components 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/one1.png)  



###项目路由Router

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/two1.png) 

###Modules

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/three1.png) 

###项目公共工具Utils（由于使用的是Vue-element-admin，所以附带了一些小工具）

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/one2.png) 

 

本人负责的是二期开发，所以登陆页，视图样式很多是已经完成了，主要负责：

① 广告系列的添加编辑投放。

② 改变广告状态（启用、暂停、移除）。

③ 广告组根据广告系列的添加投放。

④ 为广告添加关键字词。

⑤ 广告附加信息的渲染功能与添加广告内容页面编辑（文字广告、图片广告、自适应广告、大型展示广告等等）。

 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/two2.png) 

 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/three2.png) 

 

这是项目的主页面，插用chart，利用路由复用，系列与关键字，广告等视图复用，点击哪个功能router路由就会跳转到某个页面。

 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/tow3.png) 

 

这是添加广告系列，分五步，第一步判断类型，然后根据类型传值name，不同类型会有不同的组件使用

 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/onee.png) 

  

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/hh.png) 

 

当填写完毕后，后端会根据前端的编辑功能提交的数据判断是否是规定的内容，如果不是即会返回相应的提示错误，用户再根据错误纠正错误填写，当输入的值符合格式，即可通过审核，进入下一步。 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/eee1.png) 

 

获取selection的值，显示在右方已选择项，类似购物车的增删选中的商品功能 

![img](https://raw.githubusercontent.com/mufengsm/aiqianduan9/master/imges/img/yyy1.png) 

 

最后一步填写广告信息，右方为显示板，获取填写的内容，最后添加保存即可实现完整的添加广告系列流程，后端会在数据库增加相应的一则数据储存。

 

这就是一套完整的广告添加编辑功能，其他添加功能万变不离其宗，无非是根据需要的id不同来实现添加，又或者是在添加编辑页面上需要的功能不一样，例如添加关键字等等，编辑一下相应的组件视图传值数据即可。