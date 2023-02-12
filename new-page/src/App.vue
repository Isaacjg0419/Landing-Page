<template>
    <div id="app">
        <div>
           <!--  <div class="row">
                <div class="col">
                    <div class="row">
                        <div class="col-auto text-start">
                            <router-link to="/">Home</router-link>
                            <a href="https://themeforest.net/item/izpay-mobile-app-fintech-startup-elementor-template-kit/30074905"> Envato Market </a>
                        </div>
                        <div class="col text-end">
                            Buy Now
                        </div>
                    </div>
                </div>
            </div> -->
            <!-- <router-link to="/about">About</router-link> -->
        </div>
        <router-view />
    </div>
</template>
<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: start;

    color: #2c3e50;
}

nav {
    padding: 30px;
}

nav a {
    font-weight: bold;
    color: #2c3e50;
}

nav a.router-link-exact-active {
    color: #42b983;
}
</style>