<template>
  <div class="relative group">
    <div
      class="absolute inset-0 bg-gradient-to-r from-gray-100 to-gray-900 shadow-md hover:shadow-lg transition-all duration-300 transform -skew-y-6 sm:skew-y-0 sm:-rotate-6 group-hover:md:-rotate-10 group-hover:shadow-md rounded-xl md:rounded-3xl">
    </div>
    <div
      class="relative bg-white rounded-xl md:rounded-3xl shadow-md hover:shadow-lg transition-all duration-300  p-8 flex flex-col items-center justify-between  h-full">
      <h1
        class="font-bold text-center pb-2 md:pb-4 text-lg sm:text-xl md:text-2xl uppercase">
        {{ title }}</h1>
      <div class="px-4 text-gray-600 text-lg text-center">
        {{ description }}
      </div>
      <div
        class="bg-gray-900 text-white py-2 px-4 block rounded mt-4 text-lg text-center">
        {{ price }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title', 'description', 'price']
}
</script>

<style lang="css">
.footer-2 {
  color: #ff0000!important;
}
</style>
