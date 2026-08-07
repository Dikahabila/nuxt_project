<template>
    <section class="hero-isi-artikel">
  <div class="container">
    <div class="row align-items-center">

      <!-- Teks -->
       <div class="row align-items-center" style="min-height: 100vh;">
      <div class="col-lg-6">
<h2 class="display-5 fw-bold hero-isi-artikel-title">
  A passion for putting patients first. 
</h2>   
 <div class="d-flex align-items-center flex-wrap gap-3">
 <div class="article-info">


              <small>
                <i class="bi bi-calendar3 me-1"></i>
                Monday 05, September 2021
              </small>

              <small>
                <i class="bi bi-person me-1"></i>
                By Author
              </small>

              <small>
                <i class="bi bi-eye me-1"></i>
                68
              </small>

              <small class="text-danger">
                <i class="bi bi-heart me-1"></i>
                86
              </small>

            </div>
            </div>
            
      </div>
      </div>

      <!-- Gambar -->
      

    </div>
    </div>
  </section>
</template>
<style>
.hero-isi-artikel {
    width: 100%;
    height: 300px;
    background: url("~/assets/svg/rectangle-3-6.svg") no-repeat center center;
    background-size: cover;
    position: relative;

    display: flex;
    align-items: center;
    overflow: hidden;
}

.hero-isi-artikel::before {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(255, 255, 255, 0.6); /* ubah angka 0.6 sesuai kebutuhan */
    z-index: 1;
}

.hero-isi-artikel-title {
    font-family: "Yesefa One", serif;
    color: #1F2B6C;
    font-size: 38px;
    position: relative;
    z-index: 2;
}</style>