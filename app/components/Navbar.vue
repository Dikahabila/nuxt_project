<template>
  <nav class="navbar navbar-expand-lg custom-navbar fixed-top">
    <div class="container">

      <NuxtLink class="navbar-brand" to="/">
      </NuxtLink>

      <!-- HAMBURGER DESKTOP (JANGAN DIUBAH) -->
      <!-- Tombol toggler lama untuk collapse desktop TIDAK dipakai lagi di mobile,
           karena diganti tombol offcanvas di bawah. Dihapus supaya tidak dobel. -->

      <!-- ISI NAVBAR DESKTOP (>=992px) -->
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

        <!-- BAGIAN KANAN (DESKTOP) -->
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

      <!-- HAMBURGER MOBILE/TABLET (< 992px) -> BUKA OFFCANVAS -->
      <button
        class="navbar-toggler d-lg-none order-lg-last"
        type="button"
        data-bs-toggle="offcanvas"
        data-bs-target="#mobileSidebar"
        aria-controls="mobileSidebar"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

    </div>
  </nav>

 <!-- OFFCANVAS SIDEBAR MOBILE/TABLET -->
<div
  class="offcanvas offcanvas-end mobile-sidebar"
  tabindex="-1"
  id="mobileSidebar"
  aria-labelledby="mobileSidebarLabel"
>
  <div class="offcanvas-header">
    <span id="mobileSidebarLabel" class="fw-bold">
      Menu
    </span>

    <button
      type="button"
      class="btn-close-custom"
      data-bs-dismiss="offcanvas"
      aria-label="Close"
    >
      <i class="bi bi-x-lg"></i>
    </button>
  </div>

  <div class="offcanvas-body">
    <ul class="sidebar-nav">

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/"
        >
          Home
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/aboutus"
        >
          About Us
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/services"
        >
          Services
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/doctors"
        >
          Doctors
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/news"
        >
          News
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/contact"
        >
          Contact
        </NuxtLink>
      </li>

      <li>
        <NuxtLink
          class="sidebar-link"
          to="/search"
        >
          <i class="bi bi-search me-2"></i>
          Search
        </NuxtLink>
      </li>

      <li class="mt-3">
        <NuxtLink
          class="btn appointment-btn w-100 rounded-pill sidebar-appointment-btn"
          to="/bookandappoinment"
        >
          Appointment
        </NuxtLink>
      </li>

    </ul>
  </div>
</div>
</template>

<script setup>
import '~/assets/css/navbar.css'
</script>