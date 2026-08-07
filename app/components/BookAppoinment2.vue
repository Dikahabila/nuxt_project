<template>
  <div class="container py-5">
    <div class="row g-4">

      <!-- Kiri : Form -->
      <div class="col-lg-6">

       <h5 class="card-title card-isi-news">Book And appointment</h5> 

        <p class="mb-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque placerat scelerisque tortor ornare ornare. Convallis felis vitae tortor augue. Velit nascetur proin massa in. Consequat faucibus porttitor enim et.
        </p>

        <div class="appointment-form">
          <div class="row g-0">

            <div class="col-6">
              <input type="text" class="form-control" placeholder="Name">
            </div>

            <div class="col-6">
              <select class="form-select">
                <option>Gender</option>
              </select>
            </div>

            <div class="col-6">
              <input type="email" class="form-control" placeholder="Email">
            </div>

            <div class="col-6">
              <input type="text" class="form-control" placeholder="Phone">
            </div>

            <div class="col-6">
              <input type="date" class="form-control">
            </div>

            <div class="col-6">
              <input type="time" class="form-control">
            </div>

            <div class="col-6">
              <select class="form-select">
                <option>Doctor</option>
              </select>
            </div>

            <div class="col-6">
              <select class="form-select">
                <option>Department</option>
              </select>
            </div>

            <div class="col-12">
              <textarea class="form-control" rows="5" placeholder="Message"></textarea>
            </div>

            <div class="col-12">
              <button class="submit-btn w-100">
                Submit
              </button>
            </div>

          </div>
        </div>

      </div>

      <!-- Kanan : Schedule Hours -->
      <div class="col-lg-6">

        <div class="schedule-card">
            <h2 class="schedule-title">Schedule Hours</h2>
            <div class="d-flex justify-content-between">
    <span class="schedule-span">Monday</span>
    <span class="schedule-line"></span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>
            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">Tuesday</span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>
            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">Wednesday</span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>
            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">Thursday</span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>
            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">friday</span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>
            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">Saturday</span>
    <span class="schedule-span">08:00 AM - 07:00 PM</span>
</div>

            <div class="d-flex justify-content-between mt-2">
    <span class="schedule-span">Sunday</span>
    <span class="schedule-span">Closed</span>
</div>
 <hr class="schedule-divider">

    <div class="emergency d-flex align-items-center mt-2">

      <i class="bi bi-telephone fs-1"></i>

      <div class="emergency text-center">
        <h5 class="mb-1">Emergency</h5>
        <p class="mb-0 fs-5 fw-bold">(237) 681-812-255</p>
      </div>

</div>
</div>
</div>
</div>
</div>
</template>
<script setup>
import '~/assets/css/book.css'
</script> 

<style>
/* Card */
.schedule-card{
    background-color: #1F2B6C;
    border-radius: 8px;
    padding: 20px 30px 5px 30px;
    height: 100%;
}

/* Judul */
.schedule-title{
    color: #9DB9F6;
    font-family: "Yesefa One", serif;
    text-align: center;
    font-size: 48px;
    margin-bottom: 30px;
}
.schedule-span{
    color: white;
}

/* Setiap baris jadwal */
.schedule-item{
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #fff;
    font-size: 16px;
    margin-bottom: 18px;
}

/* Garis pemisah */
.schedule-divider{
    width: 80%;
    border: none;
    border-top: 2px solid #9DB9F6;
    margin: 30px auto;
}

/* Bagian emergency */
.emergency{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    gap: 8px;
}

/* Icon telepon */
.emergency i{
    color: #9DB9F6;
    font-size: 32px;
}

/* Judul Emergency */
.emergency h5{
    color: white;
    margin-bottom: 5px;
    font-size: 20px;
    
}


/* Nomor telepon */
.emergency p{
    color: #9DB9F6;
    margin: 0;
    font-size: 38px;
}


</style>