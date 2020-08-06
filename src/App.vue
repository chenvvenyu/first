<template>
  <div id="app">
    <div class="box">
      <chat-com :msg='onile'></chat-com>
      <userlist-com :list='list' @choose='choose'></userlist-com>
    </div>
  </div>
</template>

<script>
import chatCom from "./components/chatcom";
import userlistCom from "./components/userlist";
export default {
  name: "App",
  components: {
    chatCom,
    userlistCom,
  },
  data() {
    return {
      msg: 12333,
      list:['小明','小万','小红','李四','万万'],
      onile:'小明'
    };
  },
  methods:{
    choose(index){
      this.onile=this.list[index]
    }
  }
};
</script>

<style>
.box {
  height: 500px;
  width: 500px;
  background-color: aqua;
  display: flex;
}
</style>

