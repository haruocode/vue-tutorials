<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/privacy">プライバシーポリシー</router-link> |
      <router-link :to="{ name: 'user', params: { id: 1 }, query: { q: 'hogehoge' } }">ユーザー1</router-link>
    </div>
    <router-view />
  </div>
</template>

<style scoped>
#nav a.router-link-exact-active {
  color: deeppink;
  font-size: 30px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}
</style>
