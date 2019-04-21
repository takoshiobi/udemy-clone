<template>
    <div class="container categories">
        <h3>Top categories</h3>
        <div class="row">
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/coding.png" alt="" />
                    Development
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/analytics.png" alt="" />
                    Business
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/monitor.png" alt="" />
                    IT and Software
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/sketch.png" alt="" />
                    Design
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/seo.png" alt="" />
                    Marketing
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/open-book.png" alt="" />
                    Personal Development
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/camera.png" alt="" />
                    Photography
                </div>
            </div>
            <div class="col-md-6 col-lg-3 col-12 col-sm-12 col-xl-3">
                <div class="topItem">
                    <img src="../assets/icons/music.png" alt="" />
                    Music
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.topItem {
    border: 1px solid;
    padding: 20px 0;
    margin-top: 20px;
    font-size: 16px;
    border: 1px solid #e3e3e4;
    box-shadow: 0px 2px 4px #e3e3e4;
}

.topItem:hover {
    box-shadow: 4px 4px 10px #e3e3e4;
}

h3 {
    margin-top: 20px;
    color: #29303b;
}

.categories {
    padding-bottom: 40px;
}

.topItem img {
    width: 30px;
    margin-left: 20px;
    margin-right: 10px;
}
</style>
