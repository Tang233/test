<template>
  <div>
    <p>{{msg}}</p>
    <p>这里是rawhtml里面的代码：{{rawhtml}}</p>
    <p>这里是加了rawhtml代码的标签效果：<span v-html="rawhtml"></span></p>
    <p v-if="seen">你现在看得到我吗？</p>
    <!--不是很懂v-bind-->
    <p v-bind:id="dynamicId">1234</p>


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'HelloWorld......',
      rawhtml: '<span style= "color:red">red</span>',
      seen: false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
