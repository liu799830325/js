<template>
    <div class="nav-buttom">
        <router-link to="/home">
        <i class="el-icon-s-home"></i>
        <label>首页</label>
        
        </router-link>
        <router-link to="/find">
        <i class="el-icon-search"></i>
        <label>发现</label>
        
        </router-link>
        <router-link to="/order">       
        <i class="el-icon-s-order" ></i>
        <label>订单</label>
        
        </router-link>
        <router-link to="/my">     
        <i class="el-icon-s-custom" ></i>  
        <label>我的</label>
        
        </router-link>
    </div>
</template>
<script>
  

export default {
    data() {
        return {
            name:"首页"
        }
    },
}
</script>
<style scoped>
div{
    height: 40px;
    margin-bottom: 0px;
}
.nav-buttom{
    height: 50px;
    position:fixed;
    bottom: 0;
    background: darkgrey;
    border-top:1px solid #f4f4f4;
    padding-top: 5px;
    width: 100%;
    /* line-height: 50px; */
    font-size: 18px;
}
.nav-buttom > a{
    display: inline-block;
    width: 25%;
    float: left;
    text-decoration: none;
}
a:hover{
    background: firebrick;
}
.nav-buttom i{
    display: block;
    font-size: 26px;
}
.router-link-active {
            color:red;
            font-weight: 700;
            font-style: italic;
            text-decoration: none;
            font-size: 15px;
        }

</style>