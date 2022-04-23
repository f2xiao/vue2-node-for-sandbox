<template>
  <div id="app">
     <nav class="flex justify-center space-x-4">
      <a href="/dashboard" class="font-medium px-3 py-2 text-slate-700 rounded-lg hover:bg-slate-100 hover:text-slate-900">Home</a>
      <a href="/team" class="font-medium px-3 py-2 text-slate-700 rounded-lg hover:bg-slate-100 hover:text-slate-900">Team</a>
      <a href="/projects" class="font-medium px-3 py-2 text-slate-700 rounded-lg hover:bg-slate-100 hover:text-slate-900">Projects</a>
      <a href="/reports" class="font-medium px-3 py-2 text-slate-700 rounded-lg hover:bg-slate-100 hover:text-slate-900">Reports</a>
    </nav>
    <h1 class="text-3xl font-bold underline">Hello world!</h1>
    <ul class="list-disc list-inside">
      <li>One</li>
      <li>Two</li>
      <li>Three</li>
    </ul>
    <div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-lg flex items-center space-x-4">
      <div class="shrink-0">
        <img class="h-12 w-12" src="@/assets/logo.png" alt="Logo">
      </div>
      <div>
        <div class="text-xl font-medium text-black">ChitChat</div>
        <p class="text-slate-500">You have a new message!</p>
      </div>
      <PrimaryButton>Reply</PrimaryButton>
    </div>

    <div class="p-6 max-w-sm mx-auto mt-4 bg-white rounded-xl">
      <div class="flex items-center space-x-2 text-base">
        <h4 class="font-semibold text-slate-900">Contributors</h4>
        <span class="rounded-full bg-slate-100 px-2 py-1 text-xs font-semibold text-slate-700">204</span>
      </div>
      <div class="mt-3 flex -space-x-2 overflow-hidden">
        
          <img class="inline-block h-12 w-12 rounded-full ring-2 ring-white" src="@/assets/logo.png" />
          <img class="inline-block h-12 w-12 rounded-full ring-2 ring-white" src="@/assets/logo.png" />
          <img class="inline-block h-12 w-12 rounded-full ring-2 ring-white" src="@/assets/logo.png" />
        
      </div>
      <div class="mt-3 text-sm font-medium">
        <a href="#" class="text-blue-500">+ 198 others</a>
      </div>

    </div>

   <div class="mx-auto max-w-sm bg-white mt-2 flex-auto">
      <vacation-card :eyebrow="'abc'" :imgAlt="'image'" :pricing="'$299CAD'" :title="'ABC'" :url="'#'" :img="imgurl"></vacation-card>
      <button class="rounded bg-violet-500 hover:bg-violet-600 active:bg-violet-700 focus:outline-none focus:ring focus:ring-violet-300">
        Add to Cart
      </button>
   </div>

  <div class="max-w-md mx-auto bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl">
  <div class="md:flex">
    <div class="md:shrink-0">
      <img class="h-48 w-full object-cover md:h-full md:w-48" src="/img/store.jpg" alt="Man looking at item at a store">
    </div>
    <div class="p-8">
      <div class="uppercase tracking-wide text-sm text-indigo-500 font-semibold">Case study</div>
      <a href="#" class="block mt-1 text-lg leading-tight font-medium text-black hover:underline">Finding customers for your new business</a>
      <p class="mt-2 text-slate-500">Getting a new business off the ground is a lot of hard work. Here are five ideas you can use to find your first customers.</p>
    </div>
  </div>
</div>  
   <div class="bg-white dark:bg-slate-900 rounded-lg px-6 py-8 ring-1 ring-slate-900/5 shadow-xl">
  <div>
    <span class="inline-flex items-center justify-center p-2 bg-indigo-500 rounded-md shadow-lg">
      <svg class="h-6 w-6 text-white" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true"><!-- ... --></svg>
    </span>
  </div>
  <h3 class="text-slate-900 dark:text-white mt-5 text-base font-medium tracking-tight">Writes Upside-Down</h3>
  <p class="text-slate-500 dark:text-slate-400 mt-2 text-sm">
    The Zero Gravity Pen can be used to write in any orientation, including upside-down. It even works in outer space.
  </p>
</div>
  </div>
</template>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: rgb(19, 27, 46);
  min-height: 100vh;
}
</style>
<script>
import PrimaryButton from "@/components/PrimaryButton.vue"
import VacationCard from "@/components/VacationCard.vue"
import logo from "@/assets/logo.png"
export default {
  computed: {
    imgurl(){
      return logo
    }
  },
  components:{
    PrimaryButton,
    VacationCard
  }
}
</script>
