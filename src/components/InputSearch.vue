<template>
<div class="relative text-white">
   <input
       type="text"
       class="w-full bg-gray-700 placholder-white px-4 py-2 rounded-lg opacity-30 focus:opacity-60 outline-nome focus:outline-nome pr-10 "
       placeholder="Search"
   />
   <SearchIcon class="w-4 h-4 absolute  top-2.5 right-2.5" />
</div>
</template>

<script setup>
import SearchIcon from "../components/icons/SearchIcon.vue"
</script>