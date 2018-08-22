# thinkphp

##介绍

> 1.什么是框架
```$xslt
    - 特征1 ： 一堆代码的集合
    - 特征2 : 一个半成品应用
    - 特征3 ：包含了一些优秀的设计模式
```
> 2.为什么要使用框架
- 不使用框架的弊端
```
   
- 每个人代码风格不一样，不便于开发和后期维护
-  一小处的修改，会牵扯出很多地方的修改
- 在后期满足客户需求（功能拓展）存在局限性
```

---------------
- 使用框架的好处
```
- 使用框架会帮助我们简单快速高效的开发项目
- 可以然能给我们有更多时间专注于业务逻辑的开发，不需要关注底层架构
- 便于处理多人协作开发中遇到的问题
```

> 3 常见的框架
 - Zend Framework
  > 是重量级框架，是php语言公司触屏的官方框架,比较臃肿，启动较慢
 - YII
  > 美国华人开发,外企应用比较多
 - Symfony
  > 重量级 国外框架
 - Laravel
  > 轻量级 国外框架
 - Codelgniter
  > 轻量级框架，简称CI框架，代码火焰。国外框架
 - ThinkPhp
  > 是一款国人开发的框架。国内普遍。适合入门级
 - ........
 
 > 4.MVC
 - 什么是MVC
   > MVC是一种设计模式。他是将用户的输入、输出、逻辑相分离，将整个项目分为三个部分:
   - 控制器（controller）
   - 模型（Model）
   - 视图（View）
   
 ======================

#   ThinkPHP 框架
   > - 1.国人自主开发，中文注释，中文文档，论坛
   > - 2.下载地址  http://www.thinkphp.cn/
   
###下载步骤
   > 第一步：
   - ![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/学习路线.png?raw=true)
   
   > 第二步：下载经典的3.2.3版本
   - ![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot002.png?raw=true)

   > 第二步：自行解压


=============================================
### 目录结构
#### 最外面的总体结构

- ![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot003.png?raw=true)

#### Aplication目录下面的文件

- ![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screen004.png?raw=true)




#### Thinkphp目录下面的文件


![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot001.png?raw=true)
![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/目录结构.png?raw=true)

#### Thinkphp --> config目录下面的文件

![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screen005.png?raw=true)


#####注意：
- convention.php 是*系统*级别的配置文件。另外还有*应用*级别和*分组*级别的配置文件

- 作用范围上：
  - > 系统>应用>分组
  
- 优先级上：
  - > 分组>应用>系统
  
#### thinkphp_3.2.3_full\ThinkPHP\Library\Think目录下
![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot006.png?raw=true)


## *部署*（重点）
> 1.配置站点目录
![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screen007.png?raw=true)

> 2.配置Apache虚拟主机的配置文件，创建一个虚拟主机
 - 文件目录 ：apache\conf\extra\httpd-vhosts.conf
 - 步骤：
   - 将之前的一段站点配置代码复制 进行修改
   ![目录结构](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screen008.png?raw=true)
> 2.重启Apache
> 3.修改host文件，将配置文件中申明的两个域名做一下绑定（解析）
  - #### host文件位置：C:\Windows\System32\drivers\etc\hosts
   ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot008.png?raw=true)
    -------------
  - #### 快速找到位置
     - 1.运行 drives
     - 2.运行 to hosts
    -------------
  - #### 添加域名绑定解析
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot009.png?raw=true)
  -------------
  - #### 看是否绑定成功 在cmd中使用ping命令
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot010.png?raw=true)
  -------------
  - #### 在浏览器中查看（下图表示成功）
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot011.png?raw=true)
   -------------
  - #### 将代码文件复制到站点目录中
      -（如：将thinkPHP里面的文件复制进去）*为了一步步学习thinkPHP特性，我们只复制两个文件，如下图*
      ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot012.png?raw=true)
  --------------
  - #### 再次通过浏览器查看
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot013.png?raw=true)
  
  -------------
  - ### 打开站点目录,会发现多了一个Application目录。（刚刚并没有复制进去）   
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot014.png?raw=true)
    
  -------------  
  - #### 生成的Application和thinkphp解压包解压出来的Application不一样
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot015.png?raw=true)
     
  -------------     
  - ### Common目录下
    ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot016.png?raw=true)
   
-------------    
## 细节问题
  - ### 自动生成
    - 在首次运行index.php入口文件时会自动生成相应的目录。目录的名字取决于在index.php定义的常量APP_PATH
     ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot019.png?raw=true)
     - 如果改变的话，就会生成相应的目录。
     -------------   
  - ### 目录安全文件  
    - 在自动生成的目录下都会有一个空白的html文件，文件名叫做index.html.这就叫做目录安全文件 
    - 作用：
         - 隐藏目录结构，保证安全
         ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot017.png?raw=true)
  
     -------------   
  - ### 默认访问
    - 默认分组/平台：Home
    - 默认控制器：index
    - 默认方法：index()
     可以在系统配置文件中找到：WWW\thinkPHP-learning\ThinkPHP\Conf      
      ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot020.png?raw=true)
      
       -------------   
## thinkPHP中控制器 
   - ### 控制器创建
      - 命名规则： *控制器名(英文首字母大写)+Controller+.class.php*
         - 例如： 
         ```
         UserController.class.php
         ```
         ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot021.png?raw=true)
               
          ```ruby
          <?php
          #声明命名控件
          namespace Home\Controller;
          #引入父类控制器
          use Think\Controller;
          #声明控制器（类）并且继承父类
          class UserController extends Controller {
              public function test(){    
              }
          } ?> 
         ```
         
      - 命名空间声明和使用必须和目录挂钩
      
      - 完善 测试```UserController.class.php```
        
         ```ruby
                  <?php
                  #声明命名控件
                  namespace Home\Controller;
                  #引入父类控制器
                  use Think\Controller;
                  #声明控制器（类）并且继承父类
                  class UserController extends Controller {
                      public function test(){
                         echo "测试UserController.class.php成功";
                      }
                  }
           ```
           ![](https://github.com/HunterXing/resourse/blob/master/images/screenshot/screenshot022.png?raw=true)
-------------              
      - 根据需要，后期可添加控制器     


-------------    
## *路由形式（重点）*
### *路由：*是指访问项中具体某个方法的URL地址
#### 四种路由形式
- 普通形式路由(get形式路由)      (get-2k;  post-8M)
    ```
    http://网址/入口文件?m=分组名&c=控制器名&a=方法名&参数名=参数值
    例如访问上述控制器的方法，并且传递一个参数 id = 1：
    http://www.xingheng.com/index.php?m=Home&c=User&a=test&id=1
    ```
    - 缺点：在URL暴露参数,不安全
- Pathinfo形式路由
    ```aidl

` ``        
- Rewrite形式路由
- 兼容形式路由

