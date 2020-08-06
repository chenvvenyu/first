<template>
    <div class="userlist">
        <div v-for="(item,index) in list" :key="index" @click="choose(index)">
            <h3 >{{item}}</h3>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{

        }
    },
    props:['list'],
    methods:{
        choose(index){
            this.$emit('choose',index)
        }
    }
}
</script>

<style  scoped>
.userlist{
    width: 30%;
    height: 100%;
}
</style>