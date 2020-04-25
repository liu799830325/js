<template>
    <div class="index-head">
        <div class="head1" v-for="(list,index) in lists"  :key="index">
            <i  class="iconfont" v-bind:class="list.icon" :style="{background:list.color}"></i>
            <lable>{{list.title}}</lable>
        </div>
       
    </div>
</template>
<script>
export default {
    data() {
        return {
            
            lists:[
                {title:'美食',icon:'el-icon-eleme',color:'red'},
                {title:'电影',icon:'el-icon-s-shop',color:'blue'},
                {title:'旅游',icon:'el-icon-s-shop',color:'red'},
                {title:'商店',icon:'el-icon-s-goods',color:'green'},
            ]
        }
    },
}
</script>
<style scoped>
/* .head > .head1{
    display: inline-block;
    width: 25%;
    float: left;
} */
 .index-head{
    /* position:absolute; */
    margin-top: 5%; 
}
.index-head .head1{
    width: 25%;
    float: left;
    text-align: center;
}
.index-head .head1 .iconfont{
    font-size: 40px;
    display:inline-block;
    border-radius: 50%;
    color: whitesmoke;
}
.index-head lable{
    display: block;
}
/* .head1{ 
    width: 1000px;
    background: darkkhaki;
    position:absolute;
    
    float: left;
    margin: 0 auto;
}  */
/* .head1 i {
    position:absolute;
    display: block;
    font-size: 50px; 
 }   */

</style>