<template>
    <header class="header">
        <div class="header__container _container">
            <div class="header__body flex items-center min-h-[105px]">

                <div class="flex w-full max-w-[500px] logoW"><img src="~/assets/img/logo.png" alt="logo" class="logo"></div>

                <MenuFlowbite class="flex justify-start w-full max-w-[711px]"></MenuFlowbite>

                <ButtonBorderWhite>Позвонить нам</ButtonBorderWhite>
            </div>
        </div>
    </header>
</template>


<!-- component script -->


<!-- component style -->
<style lang="scss">
/* ----------------reset css--------------------- */
/* * {
    outline: 1px solid tomato;
} */
@charset "UTF-8";

@font-face {
    font-family: 'MontserratMedium';
    /* no ~ before assets! */
    src: url('assets/fonts/Montserrat-Medium.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: "MontserratSemiBold";
    src: url("assets/fonts/Montserrat-SemiBold.ttf") format("truetype");
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: "MontserratBold";
    src: url("assets/fonts/Montserrat-Bold.ttf") format("truetype");
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

*,
*::before,
*::after {
    padding: 0;
    margin: 0;
    border: 0;
    box-sizing: border-box;
}

a {
    text-decoration: none;
}

ul,
ol,
li {
    list-style: none;
}

img {
    vertical-align: top;
}

h1,
h2,
h3,
h4,
h5,
h6 {
    font-weight: inherit;
    font-size: inherit;
}

h1 {
    font-size: 32px;
    line-height: 1.5;
}

html,
body {
    height: 100%;
    font-family: 'MontserratMedium';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    color: #FFFFFF;
}

/* -----------------reset css------------------- */
/* --------------------------------------------- */
.wrapper {
    min-height: 100%;
    overflow: hidden;
    display: flex;
    flex-direction: column;
}

._container {
    max-width: 1422px;
    margin: 0 auto;
    padding: 0 15px;
    box-sizing: content-box;
}

/* --------------------------------------------- */
</style>
<style lang="scss">
.header {
    background: linear-gradient(108.17deg, #3A97D1 0.88%, #01558B 100%);
}

p {
    -webkit-font-smoothing: auto;
    -moz-osx-font-smoothing: auto;
}
</style>