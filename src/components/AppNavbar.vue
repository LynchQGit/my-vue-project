<!-- 导航栏组件 -->
<template>
    <!-- nav 是一个导航栏 -->
    <nav class="navbar">
        <!-- div 的作用是用来定义文档中的分区或节（division/section）。 -->
        <!-- container 是一个容器 用来包裹内容 -->
        <div class="container">
            <!-- 这是一个导航栏 -->
            <a href="/" class="navbar-brand">MyVueApp</a>
            <div class="navbar-end">
                <button @click="login">Login</button>
                <button @click="register">Register</button>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'AppNavbar',
    methods: {
        login() {
            alert('login')
            console.log('login')
        },
        register() {
            alert('register')
            console.log('register')
        }
    }
}
</script>

<style scoped>
.navbar {
    background-color: #333;
    color: white;
    padding: 1rem 0;
}
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    /* margin 是外边距 */
    margin: 0 auto;
}
.navbar-brand {
    font-size: 1.5rem;
    text-decoration: none;
    color: white;
}
.navbar-end button {
    background-color: #fff;
    /* border 负责边框 */
    border: none;
    color: #333;
    /* rem 和 xp 是相对单位 */
    padding: 0.5rem 1rem;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    /* font-size: 16px; */
    margin-left: 1rem;
    cursor: pointer;
}
/* button:hover 是鼠标悬停时的样式 */
.navbar-end button:hover {
    background-color: #e7e7e7;
}
</style>