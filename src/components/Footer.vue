<template>
    <div>
        <div class="row">
            <div class="col-12 col-lg-3 col-md-3 col-xl-3 col-sm-12 boldLinks">
                <p class="footerLink">Udemy for Business</p>
                <p class="footerLink">Teach on Udemy</p>
                <p class="footerLink">Udemy app</p>
            </div>
            <div class="col-12 col-lg-3 col-md-3 col-xl-3 col-sm-12 otherLinks">
                <p class="footerLink">About us</p>
                <p class="footerLink">Careers</p>
                <p class="footerLink">Blog</p>
            </div>
            <div class="col-12 col-lg-3 col-md-3 col-xl-3 col-sm-12 otherLinks">
                <p class="footerLink">Topics / Concepts</p> 
                <p class="footerLink">Support</p>
                <p class="footerLink">Affiliate</p>
            </div>
            <div class="col-12 col-lg-3 col-md-3 col-xl-3 col-sm-12 dropup">
                <b-dropdown id="dropdown-dropup" no-flip dropup text="☺ English" boundary="viewport" variant="outline-secondary" class="m-2 dropupItem">
                    <b-dropdown-item href="#">English</b-dropdown-item>
                    <b-dropdown-item href="#">Deutsch</b-dropdown-item>
                    <b-dropdown-item href="#">Español</b-dropdown-item>
                    <b-dropdown-item href="#">Français</b-dropdown-item>
                    <b-dropdown-item href="#">Bahasa Indonesia</b-dropdown-item>
                    <b-dropdown-item href="#">Italiano</b-dropdown-item>
                    <b-dropdown-item href="#">日本語</b-dropdown-item>
                    <b-dropdown-item href="#">한국어</b-dropdown-item>
                    <b-dropdown-item href="#">Nederlands</b-dropdown-item>
                    <b-dropdown-item href="#">Polski</b-dropdown-item>
                    <b-dropdown-item href="#">Português</b-dropdown-item>
                    <b-dropdown-item href="#">Română</b-dropdown-item>
                    <b-dropdown-item href="#">Русский</b-dropdown-item>
                    <b-dropdown-item href="#">ภาษาไทย</b-dropdown-item>
                    <b-dropdown-item href="#">Türkçe</b-dropdown-item>
                    <b-dropdown-item href="#">中文(简体)</b-dropdown-item>
                    <b-dropdown-item href="#">中文(繁體)</b-dropdown-item>
                </b-dropdown>
            </div>
        </div>
        <div class="localPages">
            <p>Local Home Pages:
                <span class="default">  English  </span>
                <span class="local">  Deutsch  </span>
                <span class="local">  Español  </span>
                <span class="local">  Français  </span>
                <span class="local">  Bahasa Indonesia  </span>
                <span class="local">  Italiano  </span>
                <span class="local">  日本語  </span>
                <span class="local">  한국어  </span>
                <span class="local">  Nederlands  </span>
                <span class="local">  Polski  </span>
                <span class="local">  Português  </span>
                <span class="local">  Română  </span>
                <span class="local">  Русский  </span>
                <span class="local">  ภาษาไทย  </span>
                <span class="local">  Türkçe  </span>
                <span class="local">  中文(简体)  </span>
                <span class="local">  中文(繁體)  </span>
            </p>
        </div>
        <div class="footerLogo">
            <img src="https://www.udemy.com/staticx/udemy/images/v6/logo-coral.svg" alt="logo-udemy">
            <span class="copyright">Copyright © 2019 Udemy, Inc.</span>
            <div class="links">
                <span>Terms</span>
                <span>Privacy Policy and Cookie Policy</span>
                <span>Topics / Concepts</span>
            </div>
        </div>
        <div class="line"></div>
    </div>
</template>

<style scoped>
    .dropup {
        text-align: right;
        padding-right: 40px;
    }

    p.footerLink {
        cursor: pointer;
        color: #138199;
        font-size: 14px;
        margin-bottom: 10px; 
    }

    p.footerLink:hover {
        color: #0f6174;
    }

    div.boldLinks p.footerLink:nth-child(1), div.boldLinks p.footerLink:nth-child(2) {
        font-weight: bold;
    }

    .boldLinks {
        padding-left: 40px;
    }

    .localPages p {
        color: #a1a7b3;
        font-weight: bold;
        font-size: 13px;
        margin-top: 37px;
    }

    .localPages {
        margin-left: 25px;
        margin-right: 50px;
    }

    .default {
        font-weight: 400;
        margin-left: 10px;
    }

    .localPages span {
        cursor: pointer;
        margin-right: 10px;
    }

    .localPages span:hover {
        color: #0f6174;
    }

    .localPages span:first-of-type:hover {
        cursor: text;
        color: #a1a7b3; 
    }

    .local {
        font-weight: 400;
        color: #138199;
    }

    .localPages span:last-of-type {
        margin: 0;
    }

    img {
        width: 110px;
        margin: 20px;
    }

    .footerLogo {
        border-top: 1px solid #e8e9eb;
        margin-top: 40px;
        padding-top: 10px;
    }

    .footerLogo span {
        font-size: 13px;
        opacity: .65;
    }

    .links {
        text-align: right;
        position: relative;
        bottom: 50px;
        font-size: 13px;
        color: #138199;
        padding-right: 40px;
    }

    .links span {
        margin: 0 7px;
    }

    .links span:hover {
        color: #0f6174;
        cursor: pointer;
    }

    .line {
        height: 6px;
        width: 100%;
        background-color: #ec5252;
    }

    @media (max-width: 768px) {
        .boldLinks, .otherLinks {
            display: none;
        }

        .dropup {
            text-align: left;
            padding-right: 40px;
            margin-left: 20px;
        }

        .links {
            text-align: left;
            padding-bottom: 20px;
            margin-left: 20px;
            bottom: 14px;
        }
    }

    @media (max-width: 576px) {
        .copyright {
            display: block;
            position: relative;
            margin-left: 20px;
            bottom: 10px;
            margin-bottom: 10px;
        }

        .links span {
            margin-right: 7px;
            margin-left: 0;
        }
    }
</style>

