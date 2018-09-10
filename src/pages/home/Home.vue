<template>
    <div class="home-page">
        this is home page~
        <button @click="changeTheme('')">换默认</button>
        <button @click="changeTheme('1')">换红肤</button>
        <button @click="changeTheme('2')">换蓝肤</button>
        <button @click="changeTheme('3')">换绿肤</button>
    </div>
</template>

<script>
export default {
    name: 'Home',
    methods: {
        changeTheme (theme) {
            window.document.documentElement.setAttribute('data-theme', theme)
        }
    }
}
</script>

<style lang="scss">
.home-page {
    @include textColor();
}
</style>
