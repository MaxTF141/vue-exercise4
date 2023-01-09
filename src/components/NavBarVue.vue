<template>
    <nav class="navbar navbar-expand-lg bg-dark">
        <div class="container-fluid d-flex justify-content-between">
            <a class="navbar-brand" href="#">Navbar</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup"
                aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-center" id="navbarNavAltMarkup">
                <div class="navbar-nav gap-4">
                    <router-link class="text-decoration-none nav_items" to="/">HOME</router-link>
                    <router-link class="text-decoration-none nav_items" to="/products">PRODUCTS</router-link>
                    <router-link class="text-decoration-none nav_items" to="/admin">ADMIN</router-link>
                    <router-link class="text-decoration-none nav_items" to="/login">LOGIN</router-link>
                    <router-link class="text-decoration-none nav_items" to="/about">ABOUT</router-link>
                </div>
            </div>
        </div>
    </nav>

</template>
<script>
export default {

}
</script>
<style>
    .navbar-nav {
        font-family:Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    }
    .nav_items {
        color: grey;
        word-spacing: 5px   ;
    }
</style>