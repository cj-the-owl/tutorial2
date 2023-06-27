<template>
    <nav class="topnav">
        <router-link class="active" to="/">Home</router-link>
        <router-link to="/tutorials">Tutorials</router-link>
        <router-link to="/about">About</router-link>
    </nav>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    .topnav {
        background-color: #333;
        overflow: hidden;
    }

    routerlink {
        float: left;
        color: #f2f2f2;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        font-size: 17px;
    }
</style>