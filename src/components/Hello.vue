<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script lang="ts">
import Vue, {ComponentOptions} from 'vue'
export default {
  name: 'hello',
  data() {
    return {
      msg: '家'
    }
  }
} as ComponentOptions<Vue>
</script>

<!-- scoped添加私有样式  lang添加babel编译  rel添加IDE识别 -->
<style scoped lang="scss" rel="stylesheet/scss">
.hello{
  background-color: #ff1;
  height: unit(33rem);
  h1, h2 {
    color: $mainC;
    background: no-repeat;
    @include bg-image('./img');
  }
}
</style>
