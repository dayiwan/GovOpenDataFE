<template>
    <div id="container" >
        <el-container direction="vertical" >
            <Header />
            <el-main>
               <router-view></router-view>
            </el-main> 
             <el-footer style="height: auto;">
                <Footer />
            </el-footer>
        </el-container>
    </div>
</template>

<script>
import Header from '@/layout/Header'
import Footer from '@/layout/Footer'
export default {
    components: {
        Header,
        Footer
    }
}
</script>

<style lang="scss">

* {
    box-sizing: border-box;
    text-decoration: none;
    font-family: "Microsoft YaHei"
}
html {
    height: 100%;
}
body{
    margin:0;
    padding:0;
    height: 100%;
    #container{
        display: flex;
        height: 100%;
        flex-direction: column;
        .el-header{
            background-color: #E9EEF3;
            color: #333;
            text-align: center;
            padding: 0 0px;
        }
        .el-main {
            background-color: aliceblue;
            color: #333;
            text-align: center;
            padding: 0px;
            
        }
        .el-footer {
            // background-color: #2b303b;
            // color: white;
            background-color: #E9EEF3;
            color: #333;
            text-align: center;
            padding: 0 0px;
        }
    }
}
</style>

