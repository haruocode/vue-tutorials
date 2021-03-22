<template>
  <div class="privacy">
    <h1>{{ this.$route.params.id }}</h1>
    <p>{{ this.$route.query.q }}</p>
    <router-link tag="button" :to="{ name: 'first' }">First</router-link>
    <router-link tag="button" :to="{ name: 'second' }">Second</router-link>
    <router-view/>
  </div>
</template>
