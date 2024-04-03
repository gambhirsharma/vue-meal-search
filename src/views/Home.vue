<template>
  <div class="flex items-center justify-center p-8">
    <input
      type="text"
      class="text-black rounded border-2 border-gray-200 w-full"
      placeholder="Search for Meals"
    />
    <div class="flex gap-1"></div>
  </div>
</template>

<script setup>
import { computed } from 'vue'
import store from '../store'

const meals = computed(() => store.state.meals)
const letters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'.split('')
</script>
