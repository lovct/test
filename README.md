# test
测试
# 关于vue的总结: #
## 总体的框架 ##
### 文件细节部分 ###
1. **build  ---webpack配置部分**
2. **config  ---vue项目配置**
3. **node_modules  ---依赖包**
4. **src  ---项目核心文件**
  1. index.html       主页
  一般只定义一个空的根节点，在main.js里面定义的实例挂载在根节点下，内容都通过vue组件来填充
  
  2.  App.vue        根组件
  一个vue页面通常有三部分组成：模板template、js、样式(style) 
 

 - **template**
 - 模板只能包含一个父节点，也就是说顶层的div只能有一个<router-view></router-view>是子路由器视图，后面的路由器页面显示在此处
 3. main.js         **入口文件**
 main.js主要是引入vue框架，根组件及路由设置，并且定义vue实例，下面的components:{App}，后期可以引入插件，当然首先得安装插件
 4. router   **路由配置**router文件夹下，有一个index.js，即为路由配置文件  我们在路径为/的路由，该路由对应的页面是hello组件，所以我们在浏览器url访问http://localhost:8080/#/时就渲染的hello组件，类似的，我们可以设置多个路由，‘/index’,'/list'之类的，当然首先得引入该组件，再为该组件设置路由。


