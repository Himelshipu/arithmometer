<template>
  
  <!-- calculator -->
<div class="mx-auto overflow-hidden mt-10 shadow-lg mb-2 bg-gray-300 shadow-lg border rounded-lg lg:w-2/6 md:w-3/6 sm:w-4/6">
    <div class="">
    
      <div class="p-5 text-white text-center text-3xl bg-blue-500">
          <img alt="Vue logo" src="./assets/favicon.png" class="mx-auto h-12">
        <span class=" uppercase">Arithmometer</span></div>
      <div class="pt-16 p-5 pb-0 text-blue-500 text-right text-3xl bg-gray-200">2000 + 100</div>
      <div class="p-5 text-white text-right text-3xl bg-blue-500">= <span class="text-orange-500">2100</span></div>
      
      
 <div class="flex items-stretch  h-24">

    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold ">
      <div class="shadow-2xl rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">%</div>
    </div>
  
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">(</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">)</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">÷</div>
    </div>
</div>
      
<div class="flex items-stretch  h-24">
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">7</div>
    </div>
  
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">8</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">9</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">×</div>
    </div>
</div>
      
<div class="flex items-stretch  h-24">
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">4</div>
    </div>
  
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">5</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">6</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">-</div>
    </div>
</div>
      
<div class="flex items-stretch  h-24">
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">1</div>
    </div>
  
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">2</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">3</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">+</div>
    </div>
</div>
      

<div class="flex items-stretch h-24 mb-4">
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">+</div>
    </div>
  
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">0</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">.</div>
    </div>
   
    <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
      <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none">=</div>
    </div>
</div>
      
      
  </div>
</div>



  <HelloWorld msg="Welcome to Your Vue.js App"/>


</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
// import './assets/tailwind.css'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
