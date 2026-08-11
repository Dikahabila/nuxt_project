<template>
  <Navbar />

  <HeroIsiArtikel />

  <IsiArtikel
    v-if="article"
    :article="article"
  />

  <div v-else class="container py-5 text-center">
    <h3>Artikel tidak ditemukan</h3>
  </div>

  <Contact />

  <Footer />
</template>

<script setup>
import { computed } from 'vue'
import { useRoute } from 'vue-router'
import articles from '~/data/isi-news.json'

const route = useRoute()

const article = computed(() => {
  const id = Number(route.params.id)

  return articles.find(item => item.id === id)
})
</script>