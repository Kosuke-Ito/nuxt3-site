<script setup>
// const topics = ref(['photograph', 'engineering'])
</script>

<template>
  <div class="works">
    <nuxt-link to="/photograph" class="photograph">
      <h2>PHOTOGRAPH</h2>
    </nuxt-link>
    <nuxt-link to="/engineering" class="engineering">
      <h2>ENGEERING</h2>
    </nuxt-link>
  </div>

</template>

<style scoped>
.works {display: flex;justify-content: space-evenly;margin-top: 6rem;}
:where(.photograph, .engineering) {width: 45%;height: 30rem;display: flex;}
.engineering {background-color: blue;display: grid;place-items: center;color:aliceblue;}
.photograph {background-color: deeppink;display: grid;place-items: center;color:aliceblue;}
</style>
