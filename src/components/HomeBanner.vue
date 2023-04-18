<template>
    <div class="main-banner">
        <h1>Make Your Burguer</h1>
    </div>
</template>

<script>
    export default{
        name: 'HomeBanner'
    }
</script>

<style scoped>
    .main-banner{
        background-image: url('/img/burger.jpg');
        background-size: cover;
        background-position: -300px;
        height: 70vh;
        max-height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    h1{
        color: #fff;
        text-align: center;
        font-size: 60px;
        background-color: #222;
        padding: 20px 40px;
        font-weight: bold;
    }

</style>