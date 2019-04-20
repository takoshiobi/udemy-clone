<template>
    <div class="reviews">
        <div class="container">
            <h3>What our students have to say</h3>
            <div class="row">
                <div class="col-12 col-md-4 col-sm-12 col-xl-4 col-lg-4 item">
                    <div class="reviewsItem">
                        <div class="circle"></div>
                        <div class="name">Borivoje</div>
                        <p>Udemy is a life saver. I don't have the time or money for a college education. My goal is to become a freelance web developer, and thanks to Udemy, I'm really close.</p>
                    </div>
                </div>
                <div class="col-12 col-md-4 col-sm-12 col-xl-4 col-lg-4 item">
                    <div class="reviewsItem">
                        <div class="circle"></div>
                        <div class="name">Borivoje</div>
                        <p>Udemy is a life saver. I don't have the time or money for a college education. My goal is to become a freelance web developer, and thanks to Udemy, I'm really close.</p>
                    </div>
                </div>
                <div class="col-12 col-md-4 col-sm-12 col-xl-4 col-lg-4 item">
                    <div class="reviewsItem">
                        <div class="circle"></div>
                        <div class="name">Borivoje</div>
                        <p>Udemy is a life saver. I don't have the time or money for a college education. My goal is to become a freelance web developer, and thanks to Udemy, I'm really close.</p>
                    </div>
                </div>
            </div>
            <div class="companies">
                Trusted by companies of all sizes
            </div>
            <div class="logos">
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/booking.svg" alt="booking">
                </span>
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/volkswagen.svg" alt="vw">
                </span>
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/mercedes.svg" alt="mercedes">
                </span>
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/pinterest.svg" alt="pinterest">
                </span>
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/adidas.svg" alt="adidas">
                </span>
                <span class="companyLogo">
                    <img src="https://i.udemycdn.com/partner-logos/paypal.svg" alt="paypal">
                </span>
            </div>
        </div>
    </div>
</template>


<style scoped>
    .reviews {
        background-color: #f7f8fa;
    }

    .reviewsItem {
        box-shadow: 0 2px 2px #e0e1e4;
        padding: 30px 0;
        background-color:white;
        margin: 20px 1px;
    }

    h3 {
        padding-top: 20px;
        color: #29303b;
    }

    .circle {
        background: grey;
        width: 70px;
        height: 70px;
        border-radius: 50%;
        display: inline-block;
        margin-left: 25px;
    }

    .name {
        display: inline-block;
        position: relative;
        bottom: 25px;
        padding-left: 20px;
        font-size: 17px;
        font-weight:500;
    }

    p {
        font-size: 17px;
        margin: 0 30px;
        padding-top: 10px;
        opacity: .9;
    }

    .item {
        padding: 0 5px;
    }

    .companies {
        text-align: center;
        margin-top: 20px;
        opacity: .6;
    }

    .companyLogo {
        margin: 30px;
    }

    .logos {
        display: table;
        margin: 0 auto;
        padding-top: 40px;
    }
</style>

