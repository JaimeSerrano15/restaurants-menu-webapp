<template>
  <div class="p-8">
    <input type="text" class="rounded border-2 border-gray-400 w-full" placeholder="Search for Meals" v-model="keyword" @change="searchMeals">
  </div>

  <div>
    <pre>{{ meals }}</pre>
  </div>
</template>

<script setup>
  import store from '@/store';
  import { computed, ref } from 'vue';
  
  const keyword = ref('');
  const meals = computed(() => store.state.searchedMeals);

  function searchMeals() {
    console.log(keyword.value);
    
    store.dispatch('searchMeals', keyword.value);
  }

</script>