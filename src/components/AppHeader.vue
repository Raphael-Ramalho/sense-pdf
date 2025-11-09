<template>
  <header class="flex items-center justify-between px-6 py-4 relative z-10">
    <!-- Logo -->
    <div class="flex items-center space-x-2">
      <img src="@/assets/logo.png" class="h-20" alt="" />
    </div>
    
    <!-- Join wait list Button -->
    <div>
      <button 
        @click="$emit('openWaitlist')"
        class="text-gray-300 hover:text-white transition-colors"
      >
        Join the waitlist
      </button>
    </div>
  </header>
</template>

<script setup lang="ts">
// Define emits
defineEmits<{
  openWaitlist: []
}>()
</script>