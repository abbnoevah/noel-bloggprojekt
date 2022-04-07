<template>
<div>
    <NavBar class="h-0"/>
    <nuxt></nuxt>
</div>
</template>

<script>

import NavBar from "../components/NavBar.vue";

export default {
    data() {
        return {
            NavBar
        }
    }
}

</script>

<style>

html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

/* #pageContainer {
    background-color: rgb(60,65,75);
} */

/* #navigationBar {

    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
} */

/* #navigationBar2 {
    margin: auto;

    color: white;

    box-shadow: 0 0 24px rgba(0, 10, 20, 0.6);
} */

/* #home {
    height: 100%;
    width: 24%;

    display: flex;
    justify-content: center;
    align-items: center;
} */

/* #navigationBar2 :hover {
    background-color: rgba(255, 255, 255, 0.15);
    transition: 200ms;
} */

/* #about-me {
    height: 100%;
    width: 24%;

    display: flex;
    justify-content: center;
    align-items: center;
} */

/* #home :hover {
   background-color: rgba(255, 255, 255, 0.15);
    transition: 200ms;
} */

/* #about-me :hover {
    background-color: rgba(255, 255, 255, 0.15);
    transition: 200ms;
} */
</style>