# vue

## 异步组件

> 在大型应用中,我们可能需要

##  vue 的声明周期

* 单组件的生命周期

* 父子组件的生命周期

* 兄弟组件的生命周期

* 宏 mixin 的生命周期




1.  数据观测 1 props 2 data 3 computed
  
  事件配置: event/ watcher

2.  beforeCreate 实例初始化之后,数据和事件配置之前,可用于初始化非响应式变量

3. created 已将 data 和methods 挂载到 vue 实例上 可初始化 ajax 请求

4. beforeMount 编译模版完成,但未挂载,无法获取dom

5. mounted 组件挂载完成,能直接获取dom

