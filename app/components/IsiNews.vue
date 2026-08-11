<template>
  <div class="container">
    <div class="row pt-4">

      <div
        v-for="article in articles"
        :key="article.id"
        class="col-lg-8 mx-auto mb-4"
      >

        <div class="card mb-3 border-0">

          <img
            :src="article.image"
            :alt="article.title"
            class="card-img-top"
          >

          <div class="card-body">

            <div class="d-flex align-items-center flex-wrap gap-3">

              <small>
                <i class="bi bi-calendar3 me-1"></i>
                {{ article.date }}
              </small>

              <small>
                <i class="bi bi-person me-1"></i>
                {{ article.author }}
              </small>

              <small>
                <i class="bi bi-eye me-1"></i>
                {{ article.views }}
              </small>

              <small class="text-danger">
                <i class="bi bi-heart me-1"></i>
                {{ article.likes }}
              </small>

            </div>

            <h5 class="card-title card-isi-news">
              {{ article.title }}
            </h5>

            <p class="card-text card-text-isi-news">
              {{ article.description }}
            </p>

          <NuxtLink
  :to="`/isiartikel/${article.id}`"
  class="btn read-btn px-4 rounded-pill"
>
  Read More
  <i class="bi bi-arrow-right px-1"></i>
</NuxtLink>
          </div>
        </div>

      </div>

    </div>
  </div>
</template>

<script setup>
import articles from '~/data/isi-news.json'
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

.bi-arrow-right {
  color: #1F2B6C;
}

.bi-calendar3 {
  color: #1F2B6C;
}
</style>