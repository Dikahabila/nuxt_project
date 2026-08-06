<template>
    <section class="hero-contact">
  <div class="container">
    <div class="row align-items-center">

      <!-- Teks -->
       <div class="row align-items-center" style="min-height: 100vh;">
      <div class="col-lg-6">
<h1 class="display-5 fw-bold hero-title">
   Our Contact
</h1>   
            
      </div>
      </div>

      <!-- Gambar -->
      

    </div>
    </div>
  </section>
</template>
<style>
.hero-contact {
    width: 100%;
    height: 250px;
    background: url("~/assets/svg/Rectangle 3 (3).svg") no-repeat center center;
    background-size: cover;
    position: relative;

    display: flex;
    align-items: center;
    overflow: hidden;
}

.hero-contact::before {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(255, 255, 255, 0.6); /* ubah angka 0.6 sesuai kebutuhan */
    z-index: 1;
}

.hero-title {
    font-family: "Yesefa One", serif;
    color: #1F2B6C;
    font-size: 48px;
    position: relative;
    z-index: 2;
}
</style>