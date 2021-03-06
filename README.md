# Job

### 1.显示所有职位

作为游客和注册用户，可以看到已发布的所有工作信息

验收标准：

1. 导航栏显示ALL JOBS
2. 点击ALL JOBS显示如下内容：
   1. 工作标题
   2. 工作的国家，城市
   3. 工作的性质(Volunteer/Permanent/Freelance/Contract)
   4. 工作公司名称(参考网站上面有这个内容)






### 2.根据工作职位过滤职位

作为游客和注册登陆的用户，可以根据工作职位(例如development/designer/marketing/product manager等)来过滤已发布的工作

验收标准：

- 显示所有的工作职位过滤器
- 点击对应的工作职位过滤器就会进行过滤并显示对应的工作



这个过滤器和工作性质的过滤器现在还不能叠加

### 3.根据工作性质过滤职位

作为游客和注册登陆的用户，可以根据工作性质(Volunteer/Permanent/Freelance/Contract)来过滤已发布的所有工作

验收标准：

- 显示对应工作性质的过滤器
- 点击对应的工作性质过滤器就会进行过滤并显示对应的工作



已完成。

### 4.搜索职位(参考网站还没有这个)

作为游客和注册登陆的用户，可以根据工作的标题，公司名字和职位描述

验收标准：

- 显示搜索框
- 至少支持根据工作的标题、公司名称和职位描述进行模糊搜索


mohu.js  selectJobs.js

还未完成

### 5.查看工作详情

作为游客和注册登陆的用户，可以查看每一个已发布工作的详细信息。

验收标准：

- 单击某个工作之后
  1. 标题
  2. 公司名称
  3. 职位描述(富文本，markdown)
  4. 标签
  5. 如何应聘(富文本，markdown)





### 6.发布一个工作信息

作为已经注册登陆用户，可以发布一个招聘信息来招聘人才

验收标准：

- 导航栏显示POST A JOB
- 点击POST A JOB，进入创建工作招聘页面，显示发布一个工作招聘的详细信息，包含以下信息：（*为必填项）
  1. 工作标题*
  2. 公司名称*
  3. 职位描述*(富文本，markdown)
  4. 如何应聘*
  5. 截止时间*
  6. 工作性质*(下拉菜单)
  7. 工作种类*(下来菜单)
  8. 标签
  9. 工作城市*
  10. 工作国家*
  11. 创建工作按钮(点击后进入该工作详情页面)




已完成

创建工作之后进入工作详情界面，其实工作是未发布的，如果该工作是你创建的，那么会有编辑按钮，如果还未发布，还会有一个发布工作的按钮


### 7.用户查看自己创建的工作列表

作为注册登陆用户，可以浏览自己发布的所有工作

验收标准：

- 导航栏显示MY POSTS
- 点击MY POSTS，调准到招聘者发布的招聘工作列表页面，每一个招聘项包含：
  1. 工作职位
  2. 招聘工作的状态，hidden(未发表)／public(成功发表)


这个功能合并在用户详情页面里面




### 8.用户查看自己创建的工作详情

作为已经注册登陆的用户，可以查看并**修改**自己发布的工作

验收标准：

- 点击某一个工作项，进入工作详细页面，包含以下信息：
  1. 工作标题
  2. 公司名称
  3. 职位描述(富文本，markdown)
  4. 标签
  5. 如何应聘
  6. 编辑按钮
     - 点击编辑按钮，进入编辑页面，与创建工作招聘页面一样，只不过预填了原来的信息，用户可以修改
     - 点击更新工作的按钮之后，进入该工作的详细页面
     - 如果该工作还未发表，则会多出来一个发布工作的按钮，点击之后，跳转到招聘工作列表(MY POSTS)





### 9.修改账户信息

作为已经注册登陆的用户，可以修改自己的账户信息，同时可以注销账户

验收标准：

- 导航栏显示ACCOUNT
- 点击ACCOUNT，跳转到账户详细页面，包含：
  1. 用户信息 邮箱／密码／密码确认／现在的密码／公司名称／公司地址(国家，城市)／公司所属行业
  2. 更改按钮
  3. 点击更改按钮，如果现在的密码输入错误，那就修改不会成功，会有错误提示，如果全部信息填写正确，那么修改成功，返回首页。
  4. 注销账号的按钮，单击之后就会注销账户，回到未登录状态的首页。(这个注销账号的意思应该是删除账号 参考参考网站)




因为注册的时候没有要求填写公司信息，所以在个人页面还可以填写公司信息。

同时也可以修改密码。

注意注销账号的删除用户的意思.

### 10.登陆

作为已经注册的用户，可以直接登录该网站来进行使用

作为未注册的用户，(貌似必须先要点SIGN IN才能SIGN UP)

验收标准：

- 导航栏显示SIGN IN 
- 点击SIGN IN，跳转到登陆页，包含：
  1. 邮箱输入框，密码输入框
  2. 复选框 Remember me
  3. 登陆按钮 如果账号信息填写正确，那么登陆成功并且回到首页，否则提示错误信息
  4. 注册按钮 点击注册按钮之后，跳转到注册页面：
     1. 邮箱输入框
     2. 密码输入框
     3. 密码确认框
     4. 注册按钮 点击注册按钮后，验证注册信息是否正确(邮箱是否合法，密码和密码确认框是否一致)，如果注册信息填写正确，则跳转至首页，需要用户去邮箱里点击验证链接来登陆到该网站。如果注册信息有误，则给出错误信息提示
  5. 未收到验证邮件超链接 点击之后跳转到重新发送验证邮件页面，跟忘记密码页面包含项一样
  6. 忘记密码超链接 点击之后跳转到忘记密码页面，包含：
     1. 邮箱输入框
     2. 发送重置密码邮件的按钮 点击后发送邮件给该邮箱，并跳转到登陆界面
     3. 登陆超链接 点击后跳转到登陆界面
     4. 注册超链接 点击后跳转到注册界面

已完成，现在需要测试。所有的邮件验证都改成了发送验证码的形式

### 10.退出登录

作为已经注册登陆的用户，可以退出登录

验收标准：

* 导航栏显示LOGOUT
* 点击LOGOUT，退出登录



已完成，需测试。

### 11.收费设置(可选)

* 该公益组织希望设置一个收费功能，例如发布一个工作信息，需要向job poster收取一定的费用
* 收费方式可以是，一个招聘30天30元
* 后台可以设置招聘文章的天数以及费用
* 公益组织会有赞助商，有时会会给赞助商一些优惠码(赠送赞助商3个优惠码，一个优惠码可以用于免费发布一个工作信息一个月)
  * 后台可以生产优惠码
  * 缴费的时候，可以输入优惠码免除缴费

没做，应该是最后做吧。