<template>
     <div  class="flex items-center space-x-4">
         <div class="bg-orange-500 p-2 rounded-1g">
              <component :is="icon" class="w-4 h-4"/>
         </div>
         
         <span>
              <slot></slot>
         </span>
      </div>
</template>

<script lang="ts" setup>
import HomeIcon from '../icons/Homeicon.vue'
import { defineProps } from "vue"; 
defineProps({
     icon: { default: null }
});
</script>