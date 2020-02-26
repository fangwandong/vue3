<template>
  <div>
    <!-- 绑定数据，在一秒内改变数据 -->
    <button class="demoBtn">{{msg}}</button>

    <!--绑定默认属性内容 -->
    <button  class="demoBtn">{{defaultMsg}}</button>
    
    <!-- 按钮点击事件，通过指令触发 -->
    <button class="demoBtn" v-on:click="doClick">{{clickMsg}}</button>

  </div>
</template>

<script>
export default {
  name: "myBtn",
  data: function() {
    return {
      msg: "我的按钮"
    };
  },

  //属性定义
  props: {
    defaultMsg: {
      default: "默认按钮"
    },
    clickMsg:{
        default:"点击按钮"
    }
  },

  //在组件初始化之后，一秒钟改变按钮的数据
  mounted() {
    //组件正式被初始化之后调用，数据驱动去改版按钮的内容
    var self = this;
    setTimeout(function() {
      self.msg = "改变按钮";
    }, 1000);
  },

  //点击按钮事件--方法
  methods: {
    doClick: function() {
      alert(this.clickMsg);
    }
  }
};
</script>

<style>
.demoBtn {
  width: 100px;
  height: 100px;
  padding: 10px;
  margin: 10px;
  font-size: 16px;
}
</style>