<template>
  <!-- Judul -->
  <div class="row text-center pt-5">
    <h6 class="text-primary fw-bold">
      {{ contactData.subtitle }}
    </h6>

    <h1 class="title">
      {{ contactData.title }}
    </h1>
  </div>

  <!-- Cards -->
  <div class="container">
    <div class="row g-4 mt-2">

      <div
        v-for="(card, index) in contactData.cards"
        :key="index"
        class="col-lg-3"
      >

        <div class="card w-75 mx-auto">

          <div
            class="card-body"
            :class="card.theme"
          >

            <div class="pt-4">
              <i
                :class="`bi ${card.icon} fs-2`"
              ></i>
            </div>

            
            <h5
              class="fw-bold"
              :class="card.titleClass"
            >
              {{ card.title }}
            </h5>

            
            <p
              v-for="(item, itemIndex) in card.items"
              :key="itemIndex"
              class="card-subtitle mb-2"
              :class="card.subtitleClass"
            >
              {{ item }}
            </p>

          </div>

        </div>

      </div>

    </div>
  </div>
</template>

<script setup>
import contactData from '../data/contact.json'

import '~/assets/css/contact.css'
</script>