<template>
    <div class="navigation">
       <img class="logo" src="https://www.udemy.com/staticx/udemy/images/v6/logo-coral.svg"/>
       <span class="categories">Categories</span>
        <b-input-group class="mt-3 inputGroup">
            <b-input-group-text class="inputSlot" slot="append"><font-awesome-icon class="search" icon="search" /></b-input-group-text>
            <b-form-input value="Search for anything" class="inputForm"></b-form-input>
        </b-input-group>
    </div>
</template>


<style scoped>
    .navigation {
        height: 64px;
    }

    .logo {
        width: 125px;
        padding-top: 18px;
        padding-left: 20px;
    }

    .categories {
        margin-left: 60px;
        position: relative;
        top: 10px;
        opacity: .8;
        cursor: pointer;
    }

    .inputGroup {
        width: 400px;
        display: inline-flex;
        position: absolute;
        margin-left: 40px;
        height: 40px;
        border: none !important;
        border-radius: 0 !important;

    }

    .search {
        cursor: poiner;
        color: #ec5252;
        width: 20px;
        height: 14px;
        border: none !important;
        border-radius: 10px !important;
        
    }

    .search:hover {
        color: white;
    }

    .inputForm {
        border: none !important;
        opacity: .8;
        border-radius: 0;
        height: 40px;
        background-color: #f2f3f5;


    }

    /* fix it */
    .inputSlot {
        background-color: #f2f3f5;
        padding: 0 20px;
        border: none !important;
        transition: .2s;
        cursor: pointer;

    }

    .inputSlot:hover {
        background-color: #ec5252;
        border: none !important;
        border-radius: 5px;
    }
</style>

