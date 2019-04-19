<template>
    <div>
        <div class="lineGrad"></div>
        <div class="recContent">
            <h1>Get personalized recommendations</h1>
            <p>Answer a few questions for your top picks</p>
            <button>Get started</button>
        </div>
    </div>
</template>

<style scoped>
    .lineGrad {
        margin-top: 40px;
        height: 7px;
        background: rgb(111,27,82);
        background: linear-gradient(90deg, rgba(111,27,82,1) 0%, rgba(230,80,82,1) 100%);
    }
    .recContent {
        background: #29303b;
        height: 300px;
    }

    h1, p {
        text-align: center;
        color: white;
    }

    h1 {
        font-size: 24px;
        padding-top: 100px;
    }

    p {
        font-size: 16px;
    }

    button {
        display: table;
        margin: 0 auto;
        color: white;
        background: #ec5252;
        font-weight: bold;
        font-size: 14px;
        padding: 7px;
        border-radius: 5px;
        transition: .2s;
    }

    button:hover {
        background-color: #ad3652;
    }
</style>
