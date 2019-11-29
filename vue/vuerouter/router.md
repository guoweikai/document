# 介绍

vuerouter 支持三种模式

## 功能简介
***
* 嵌套的路由/视图表
* 模块化的, 基于组件的路由配置
* 路由参数, 查询, 通配符
* 基于 Vue.js 过渡系统的视图过渡效果
* 细粒度的导航控制
* 带有自动激活的 CSS class 的连接
* HTML5 历史模式或 hash 模式, 在 IE9 中自动降级
* 自定义的滚动条行为

## 基础

***
### 起步
***

 **html**  

 ```
 <script src="https://unpkg.com/vue/dist/vue.js"></script>
<script src="https://unpkg.com/vue-router/dist/vue-router.js"></script>

<div id="app">
  <h1>Hello App!</h1>
  <p>
    <!-- 使用 router-link 组件来导航. -->
    <!-- 通过传入 `to` 属性指定链接. -->
    <!-- <router-link> 默认会被渲染成一个 `<a>` 标签 -->
    <router-link to="/foo">Go to Foo</router-link>
    <router-link to="/bar">Go to Bar</router-link>
  </p>
  <!-- 路由出口 -->
  <!-- 路由匹配到的组件将渲染在这里 -->
  <router-view></router-view>
</div>
 ``` 

 **js**

 ```
 // 0. 如果使用模块化机制编程，导入Vue和VueRouter，要调用 Vue.use(VueRouter)

// 1. 定义 (路由) 组件。
// 可以从其他文件 import 进来
const Foo = { template: '<div>foo</div>' }
const Bar = { template: '<div>bar</div>' }

// 2. 定义路由
// 每个路由应该映射一个组件。 其中"component" 可以是
// 通过 Vue.extend() 创建的组件构造器，
// 或者，只是一个组件配置对象。
// 我们晚点再讨论嵌套路由。
const routes = [
  { path: '/foo', component: Foo },
  { path: '/bar', component: Bar }
]

// 3. 创建 router 实例，然后传 `routes` 配置
// 你还可以传别的配置参数, 不过先这么简单着吧。
const router = new VueRouter({
  routes // (缩写) 相当于 routes: routes
})

// 4. 创建和挂载根实例。
// 记得要通过 router 配置参数注入路由，
// 从而让整个应用都有路由功能
const app = new Vue({
  router
}).$mount('#app')

// 现在，应用已经启动了
 ```

### 动态路由
***

 >当使用路由参数时, 例如,我们有一个 user 组件, 对于所有 ID 各不相同的用户,都要使用这个组件来渲染. 那么,我们可以在 vue-router 的路由路径中使用"动态路径参数",来达到这个效果

*  **响应路由参数的变化**

>提醒一下，当使用路由参数时，例如从 /user/foo 导航到 /user/bar，原来的组件实例会被复用。因为两个路由都渲染同个组件，比起销毁再创建，复用则显得更加高效。不过，这也意味着组件的生命周期钩子不会再被调用

*  **捕获所有路由或 404 Not found 路由**

* **高级匹配模式**

* **匹配优先级**










###  嵌套路由

### 编程式的导航

###  命名路由

### 命名视图



### 重定向和别名

###  路由组件参数

### HTML5 history 模式

## 进阶

### 导航守卫

* **全局前置守卫**

> 可以试用贴 router.beforeEach 注册一个全局前置守卫

 ` ` `


