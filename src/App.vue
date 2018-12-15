<template>
    <div id="app">
        <img alt="Vue logo" src="./assets/logo.png">
        <Content/>
        info
    </div>
</template>

<script>
    import Content from './components/Content'

    export default {
        name: 'app',
        components: {
            Content
        }
    }
</script>

<style lang="scss">
    @import "assets/css/index.scss";
</style>
