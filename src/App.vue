<template>
  <div @androidback="back">
    <!-- 路由匹配到的组件将渲染在这里 -->
    <router-view style="flex:1"></router-view>
  </div>
</template>

<script>
  /*ES6语法 export与export default均可用于导出常量、函数、文件、模块等，
  你可以在其它文件或模块中通过import+(常量 | 函数 | 文件 | 模块)名的方式，将其导入，以便能够对其进行使用，
  但在一个文件或模块中，export、import可以有多个，export default仅有一个。 */
  export default {
    methods: {
      back: function () {
        this.$router.back()
      }
    }
  }
</script>
