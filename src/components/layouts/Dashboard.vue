<template>
  <div class="bg-gray-800 flex text-white max-h-screen h-screen">
    <div class="w-64">
     <span class="font-semibold p-6  block opacity-90">skateboard</span>

        <nav class="o-6">
           <h3 class="opacity-50 uppercase font-semibold tracking-wider mb-6 text-xs">Menu</h3>
        
          <div class="space-y-6">                  
               <MenuItem :icon="HomeIcon">Discover</MenuItem>
               <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
               <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
               <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
               <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
               <MenuItem :icon="TrendingUpIcon">Trending</MenuItem>
          </div>  
        </nav> 
    </div>

    <div class="  flex-1 h-screen relative overflow-y-auto">
      <header class="flex p-5 bg-gray-800 z-20 sticky top-0 items-center justify-between">
       <InputSearch class="w-96" />
     
     <div class="flex items-center">
       <div class="flex items-center space-x-3">
         <div class="w-10 h-10 ">
             <Avatar class="rounded-full overflow-hidder w10 h-10" />
         </div>
          <span>thonas</span>
          <chevronDownIcon class="w-4 h-4" /> 
       </div >

       <BellIcon class="w-4 h-4 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition duration-100" /> 
        </div> 
      </header>
     <div class="px-5 pb-5 content">
      <h1 class="font-bold text-4xl mt-6 mb-4">Discover</h1>
      <div class="grid gap-4 grid-cols-12">
      <div class="col-span-6 h-40 rounded-3xl  overflow-hidden relative">
        <div class=" flex w-ful h-full ">
          <img src="https://via.placeholder.com/2000x1400"
           class="w-full object-cover"
           />        
       </div>
       <div class="z-10 absolute top-0 p-6 w-full botton-0  "> 
            <h3 class="text-2xl max-w-xs"
            > How to do Basic Jumping and  landing safely</h3> 

         <div class="absolute right-2 botton-6 px-2 py-0 rounded-lg  bg-gray-800 bg-opacity-50 text-white"
         >7 minutes</div>       
      </div>  
    </div>


          <div class="col-span-4 h-36 rounded-3xl  overflow-hidden relative">
        <div class=" flex w-ful h-full ">
          <img src="https://via.placeholder.com/2000x1400"
           class="w-full object-cover" 
          />        
       </div>

       <div class="z-10 absolute top-0 p-6 w-full botton-0  "> 
            <h3 class="text-2xl max-w-xs"
            > How to do Basic Jumping and  landing safely</h3> 

         <div class="absolute right-2 botton-6 px-2 py-0 rounded-lg  bg-gray-800 bg-opacity-50 text-white"
         >7 minutes</div>       
       </div>  
       </div>
      </div>  
      
        <h1 class=" text-2xl mt-6 mb-4">Most Watched</h1>

        <div class="grid grid-cols-4 gap-4">
            <CardItem v-for="n of 10" />
        </div>
     </div>
       </div>
    </div>  
</template>

<script lang="ts" setup>
import HomeIcon from "../icons/Homeicon.vue"
import TrendingUpIcon from "../icons/TrendingUIconp.vue"
import chevronDownIcon from "../icons/ChevronDownIcon.vue"
import BellIcon from "../icons/BellIcon.vue"
import MenuItem from "../navs/MenuItem.vue";
import InputSearch from "../InputSearch.vue"
import Avatar from "../Avatar.vue"
import CardItem from "../CardItem.vue"
</script>