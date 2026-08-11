<template>
  <nav class="navbar navbar-expand-lg custom-navbar fixed-top">
    <div class="container">

      <NuxtLink class="navbar-brand" to="/">
      </NuxtLink>

      <!-- HAMBURGER BOOTSTRAP -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- ISI NAVBAR -->
      <div
        class="collapse navbar-collapse"
        id="navbarSupportedContent"
      >

        <ul class="navbar-nav me-auto mb-2 mb-lg-0">

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/">
              Home
            </NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/aboutus">
              About Us
            </NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/services">
              Services
            </NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/doctors">
              Doctors
            </NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/news">
              News
            </NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink class="nav-link" to="/contact">
              Contact
            </NuxtLink>
          </li>

        </ul>

        <!-- BAGIAN KANAN -->
        <div class="d-flex align-items-center gap-4">

          <NuxtLink
            to="/search"
            class="search-icon"
          >
            <i class="bi bi-search"></i>
          </NuxtLink>

          <NuxtLink
            to="/bookandappoinment"
            class="btn appointment-btn px-4 rounded-pill"
          >
            Appointment
          </NuxtLink>

        </div>

      </div>
    </div>
  </nav>
</template>

<script setup>
import '~/assets/css/navbar.css'
</script>