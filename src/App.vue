<template>
  <div id="nav" style="display:none;">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view />
</template>

<style lang="scss">
* {
    margin: 0;
    padding: 0;
}
</style>
