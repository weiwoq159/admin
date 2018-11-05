<template>
    <div id="app">
        <el-container>
            
            <el-header height='80px'>
                <el-row>
                    <el-col :span="8" class='header-left'>
                        <a class="logo" href=''><img src="./assets/u8.png" alt=""></a>
					    <p class="title">商誉宝 <span>管理员系统</span></p>
                    </el-col>
                    <el-col :span="8" :offset="6" class='user'>
                        <p>你好，<span>{{username}}</span> <a href="">退出</a></p>
                    </el-col>
                </el-row>
                
            </el-header>
            
            <el-main>
                <!-- Main content -->
                
            </el-main>
            <el-footer>
                <!-- Footer content -->
            </el-footer>
        </el-container>
        <router-view />
    </div>
</template>

<script>
    export default {
        name: 'App',
        data() {
            return {
                username: '张丽丽1'
            }
        }
    }

</script>

<style lang='stylus'>
$black = #000
$white = #fff
body
    margin 0px
    .el-container
        color $white
        .el-header
            background $black
            .el-row
                height 80px
                width 80%
                margin 0 auto
                .logo
                    float left
                    line-height 80px
                    height 80px
                    img
                        vertical-align middle                        
                .title
                    float: left;
                    height: 27px;
                    font-size: 18px;
                    padding-left: 10px;
                    border-left: 1px solid #fff;
                    margin-top: 30px;
                    margin-left: 10px;
                    line-height: 36px;
                    color: #fff;
                .user
                    font-size: 12px;
                    font-family: "Microsoft YaHei";
                    color: rgb(251, 251, 251);
                    line-height: 100px;
                    text-align: right;
                    a
                        margin-left: 20px;
                        color: #fff;
                        text-decoration: none;
</style>
