   Vue是一套构建用户界面的 渐进式框架。与其他重量级框架不同的是，Vue 采用自底向上增量开发的设计。
   Vue 的核心库只关注视图层非常容易与其他库或者已有项目整合。
   另一方面，Vue有能力驱动采用单文件组件和Vue生态系统支持的库开发的复杂单页应用。  
   # 模块化  
     1.Vue 文件格式可以支持局部 CSS，只要在 <style> 标签上加上一个 scoped 属性。并且一个组件的局部 CSS 不会像单纯的选择器嵌套那样『渗透』到它包含的子组件当中去。  
     2.每一个 Vue 组件最终都被编译为纯粹的 JavaScript 模块，并且不需要任何浏览器 polyfill 即可支持到最低 IE9。如果你想，你也可以把它包在一个原生的自定义元素中。  
     3.Vue 文件的 <script> 默认支持 ES2015。  
     4.你可以在每一个语言块中使用任何你想用的预处理器。  
     5.当使用 Webpack + vue-loader 时，你可以借助 Webpack 的强大功能将静态资源作为模块依赖来处理。

   # 组件化  
     1.用 props 来定义如何接收外部数据。
     2.用自定义事件来向外传递消息。
     3.用 <slot> API 来将外部动态传入的内容（其他组件或是 HTML）和自身模板进行组合。
     
  # 响应式编程  
     var object = {
        message: 'Hello World!'
     }
     <div id="example">
       {{ message }}
     </div>
     new Vue({
      el: '#example',
      data: object
     })
     用vue将这样的对象与模板绑定，当修改 object.message 的值时，渲染的 HTML 会自动更新。vue可以轻松保证状态和视图的同步。  

  # 路由  
      vue非常小巧，压缩后min源码为72.9kb，gzip压缩后只有25.11kb，想比Angular为144kb，可以自驾搭配使用需要的库插件，类似路由插件(Vue-router)，Ajax插件(vue-resource)等。
      
  # 动画  
      Vue 的反应式系统使得它可以用来开发高效的数据驱动的逐帧动画。这一类逐帧动画在基于脏检查或是 Virtual DOM 的框架中，往往会导致性能问题，因为即使只是改了一个值，整个所处的子树（scope 或是 component）都需要重新计算。而 Vue 则是改了多少，计算多少，不会有无谓的浪费
