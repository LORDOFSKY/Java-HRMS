# Java-HRMS
基于SSM框架的人力资源管理后台系统
## 用到的技术栈有：
* 框架：SSM
* 数据库：MySQL
* 前端框架：Bootstrap
* 项目管理：Maven
* 开发工具：Intellij IDEA
* 开发环境：Windows

### 数据库表
* tbl_emp表
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/emp.jpg)
* tbl_dept表
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/dept.jpg)

## 前端页面实现的最终效果如下
### 主页面
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E4%B8%BB%E9%A1%B5%E9%9D%A2.jpg)

### 员工操作页面
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E4%B8%BB%E9%A1%B52.jpg)

### 登录页面
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.jpg)

## 员工CRUD操作前后端实现
### 员工添加
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E5%91%98%E5%B7%A5%E6%B7%BB%E5%8A%A0.jpg)
#### 主要完成的功能有：
* 点击左侧栏的员工新增按钮，弹出员工新增的模态框页面；
* 对输入的姓名和邮箱格式进行验证，格式不正确，提示错误信息；
* 对输入的姓名进行姓名是否重复判断，重复则提示重复信息；
* 添加成功后跳转到添加记录所在的页面（即最后一页）；
* 添加失败则提示错误信息；

### 员工更改
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E5%91%98%E5%B7%A5%E6%9B%B4%E6%94%B9.jpg)
#### 更改成功
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E5%91%98%E5%B7%A5%E6%9B%B4%E6%94%B9%E6%88%90%E5%8A%9F.jpg)
#### 更改主要完成的功能有：
* 获取点击修改员工的id与name;
* 根据id或name查询出对应员工信息进行回显；
* 回显部门列表；
* 进行修改，对修改的邮箱格式进行判断；
* 点击更新按钮，发送AJAX请求到后台进行保存；
* 更改成功后跳转到当前更改页面；

###员工删除
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E5%91%98%E5%B7%A5%E5%88%A0%E9%99%A4.jpg)
#### 删除成功
![首页](https://github.com/LORDOFSKY/Java-HRMS/blob/master/WebRoot/picture/%E5%88%A0%E9%99%A4%E6%88%90%E5%8A%9F.jpg)
#### 删除主要完成的功能有：
* 弹出确认框：是否删除XX信息；
* 发送AJAX请求，执行删除操作；
* 删除成功后，跳转到当前页；
