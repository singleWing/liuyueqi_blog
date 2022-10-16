<template>
    <div>
        <el-image
            style="width: 100px; height: 100px"
            :src="url">
            <div slot="error" class="image-slot">
                <i class="el-icon-picture-outline"></i>
            </div>
        </el-image>
        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
          <el-menu-item index="1">首页</el-menu-item>
          <el-menu-item index="2">菜单1</el-menu-item>
          <el-menu-item index="3">菜单2</el-menu-item>
          <el-menu-item index="4">菜单3</el-menu-item>
          <el-menu-item index="5">关于</el-menu-item>
        </el-menu>
    </div>
</template>

<script lang="ts">
    export default{
        data(){
            return{
                activeIndex:'1'
            }
        },
        methods:{
            handleSelect(key,keyPath){
                console.log(key,keyPath)
            }
        }
    }
</script>

<style>

</style>