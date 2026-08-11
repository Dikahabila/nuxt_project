<template>
  <div class="container">
    <div class="row pt-4">
      <div class="col-lg-8 mx-auto">

        <div class="card mb-3 border-0">

          <!-- Gambar artikel -->
          <img
            :src="article.image"
            :alt="article.title"
            class="card-img-top"
          >

          <div class="card-body">

            <!-- Isi artikel -->
            <p class="card-text card-text-isi-news">
              {{ article.content }}
            </p>

            <!-- Previous & Next -->
            <div class="d-flex justify-content-between mt-4">

              <NuxtLink
                v-if="article.id > 1"
                :to="`/isiartikel/${article.id - 1}`"
                class="btn read-btn px-4 rounded-pill"
              >
                <i class="bi bi-arrow-left me-1"></i>
                Previous Article
              </NuxtLink>

              <span v-else></span>

              <NuxtLink
                v-if="article.id < totalArticles"
                :to="`/isiartikel/${article.id + 1}`"
                class="btn read-btn px-4 rounded-pill"
              >
                Next Article
                <i class="bi bi-arrow-right ms-1"></i>
              </NuxtLink>

            </div>

          </div>
        </div>

      </div>
    </div>
  </div>
</template>


<script setup>
import articles from '~/data/isi-news.json'

const props = defineProps({
  article: {
    type: Object,
    required: true
  }
})

const totalArticles = articles.length
</script>


<style>
.card-isi-news {
  color: #1F2B6C;
  font-family: "Yesefa One", serif;
  font-size: 32px;
}

.bi-person {
  color: #159EEC;
}

.card-text-isi-news {
  color: black;
}

.read-btn {
  color: #1F2B6C;
  background-color: #9DB9F6;
}

.bi-arrow-right,
.bi-arrow-left {
  color: #1F2B6C;
}

.bi-calendar3 {
  color: #1F2B6C;
}
</style>