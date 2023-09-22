<template>
  <div class="demo">
    <h2>学校名称: {{ name }}</h2>
    <h2>学校地址: {{ address }}</h2>
    <button @click="showName">点我提示学校名</button>
  </div>
</template>

<script>
// 组件交互相关的代码(数据、方法等等)
    //往后没必要再写Vue.extend,因为在该组件被注册时Vue会把该对象作为配置对象帮你调用Vue.extend,
    // export default Vue.extend({
    // name: "School",
    // data() {
    //     return {
    //     name: "尚硅谷",
    //     address: "北京昌平",
    //     };
    // },
    // methods: {
    //     showName() {
    //     alert(this.name);
    //     },
    // },
    // });
    export default {
    name: "School",
    data() {
        return {
        name: "尚硅谷",
        address: "北京昌平",
        };
    },
    methods: {
        showName() {
        alert(this.name);
        },
    },
    };
</script>

<style>
    /* 组件样式 */
    .demo {
    background-color: orange;
    }
</style>