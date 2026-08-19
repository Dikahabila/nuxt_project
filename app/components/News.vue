<template>

  <!-- Section Title -->
  <div class="container">
    <div class="row text-center pt-5">
      <h6 class="text-primary fw-bold">
        BETTER INFORMATION, BETTER HEALTH
      </h6>

      <h1 class="title">
        News
      </h1>
    </div>
  </div>


  <!-- News Cards -->
  <div class="container">

    <div class="row g-4 justify-content-center pt-3">

      <div
        v-for="post in articles"
        :key="post.id"
        class="col-lg-6"
      >
<NuxtLink
  :to="`/isiartikel/${post.id}`"
  class="text-decoration-none"
>
        <div
          class="card mb-3 border-0 shadow-sm"
          style="max-width: 540px;"
        >

          <div class="row g-0">

            <!-- Image -->
            <div class="col-md-4">

              <img
                :src="post.image"
                class="img-fluid rounded-start"
                :alt="post.title"
              >

            </div>


            <!-- Content -->
            <div class="col-md-8">

              <div class="card-body-news mx-2">

                <!-- Date & Author -->
                <p class="card-title-news">
                  {{ post.date }} | {{ post.author }}
                </p>


                <!-- Title -->
                <h6 class="card-text-news">
                  {{ post.title }}
                </h6>


                <!-- Views & Likes -->
                <div class="d-flex gap-3">

                  <div class="d-flex align-items-center">
                    <i class="bi bi-eye"></i>

                    <span class="ms-2">
                      {{ post.views }}
                    </span>
                  </div>


                  <div class="d-flex align-items-center">
                    <i class="bi bi-heart"></i>

                    <span class="ms-2">
                      {{ post.likes }}
                    </span>
                  </div>

                </div>


            

              </div>

            </div>

          </div>

        </div>
        </NuxtLink>

      </div>

    </div>

  </div>


  <!-- Dots -->
  <div class="dots text-center">
    <i class="bi bi-three-dots fs-1"></i>
  </div>

</template>


<script setup>

import articles from '~/data/isi-news.json'

import '~/assets/css/news.css'

</script>