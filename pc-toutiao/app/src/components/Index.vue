<template>
    <div class="main-container">
    <Header></Header>
    <div class='main'>
        <div class="main-left">
            <Nav></Nav>
        </div>
<<<<<<< HEAD
        <div class="main-center">
            <Comment></Comment>
        </div>
=======
        <div class="main-center"></div>
>>>>>>> 560d6fc7d3213f4217924a1f7ba9394b8959993d
        <div class="main-right">
            <div class="search-container">
                <Search></Search>
            </div>
            <div class="login-container">
                <Login></Login>
            </div>
            <div class="more-container">
                <More></More>
            </div>
            <div class="friends-link">
                <Friendslink></Friendslink>
            </div>
        </div>
    </div>
    </div>
</template>
<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';
import Nav from "./nav/Nav.vue"
import Header from "./header/Header.vue"
import Search from "./search/Search.vue"
import Login from "./login/Login.vue"
import More from "./more/More.vue"
import Friendslink from "./friendslink/Friendslink.vue"
import { VueEditor } from "vue2-editor";
import Comment from './comment/Comment'

export default {
//import引入的组件需要注入到对象中才能使用
components: {
    Nav,
    Header,
    Search,
    Login,
    More,
    Friendslink,
    VueEditor,
    Comment
},
data: function() {
//这里存放数据
    return {

    };
},
//监听属性 类似于data概念
computed: {

},
//监控data中的数据变化
watch: {

},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
//生命周期 - 创建之前
beforeCreate() {

},
//生命周期 - 挂载之前
beforeMount() {

},
//生命周期 - 更新之前
beforeUpdate() {

},
 //生命周期 - 更新之后
updated() {

},
//生命周期 - 销毁之前
beforeDestroy() {

},
//生命周期 - 销毁完成
destroyed() {

},
//如果页面有keep-alive缓存功能，这个函数会触发
activated() {

},
}
</script>
<style lang='less' scoped>
.main {
    display: flex;
    width: 100%;
    height: 100vh;

    .main-left {
        padding: 0 10px;
        display: flex;
        justify-content: flex-end;
        flex: 20%;
        nav {
            
        }
    }

    .main-center {
        flex: 50%;
    }

    .main-right {
        display: flex;
        flex-direction: column;

        justify-content: flex-start;
        flex: 30%;

        .search-container {
            margin: 10px 0;
            width: 70%;
            height: 50px;
            border: 1px solid grey;
            border-radius: 5px;
            overflow: hidden;
        }

        .login-container {
            margin: 10px 0;
            padding: 20px;
            width: 70%;
            height: 250px;
            background-color: #f4f5f6;
        }

        .more-container {
            margin: 10px 0;
            width: 70%;
            height: 220px;
        }

        .friends-link {
            margin: 10px 0;
            width: 70%;
            height: 220px;
        }
    }
}
</style>