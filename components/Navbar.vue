<template>
  <div class="navbar">
    <h1><nuxt-link to="/">{{ msg }}</nuxt-link></h1>
    <ul class="menu">
      <li v-for="item in items" :key="item.key" class="text-lg font-bold">
        <nuxt-link :to="`/${item}`">{{item}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script setup>
defineProps({
  msg: String
})
const items = ref(["works", "about"])
</script>

<style scoped>
h1 a{text-decoration: none;}
.navbar{
  padding-right: 2rem;
  display: flex;
  justify-content: space-between;
  align-items: baseline;
}
.menu{display: flex;}
.menu li{margin-left: .5rem;font-size: 1.2rem;list-style: none;}
</style>
