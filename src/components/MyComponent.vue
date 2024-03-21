<template>
    <div>
        <p>This is a component</p>
        <!-- 添加一个按钮：反转消息 -->
        <p>{{ message }}</p>
        <button @click="reverseMessage">点我反转消息</button>
    </div>
</template>

<script>
export default {
    name: 'MyComponent',
    data() {
        return {
            message: 'Hello Vue!'
        }
    },
    methods: {
        reverseMessage() {
            this.message = this.message.split('').reverse().join('')
        }
    },
}
</script>

<style scoped>
/* 仅用于这个组件的样式 */
</style>