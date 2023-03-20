<template>
    <div class="authorInfo-container">
        <div class="bk-container"></div>
        <div class="block">
            <div class="avatar">
                <img src="./../../assets/static/default_avatar.jpg" alt="">
            </div>
            <div class="author">
                <span>Agoni</span>
            </div>
            <div class="line"></div>
            <div class="desc">
                <span>一个疯狂的coder</span>
            </div>
        </div>
        <div class="links">
            <ul class="list">
                <a class="item" target="_blank" href="https://github.com/liyunlong6">
                    <img src="../../assets/static/3.png" alt="">
                </a>
                <a class="item" target="_blank" href="https://github.com/liyunlong6">
                    <img src="../../assets/static/3.png" alt="">
                </a>
            </ul>
        </div>
        <div class="footer">
            <div class="articles item">
                <div class="text">Articles</div>
                <div class="count">15</div>
            </div>
            <div class="tags item ">
                <div class="text">Tags</div>
                <div class="count">4</div>
            </div>
            <div class="articles item">
                <div class="text">Talks</div>
                <div class="count">15</div>
            </div>
            <div class="tags item ">
                <div class="text">Categories</div>
                <div class="count">4</div>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="less" scoped>
.authorInfo-container {
    width: 100%;
    min-width: 320px;
    height: 400px;
    margin-top: 47px;
    background: linear-gradient(220.55deg, #DEB5FF 0%, #6F00B3 100%);
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    position: relative;

    .bk-container {
        position: absolute;
        top: 40px;
        left: 4px;
        border-radius: 15px;
        border: 1px solid black;
        background: #1a1a1a;
        opacity: 0.9;
        height: 350px;
        width: 310px;
    }

    .block {
        z-index: 5;
        width: 300px;
        height: 240px;
        margin: 0 auto;
        margin-top: 15px;
        opacity: 1;
        text-align: center;


        .avatar {
            margin: 0 auto;
            width: 100px;
            height: 100px;
            border-radius: 50%;

            img {
                width: 90px;
                height: 90px;
                border-radius: 50%;
            }
        }

        .author {
            font-size: 30px;
            color: #fff;
        }

        .line {
            margin: 0 auto;
            margin-top: 10px;
            width: 80px;
            height: 3px;
            border-radius: 3px;
            background-image: linear-gradient(135deg, #F6CEEC 10%, #D939CD 100%);
        }

        .desc {
            margin-top: 25px;
            color: #ccc;
        }
    }

    .links {
        height: 50px;
        margin: 0 auto;

        .list {
            height: 100%;
            display: flex;
            text-align: center;
            z-index: 5;

            .item {
                width: 31px;
                height: 31px;
                z-index: 2;
                margin-left: 20px;
                background-color: #fff;
                border-radius: 50%;

                img {
                    height: 108%;
                    width: 108%;
                    border-radius: 50%;
                }
            }
        }
    }

    .footer {
        bottom: 20px;
        color: white;
        height: 40px;
        display: flex;
        z-index: 5;
        justify-content: space-around;
        margin: 0 auto;
        margin-top: 15px;

        .item {
            text-align: center;
            min-width: 60px;

        }
    }
}
</style>