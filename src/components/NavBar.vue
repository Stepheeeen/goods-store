<template>
    <div class="navbar">
        <h2>{{ navName }}</h2>

        <ul>
            <li>
                Home
            </li>
            <li>
                Sales
            </li>
            <li>
                Contact
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    props: {
        navName: String
    }
};
</script>

<style>
    .navbar{
        width: 100%;
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background: white;
        font-family: sans-serif;
        padding: 10px;
        height: 80px;
        z-index: 9000;
        box-shadow: 0 0 3px 0 #808080;
    }
    ul{
        display: flex;
        margin-right: 20px;
    }
    ul li{
        list-style: none;
        margin-right: 15px;
        font-size: 18px;
    }
    @media screen and (max-width: 500px) {
        ul{
        margin-right: 0;
    }
    }
</style>