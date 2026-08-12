<template>
  <div class="container py-5">
    <div class="row justify-content-center">
       <div class="mb-4 ms-lg-5">
    <h6 class="text-primary fw-bold">GET IN TOUCH</h6>
            <h1 class="title">Contact</h1> 
</div>
         <div class="col-xl-10">
      <div class="row g-4">


      <!-- Contact Form -->
      <div class="col-lg-7">
        <div class="appointment-form">
          <div class="row g-0">

            <div class="col-md-6">
              <input type="text" class="form-control" placeholder="Name">
            </div>

            <div class="col-md-6">
              <input type="email" class="form-control" placeholder="Email">
            </div>

            <div class="col-12">
              <input type="text" class="form-control" placeholder="Subject">
            </div>

            <div class="col-12">
              <textarea class="form-control" rows="8" placeholder="Message"></textarea>
            </div>

            <div class="col-12">
              <button class="submit-btn w-100">
                SUBMIT
              </button>
            </div>

          </div>
        </div>
      </div>

      <!-- Contact Cards -->
     <div class="col-lg-5">
  <div class="row g-3">

    <!-- Emergency -->
    <div class="col-12 col-sm-6">
      <div class="card h-100">
        <div class="card-body contact-card-body">
          <div class="pt-4">
            <i class="bi bi-telephone fs-2"></i>
          </div>

          <h5 class="card-title-contact fw-bold">
            EMERGENCY
          </h5>

          <p class="card-subtitle mb-2 contact-subtitle">
            (237) 681-812-255
          </p>

          <p class="card-subtitle contact-subtitle">
            (237) 666-331-894
          </p>
        </div>
      </div>
    </div>

    <!-- Location -->
    <div class="col-12 col-sm-6">
      <div class="card h-100">
        <div class="card-body contact-card-loc">
          <div class="pt-4">
            <i class="bi bi-geo-alt fs-2"></i>
          </div>

          <h5 class="card-title-location fw-bold location-title">
            LOCATION
          </h5>

          <p class="card-subtitle mb-2 location-subtitle">
            0123 Some place
          </p>

          <p class="card-subtitle location-subtitle">
            9876 Some country
          </p>
        </div>
      </div>
    </div>

    <!-- Email -->
    <div class="col-12 col-sm-6">
      <div class="card h-100">
        <div class="card-body contact-card-body">
          <div class="pt-4">
            <i class="bi bi-envelope fs-2"></i>
          </div>

          <h5 class="card-title fw-bold">
            EMAIL
          </h5>

          <p class="card-subtitle mb-2 email-subtitle">
            fildinese@gmail.com
          </p>

          <p class="card-subtitle email-subtitle">
            myebstudios@gmail.com
          </p>
        </div>
      </div>
    </div>

    <!-- Working Hours -->
    <div class="col-12 col-sm-6">
      <div class="card h-100">
        <div class="card-body contact-card-body">
          <div class="pt-4">
            <i class="bi bi-clock fs-2"></i>
          </div>

          <h5 class="card-title fw-bold">
            WORKING HOURS
          </h5>

          <p class="card-subtitle mb-2 working-subtitle">
            Mon-Sat 09:00-20:00
          </p>

          <p class="card-subtitle working-subtitle">
            Sunday Emergency only
          </p>
        </div>
      </div>
    </div>

  </div>
</div>
</div>
</div>
</div>
</div>
</template>

<script setup>
import '~/assets/css/contact.css'
</script>
