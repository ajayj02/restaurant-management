<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Mycomp from './components/Mycomp.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="Bash on regarless" />
      <Mycomp name="Deepak" gender="his" callsign="Dick"/>
    </div>
  </header>
</template>

