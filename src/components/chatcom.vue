<template>
    <div class="chatcom">
        <h1>和聊天{{msg}}</h1>
    </div>
</template>
<script>
export default {
    data(){
        return{

        }
    },
    props:['msg']
}
</script>
<style scoped>
.chatcom{
    height: 100%;
    width: 70%;
    background-color: pink;
}
</style>