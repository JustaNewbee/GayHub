<template>
    <div id="app">
        <page-header></page-header>
        <router-view/>
    </div>
</template>

<script>
import PageHeader from './components/Header'
export default {
    name: 'App',
    components: {
        PageHeader
    }
}
</script>

<style>
body {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
</style>
