<template>
    <div class="navigation">
        <img
            class="logo"
            src="https://www.udemy.com/staticx/udemy/images/v6/logo-coral.svg"
        />
        <span class="categories">Categories</span>
        <b-input-group class="mt-3 inputGroup">
            <b-input-group-text class="inputSlot" slot="append"
                ><font-awesome-icon class="search" icon="search"
            /></b-input-group-text>
            <b-form-input
                value="Search for anything"
                class="inputForm"
            ></b-form-input>
        </b-input-group>
        <span class="button-light">Udemy for Business</span>
        <span class="button-light">Teach of Udemy</span>
        <div class="buttonsGroup">
            <span class="login">Log In</span>
            <span class="signup">Sign Up</span>
        </div>
    </div>
</template>

<style scoped>
.navigation {
    height: 70px;
}

.logo {
    width: 125px;
    padding-top: 20px;
    padding-left: 20px;
}

.categories {
    margin-left: 60px;
    position: relative;
    top: 13px;
    opacity: 0.8;
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
    opacity: 0.8;
    border-radius: 0;
    height: 40px;
    background-color: #f2f3f5;
}

/* fix it */
.inputSlot {
    background-color: #f2f3f5;
    padding: 0 20px;
    border: none !important;
    transition: 0.2s;
    cursor: pointer;
}

.inputSlot:hover {
    background-color: #ec5252;
    border: none !important;
    border-radius: 5px;
}

.buttonsLight {
    position: absolute;
    right: 40px;
}

.button-light {
    position: relative;
    top: 13px;
    left: 490px;
    margin-left: 10px;
    font-size: 13px;
    opacity: 0.7;
    cursor: pointer;
    padding: 13px;
    border-radius: 3px;
    border: 1px solid white;
}

.button-light:hover {
    background-color: #f2f3f5;
    border: 1px solid #dfdfdf;
}

.buttonsGroup {
    position: absolute;
    right: 30px;
    top: 25px;
}

.buttonsGroup span {
    margin-left: 5px;
}

.signup {
    background-color: #ec5252;
    border: 1px solid #ec5252;
    color: white;
    padding: 10px;
    font-size: 16px;
    border-radius: 3px;
    transition: 0.1s;
    cursor: pointer;
}

.signup:hover {
    background-color: #c74444;
}

.login {
    border: 1px solid #686f7a;
    color: #686f7a;
    padding: 10px;
    font-size: 16px;
    border-radius: 3px;
    transition: 0.1s;
    cursor: pointer;
}

.login:hover {
    border: 1px solid #474c53;
    color: #484d55;
}

@media (max-width: 768px) {
    .login,
    .signup,
    .button-light,
    .inputGroup,
    .categories {
        display: none;
    }

    .logo {
        width: 100px;
        display: table;
        margin: 0 auto;
        padding-top: 13px;
        padding-left: 0;
    }

    .navigation {
        height: 50px;
    }
}
</style>
