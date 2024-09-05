<template>
  <input type="text" name="" id="">
  <p>{{ meals }}</p>
</template>

<script setup>
import store from "@/store";
import { computed } from "vue";


  const meals = computed(() => store.state.meals);

</script>