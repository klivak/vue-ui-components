<template>
  <div id="app">
    <header>
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/banner">Banner</router-link>
      </div>
    </header>
    <main>
      <router-view/>
    </main>
    <footer>

    </footer>
  </div>
</template>

<style lang="scss">
    @import "assets/css/index.scss";
</style>
