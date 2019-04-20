<template>
    <div class="header">
        <div class="headerText col-lg-6 col-md-6 col-sm-6 col-12">
            <h1>Learn and save</h1>
            <p>Grow your expertise with courses from $20!</p>
            <b-input-group class="mt-3 inputGroup">
                <b-input-group-text class="inputSlot" slot="append"
                    ><font-awesome-icon class="search" icon="search"
                /></b-input-group-text>
                <b-form-input
                    value="What do you want to learn?"
                    class="inputForm"
                ></b-form-input>
            </b-input-group>
        </div>
    </div>
</template>

<style scoped>
.header {
    background: url('../assets/img/bg-lg.jpg');
    width: 100%;
    height: 500px;
    color: white;
}

.headerText {
    padding-top: 15%;
    padding-left: 60px;
}

h1 {
    font-size: 48px;
}

p {
    font-size: 20px;
}

.search {
    cursor: poiner;
    color: #ec5252;
    width: 20px;
    height: 50px;
}
.search:hover {
    color: white;
}

.inputSlot:hover {
    background-color: #ec5252;
    border: none !important;
    border-radius: 0%;
}

.inputGroup {
    width: 450px !important;
    height: 50px;
    cursor: pointer;
    background-color: white;
}

.inputSlot {
    background-color: white;
    padding: 0 20px;
    border: none !important;
    transition: 0.2s;
}

.inputForm {
    height: 50px;
    border: none !important;
    font-size: 20px;
    opacity: 0.6;
}
</style>
