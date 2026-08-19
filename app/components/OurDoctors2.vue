<template>

  <div class="container">
    <div class="row text-center pt-5">
      <h6 class="text-primary fw-bold">TRASTED CARE</h6>
      <h1 class="title">OUR DOCTORS</h1>
    </div>
  </div>

  <div class="container">
    <div class="row align-items-center g-4">


      <div class="col-12 col-md-6 col-lg-4">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-2.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>

      <div class="col-12 col-md-6 col-lg-4">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-1.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>

      <div class="col-12 col-md-6 col-lg-4">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-4.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 col-lg-4"  v-show="showAll">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-2.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 col-lg-4"  v-show="showAll">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-1.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>

      <div class="col-12 col-md-6 col-lg-4"  v-show="showAll">
        <div class="card w-100">
          <img
            src="~/assets/svg/rectangle-20-4.svg"
            class="card-img-top"
            alt="Doctor"
          >

          <div class="card-doc text-center">
            <p class="card-title">Doctor's name</p>
            <h6 class="card-text fw-bold">NEUROLOGY</h6>

            <div class="icons d-flex justify-content-center gap-3 pb-3">
              <i class="bi bi-linkedin fs-6"></i>
              <i class="bi bi-facebook fs-6"></i>
              <i class="bi bi-instagram fs-6"></i>
            </div>

            <button class="btn btn-profile w-100">
              View Profile
            </button>
          </div>
        </div>
      </div>

    </div>
  </div>
  <div class="text-center mt-4 pb-5">
  <button
    class="btn btn-profile px-4 rounded-pill"
    @click="showAll = !showAll"
  >
    {{ showAll ? 'Show Less' : 'View All Doctors' }}

    <i
      class="bi"
      :class="showAll ? 'bi-chevron-up' : 'bi-chevron-down'"
    ></i>
  </button>
</div>

  
</template>

<script setup>
import { ref } from 'vue'
import '~/assets/css/ourdoctors.css'

const showAll = ref(false)
</script>