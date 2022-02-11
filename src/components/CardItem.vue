<template>
   <div class="bg- black bg-opacify-20 rounded-3xl overflow-hidden">
      <div class="header">
        <div class="h-14 w-full flex ">
          <img src="https://via.placeholder.com/400x200" class=" w-full h-full object-cover" />
        </div>
      </div>

   <div> 
          <div class="body relative p-5">
        <avatar class="w-8 h-8 absolute right-2 -top-5 rounded-full overflow-hidden " />
      <h5 class="text-x5 mb-2  opacify-50">
          Andy William 
          <div class=" w-2 h-2 inline-block ml-2 rounded-full bg-green-400"></div>
      </h5>

      <p>Basic how to ride your skateboard comfortly</p>
        
        <div class="text-x5 flex items-center space-x-2 opacify-50 mt-5">
          <span>53k views</span>
          <div class="w-1 h-1 rounded-full bg-gray-300"></div>
          <span>2 weeks ago</span>
        </div>
    </div> 
   </div>   
 </div> 
   
</template>

<script setup>
import Avatar from "./Avatar.vue"
</script>