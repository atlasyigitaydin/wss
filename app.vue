<script setup lang="ts">
const screenShotStore = useScreenShotStore()

useHead({
  title: 'WSS – Kolay ve Hızlı Görüntü Çekme Aracı',
  meta: [
    {
      name: 'description',
      content: 'Hızlı ve kolay bir şekilde ekran görüntüsü alın. URL girerek istediğiniz sayfanın ekran görüntüsünü alabilir, hemen indirip kaydedebilirsiniz.',
    },
    {
      name: 'keywords',
      content: 'ekran görüntüsü, screenshot, web screenshot, ekran görüntüsü alma aracı, web sayfası fotoğrafı',
    },
    {
      property: 'og:title',
      content: 'Ekran Görüntüsü Al – Kolay ve Hızlı Görüntü Çekme Aracı',
    },
    {
      property: 'og:description',
      content: 'Ekran görüntüsü al, her cihazda yüksek kaliteli fotoğraflar elde et. Kolayca URL gir ve hemen indirmeye başla.',
    },
    {
      property: 'og:image',
      content: 'https://wss.atlasyigitaydin.com',
    },
    {
      property: 'og:url',
      content: 'https://wss.atlasyigitaydin.com',
    },
    {
      property: 'og:type',
      content: 'website',
    },
    {
      name: 'twitter:card',
      content: 'summary_large_image',
    },
    {
      name: 'twitter:title',
      content: 'Ekran Görüntüsü Al – Kolay ve Hızlı Görüntü Çekme Aracı',
    },
    {
      name: 'twitter:description',
      content: 'Hızlı ve yüksek kaliteli ekran görüntüsü alma aracı. URL girin, görüntüyü alın ve hemen indirin.',
    },
    {
      name: 'twitter:image',
      content: 'https://wss.atlasyigitaydin.com',
    },
  ],
  link: [
    {
      rel: 'canonical',
      href: 'https://wss.atlasyigitaydin.com',
    },
  ],
})
</script>

<template>
  <div class="fixed top-12 left-0 w-full text-white animate-pulse z-50 h-12 flex justify-center items-center">
    <div class="bg-red-600 font-bold rounded px-3 py-2">
      SYSTEM ERROR!
    </div>
  </div>
  <Loading :loading="screenShotStore.loading" />
  <NuxtPage />
</template>
