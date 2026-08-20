<template>
    <div class="container">
        <div class="row g-3 appointment-cards">
            <div class="col-12 col-md-4">
                <div class="appointment-card card-one">
                    <span>Book an Appointment</span>
                    <i class="bi bi-calendar3"></i>
                </div>
            </div>
            <div class="col-12 col-md-4">
                <div class="appointment-card card-two">
                    <span class="span-card-2">Book an Appointment</span>
                    <i class="bi bi-people"></i>
                </div>
            </div>
            <div class="col-12 col-md-4">
                <div class="appointment-card card-three">
                    <span>Book an Appointment</span>
                    <i class="bi bi-cash-stack"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.appointment-cards{
    margin-top: -55px;
    position: relative;
    z-index: 10;
}

.appointment-card{
    height: 74px;
    padding: 0 18px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: white;
    border-radius: 3px;
}

.card-one{
    background-color: #1F2B6C;
}

.card-two{
    background-color: #BFD2F8;
    color: #1F2B6C;
}

.card-three{
    background-color: #159EEC;
}

.appointment-card span{
    font-size: 16px;
}

.appointment-card i{
    font-size: 30px;
}

.bi-calendar3{
    color: #BFD2F8;
}  

.bi-people{
    color: #1F2B6C;
}

.span-card-2{
    color: #1F2B6C;
}
</style>