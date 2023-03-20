<template>
    <div class="header-container">
        <div class="logo"></div>
        <div class="nav-container">
            <ul class="nav">
                <li class="home nav-item"><a href="/home">HOME</a></li>
                <li class="about nav-item"><a href="/about">ABOUT</a></li>
                <li class="tags nav-item"><a href="/tags">TAGS</a></li>
            </ul>
        </div>
        <div class="setting"></div>
    </div>
</template>

<script setup>

</script>

<style lang="less" scoped>
.header-container {
    width: 1000px;
    height: 50px;
    border: 1px solid black;
    display: flex;
    position: relative;

    .nav-container {
        margin: 0;
        position: absolute;
        top: -3px;
        left: 20px;

        .nav {
            display: flex;
            list-style: none;

            .nav-item {
                width: 70px;
                text-align: center;
                font-size: 18px;
                margin: 0 5px;
            }

            .nav-item:hover {
                cursor: pointer;
            }
        }
    }
}
</style>
