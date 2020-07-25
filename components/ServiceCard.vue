<template>
  <div
    class="bg-white shadow-md hover:shadow-lg transition-all duration-300 px-4 py-8 rounded">
    <h1
      class="font-bold text-center pb-2 md:pb-8 text-lg sm:text-xl md:text-2xl uppercase">
      {{ title }}</h1>
    <div class="flex items-center justify-between">
      <div>
        <slot></slot>
      </div>
      <div class="pl-4 pr-4  block text-lg">
        {{ description }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['title', 'description']
}
</script>
