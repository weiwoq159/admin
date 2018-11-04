<template>
    <div id="app">
        <el-container>
            <el-header>

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
                username: '张丽丽'
            }
        }
    }

</script>

<style lang='stylus'>

</style>
