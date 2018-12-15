<template>
    <div id="app">

        <header class="header">
            <div id="nav">
                <router-link to="/">Home</router-link>
                |
                <router-link to="/templates">Templates</router-link>
            </div>
        </header>

        <main>
            <router-view/>
        </main>

        <footer class="footer"
        >
            copyright
        </footer>
    </div>
</template>

<style lang="scss">
    @import "assets/css/index.scss";
</style>
