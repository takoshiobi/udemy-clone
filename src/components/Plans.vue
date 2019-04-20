<template>
    <div class="plans container-fluid">
        <div class="row">
            <div class="col-md-6 col-12 col-sm-12 col-lg-6 col-xl-6 planItem">
                <h4>Teach on Udemy</h4>
                <p>
                    Teach what you love. Udemy gives you the tools to create an
                    online course.
                </p>
                <button>Start teaching</button>
            </div>
            <div class="col-md-6 col-12 col-sm-12 col-lg-6 col-xl-6 planItem">
                <h4>Udemy for Business</h4>
                <p>
                    Get unlimited access to 3,000+ of Udemy’s top courses for
                    your team.
                </p>
                <button>Get Udemy for Business</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
.planItem {
    text-align: center;
    padding: 40px 0;
}

h4 {
    opacity: 0.7;
}

.plans {
    background-color: #f7f8fa;
    padding-bottom: 20px;
    border-bottom: 1px solid #dedfe0;
    margin-bottom: 40px;
}

p {
    font-size: 16.6px;
    margin: 0 150px;
    padding: 10px 0;
}

.planItem:nth-of-type(2) {
    border-left: 1px solid #dedfe0;
}

button {
    display: table;
    margin: 10px auto;
    color: white;
    background: #ec5252;
    font-weight: bold;
    font-size: 14px;
    padding: 10px;
    border-radius: 2px;
    transition: 0.1s;
}

button:hover {
    background-color: #ad3652;
}
</style>
