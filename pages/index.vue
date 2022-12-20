<template>
  <div class="isolate text-white bg-back h-screen">
    <Planet src="/images/Planet%201.svg" class="w-32 inset-y-36 left-72"></Planet>
    <Planet src="/images/Planet%202.svg" class="w-46 inset-y-2/3 left-28"></Planet>
    <Planet src="/images/Planet%203.svg" class="w-36 inset-y-1/3 right-28"></Planet>
    <Planet src="/images/Planet%204.svg" class="w-28 bottom-12 right-72"></Planet>
    <Star v-for="index in 20" :key="index"></Star>
    <VHeader></VHeader>
    <!--  Create an invisible duplicate of the header for layout purposes  -->
    <VHeader class="invisible !block !static"></VHeader>
    <div class="w-full flex-center flex-col gap-8 lg:p-40 z-20">
      <p
        class="z-20 text-center max-w-7xl animate-gradientMove bg-enlarge text-transparent bg-gradient-to-r from-red-light via-purple-500 via-pink-500 to-yellow-mid bg-clip-text text-6xl lg:text-8xl font-bold">
        The Next-Gen Website Builder.</p>
      <p class="z-20 text-xl">
        Rapid web development re-imagined in one simple, coherent tool that can satisfy your every need through its
        myriad of features.
      </p>
      <div class="mt-4 flex-center gap-16 text-md">
        <a class="z-20 p-4 px-12 bg-dark-dark ring-offset-4 ring-offset-back ring-2 ring-red-mid rounded-2xl">Get
          Started</a>
        <a
          class="z-20 p-4 px-12 bg-dark-dark ring-offset-4 ring-offset-back ring-2 ring-dark-dark rounded-2xl">Documentation</a>
      </div>
    </div>
    <div class="h-screen">
      test
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
