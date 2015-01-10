## 作业要求

1. 请 Fork 该 Repository 到自己的 Github
2. Git Clone Fork 之后的 Repository 到本地，然后以此为基础开始做寒假作业，需要实现需求列表中的所有功能点，基于已有的功能点，大家可以随意创新
3. 所有 Java 代码需要 TDD 实现
4. 年后我们会一起展示大家的寒假作业


## 需求列表


+ 用户访问首页的时候能够看到所有商品的列表
	- 当用户处于未登录的状态时，首页右上角显示`亲，请登录`和`免费注册`
	- 当普通用户登陆之后首页右上角显示`用户名`和`购物车`
	- 当管理员登陆之后首页右上角显示`商品管理`
+ 用户能够点击`加入购物车`添加商品到购物车
	- 当用户处于未登录的状态时，跳转到`登陆`页面
	- 当用户处于登陆状态时，添加成功之后右上角`购物车后面的数字`会跟着改变
	- 如果商品的`库存数量不足`时，则弹框给出适当的提示
+ 在所有页面的左上角都有`商城的 Logo`，点击能够跳转到首页
+ 不同的用户，能够用自己的账号登录
	- 如果`用户名或者密码错误`时，则给出相应的错误提示
	- 普通用户登陆成功后，每个页面的右上角会显示该用户的`用户名`
	- 普通用户登陆成功后，每个页面的右上角会显示该用户的`购物车状态`
	- 管理员登陆成功后，每个页面的右上角`不显示购物车`，显示`管理商品`
+ 对于新用户，可以点击`免费注册`进入到用户注册页面
	- 用户在注册时，如果`用户名已经被占用`，会给出相应的错误提示
	- 用户在注册时，如果用户`两次输入的密码不一致`，会给出相应的错误提示
	- 用户在注册时，大家可以自己`丰富一下用户的信息`（比如：性别、年龄、联系方式……）
+ 管理员的账号，直接在`数据库中内置`即可
+ 在登陆状态下
	- 普通用户能够点击`购物车`进入到购物车页面
	- 不同的用户登录后，看到的是各自的购物车数据
	- 在购物车中商品价格的显示（原价、现价显示不同）
	- 管理员能够点击`管理商品`进入到商品管理页面
	- 用户可以 logout
+ 在购物车页面中
	- 用户能够`调整商品的数量`
	- 能够从购物车中`删除已有的商品`
	- 当选中购物车中的商品，点击`结算`后，则整个商城中对应商品的`库存数量会更新`，并且该`商品从用户购物车中消失`
+ 在商品管理页面中
	- 管理员可以点击`发布宝贝`，进入到添加商品的页面
	- 管理员可以输入内容`搜索`商城中所有商品
	- 管理员可以`删除`商城中已有的商品
	- 管理员可以`编辑`商城中已有的商品
	- 商城中以后的商品`以列表的形式展示`
	- 商品的列表中，可以`根据库存、总销量、发布时间排序`
+ 在发布宝贝的页面中
	- 管理员可以在表单中填入商品的相关属性（`标题、现价、原价、图片、商品描述、库存数量……`）
	- 管理员点击`立刻发布`时，添加的商品数据持久化到数据库中，页面跳转到商品管理页面

## Mockup

0. 所有可以演示的[Mockup](http://invis.io/6T1ZDALE2)，打不开的请翻墙后再试
0. 原始图片在项目的`mockup`目录下

## 注意事项

0. 用户注册后，密码在数据库中存储是否要加密？
0. 所有页面都有相同的 footer，怎么复用代码？
0. 整个商城完成后，如何部署使得外网可以访问？
0. 自己的项目在别人的电脑上怎么能够一个命令就跑起来？
0. 后台的 Java 代码，大家可以 TDD 了，那么 JavaScript 代码如何 TDD 呢？


