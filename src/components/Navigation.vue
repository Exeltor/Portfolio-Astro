<template>
  <button class="rounded-lg bg-white text-black hover:bg-black hover:text-white p-2" @click="showNavbar = true">
    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
    </svg>
  </button>
  <div v-if="showNavbar" class="absolute z-10 top-0 left-0 grid grid-cols-3 h-screen w-screen blurred">
    <div class="col-span-2 h-screen pl-20 flex flex-col justify-center">
      <p class="text-7xl font-bold border-r-2 border-white text-white">Where do you want to go?
        <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 inline" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
        </svg>
      </p>
    </div> 
    <div class="px-8 font-medium flex flex-col justify-center pr-20">
      <a href="/education" class="group flex flex-row items-center hover:bg-white rounded-3xl p-4">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-14 w-14 mr-14 text-white group-hover:text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path d="M12 14l9-5-9-5-9 5 9 5z" />
          <path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z" />
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222" />
        </svg>
        <p class="group-hover:text-black text-white">Education</p>
      </a>
      <a class="group flex flex-row items-center hover:bg-white rounded-3xl p-4">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-14 w-14 mr-14 text-white group-hover:text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
        </svg>
        <p class="group-hover:text-black text-white">Work Experience</p>
      </a>
      <a class="group flex flex-row items-center hover:bg-white rounded-3xl p-4">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-14 w-14 mr-14 text-white group-hover:text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
        </svg>
        <p class="group-hover:text-black text-white">Skills</p>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  data() {
    return {
      showNavbar: false
    }
  }
}
</script>

<style>

</style>