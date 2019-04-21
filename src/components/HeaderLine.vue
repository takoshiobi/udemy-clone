<template>
    <div class="headerLine row">
        <div class="item col-4 col-md-4 col-lg-4">
            <h3>100,000 online courses</h3>
            <p>Explore a variety of fresh topics</p>
        </div>
        <div class="item col-4 col-md-4 col-lg-4">
            <h3>Expert instruction</h3>
            <p>Find the right instructor for you</p>
        </div>
        <div class="item col-4 col-md-4 col-lg-4">
            <h3>Lifetime access</h3>
            <p>Learn on your schedule</p>
        </div>
    </div>
</template>

<style scoped>
h3 {
    font-size: 20px;
    font-weight: bold;
    margin-bottom: 0;
    padding-top: 20px;
    padding-left: 80px;
}

p {
    font-size: 16px;
    padding-left: 80px;
}

.headerLine {
    margin-bottom: 40px;
    color: white;
    background: rgb(111, 27, 82);
    background: linear-gradient(
        90deg,
        rgba(111, 27, 82, 1) 0%,
        rgba(230, 80, 82, 1) 100%
    );
}

@media (max-width: 768px) {
    .headerLine {
        display: none;
    }
}

@media (max-width: 992px) {
    .headerLine {
        text-align: center;
    }

    h3 {
        font-size: 16px;
        padding-top: 10px;
        padding-left: 40px;
    }

    p {
        font-size: 14px;
        padding-left: 40px;
    }
}
</style>
