<template>
  <header class="bg-white shadow h-24 flex justify-between items-stretch">
    <router-link :to="{ name: 'home' }" class="inline-flex items-center h-full px-5">
      Home
    </router-link>
    <div class="flex items-center gap-1">
      <router-link
        :to="{ name: 'byName' }"
        class="inline-flex items-center px-2 h-full hover:bg-purple-100 transition-colors"
      >
        Meals by Name
      </router-link>

      <router-link
        :to="{ name: 'byLetter' }"
        class="inline-flex items-center px-2 h-full hover:bg-purple-100 transition-colors"
      >
        Meals by Letter
      </router-link>

      <router-link
        :to="{ name: 'byIngredient' }"
        class="inline-flex items-center px-2 h-full hover:bg-purple-100 transition-colors"
      >
        Meals by Ingredients
      </router-link>
    </div>
  </header>
</template>
