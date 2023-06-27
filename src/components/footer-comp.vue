<template>
    <div class="footer">
        <h6>Footer</h6>
        <p class="footer-text-left">
            <routerlink class="menu" to="/">Home</routerlink>
            <routerlink class="menu" to="/">Tutorials</routerlink>
            <routerlink class="menu" to="/">About</routerlink>
        </p>
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    .footer {
        position: fixed;
        bottom: 0;
        left: 0;
        height: 90;
        background-color: chocolate;
    }

    .footer-text-left {
        font-size: 25px;
        padding-left: 40px;
        float: left;
        word-spacing: 20px;
    }

    .menu:hover {
        background-color: yellowgreen;
        font-size: 20px;
    }
</style>