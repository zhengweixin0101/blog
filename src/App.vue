<template>
  <div class="relative min-h-screen flex flex-col text-white">
    <Background />
    <Header />
    <div class="flex flex-1 bg-black/40 backdrop-blur-sm">
      <div class="flex-1 w-full flex flex-col px-4">
        <div class="w-full mx-auto flex-1 flex flex-col
                    max-w-full sm:max-w-[90vw] md:max-w-[85vw] lg:max-w-[75vw] 2xl:max-w-[60vw]">
          <div class="flex-1 relative z-10">
            <RouterView />
          </div>
          <Footer />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import Background from '@/components/Background.vue'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
</script>
