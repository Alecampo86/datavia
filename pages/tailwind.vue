<template>
  <div class="container text-center bg-white mx-auto mt-5 h-100">
    <h1 class="text-center text-blue-500 text-6xl py-5 border">GRID COLS</h1>

    <div class="grid grid-cols-3 gap-4">
      <div class="bg-red-500">A</div>
      <div class="bg-red-500">A</div>
      <div class="bg-red-500">A</div>
      <div class="bg-red-500">A</div>
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 my-5">
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
    </div>

    <div class="grid grid-cols-4 gap-4 my-5">
      <div class="bg-pink-500 col-span-2">B</div>
      <div class="bg-pink-500">A</div>
      <div class="bg-pink-500">A</div>
      <div class="bg-pink-500 col-span-4">C</div>
    </div>

    <div class="grid grid-cols-12 gap-4 my-5">
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
    </div>

    <div class="grid grid-cols-4 gap-4">
      <div class="bg-green-500 col-start-3">A</div>
      <div class="bg-green-500">B</div>
      <div class="bg-green-500">C</div>
      <div class="bg-green-500">D</div>
    </div>
    <!-- /////////////////////////GRID ROWS /////////////////////////////-->
    <div>
      <h1 class="text-5xl p-5">GRID - ROWS</h1>
    </div>

    <div class="grid grid-rows-4 gap-4">
      <div class="bg-blue-500 row-span-4">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
      <div class="bg-blue-500">A</div>
    </div>

      <h1 class="text-3xl mt-3" >GRID-RESPONSIVE</h1>
    <!-- Responsive -->
  <div class="grid grid-rows-1 sm:grid-rows-2 grid-cols-1 sm:grid-cols-4 gap-2 mt-5">
    <div class="bg-pink-500 col-span-1">A</div>
    <div class="bg-pink-500 col-span-1">A</div>
    <div class="bg-pink-500 col-span-1 sm:col-span-2 row-span-1 sm:row-span-2">B</div>
    <div class="bg-pink-500 col-span-1">C</div>
    <div class="bg-pink-500 col-span-1">C</div>
  </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  min-height: 100vh;
}

/* Small (sm) */
@media (min-width: 640px) {
  /* ... */
}

/* Medium (md) */
@media (min-width: 768px) {
  /* ... */
}

/* Large (lg) */
@media (min-width: 1024px) {
  /* ... */
}

/* Extra Large (xl) */
@media (min-width: 1280px) {
  /* ... */
}
</style>
