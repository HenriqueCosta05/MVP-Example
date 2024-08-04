<template>
  <nav
    class="relative block w-full min-w-screen-xl px-6 py-3 mx-auto text-white bg-white border shadow-md rounded-xl border-white/80 bg-opacity-80 backdrop-blur-2xl backdrop-saturate-200">
    <div class="flex items-center justify-between text-blue-gray-900 flex-col lg:flex-row">
      <a href="#"
        class="mr-4 block cursor-pointer py-1.5 font-sans text-base font-semibold leading-relaxed tracking-normal text-inherit antialiased">
        MVP Front-end example
      </a>
      <!--LG + -->
      <div class="hidden lg:block">
        <ul class="flex flex-col gap-2 my-2 lg:mb-0 lg:mt-0 lg:flex-row lg:items-center lg:gap-6">
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Pages
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Account
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Blocks
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Docs
            </a>
          </li>
        </ul>
      </div>
      <!--LG or minor-->
      <div class="flex justify-center items-center flex-col lg:hidden" data-collapse="collapse">
        <ul class="flex flex-col gap-2 my-2 lg:mb-0 lg:mt-0 lg:flex-row lg:items-center lg:gap-6" data-collapse-content>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Pages
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Account
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Blocks
            </a>
          </li>
          <li class="block p-1 font-sans text-sm antialiased font-medium leading-normal text-blue-gray-900">
            <a href="#" class="flex items-center transition-colors hover:text-blue-500">
              Docs
            </a>
          </li>
        </ul>
      </div>
      <button
        class="absolute top-0 right-0 mt-2 mr-2 h-6 max-h-[40px] w-6 max-w-[40px] select-none rounded-lg text-center align-middle font-sans text-xs font-medium uppercase text-inherit transition-all hover:bg-transparent focus:bg-transparent active:bg-transparent disabled:pointer-events-none disabled:opacity-50 disabled:shadow-none lg:hidden"
        type="button"
        data-collapse-target="collapse">
        <span class="absolute transform -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor"
            aria-hidden="true" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"></path>
          </svg>
        </span>
      </button>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  mounted() {
    if (process.client) {
      import('@material-tailwind/html/scripts/collapse.js')
    }
  }
}
</script>

<style scoped>
/* Add any component-specific styles here */
</style>
