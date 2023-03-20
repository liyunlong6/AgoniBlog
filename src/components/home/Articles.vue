<template>
    <div class="articles-container">

        <div class="text-articles">
            <p>ARTICLES</p>
            <div class="line"></div>
        </div>

        <div class="articles">
            <div class="article-item" v-for="article in articles" :key="article">
                <img :src="article.img" alt="">
                <div class="tags">
                    <span v-for="tag in article.tags" :key="tag">
                        # {{ tag }}
                    </span>
                </div>
                <div class="title">
                    {{ article.title }}
                </div>
                <div class="desc">
                    {{ article.desc }}
                </div>
                <div class="author">
                    {{ article.author }}
                </div>
                <div class="time">
                    <span>share on {{ article.time }}</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const articles = ref([
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
    {
        img: "./../../src/assets/static/1.jpg",
        tags: ref(["spring", "springboot"]),
        title: "docker入门",
        desc: "1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是",
        author: "Agoni",
        time: "2023.03.12"
    },
])

</script>

<style lang="less" scoped>
.articles-container {
    height: 500px;
    width: 100%;

    .text-articles {
        color: white;
        font-size: 30px;
        margin-left: 30px;

        p {
            padding: 0;
            margin: 0;
        }

        .line {
            width: 130px;
            // border: 5px solid black;
            height: 3px;
            background-image: linear-gradient(135deg, #F6CEEC 10%, #D939CD 100%);
            margin-left: 5px;
        }
    }

    .articles {
        display: flex;
        flex-wrap: wrap;
        margin-top: 25px;

        .article-item {
            width: 30%;
            min-width: 350px;
            height: 380px;
            border: 1px solid black;
            margin-right: 3%;
            margin-bottom: 20px;
            border-radius: 15px;
            overflow: hidden;
            position: relative;
            background: #212121;
            transition: all 0.3s;

            img {
                width: 100%;
                border-radius: 15px;

            }

            .tags {
                position: absolute;
                top: 160px;
                left: 15px;
                z-index: 2;
                color: rgb(190, 190, 190);
            }

            .title {
                color: white;
                font-size: 28px;
                margin-left: 10%;
                margin-top: 15px;
            }

            .desc {
                margin-top: 15px;
                width: 90%;
                height: 65px;
                margin-left: 5%;
                // font-size: 18px;
                display: -webkit-box;
                -webkit-box-orient: vertical;
                -webkit-line-clamp: 3;
                overflow: hidden;
                color: rgb(190, 190, 190);
            }

            .author {
                position: absolute;
                bottom: 25px;
                left: 20px;
                color: white;
            }

            .time {
                position: absolute;
                bottom: 25px;
                left: 80px;
                color: rgb(190, 190, 190);
            }

        }

        .article-item:hover{
            transform: scale(1.02);
        }
    }
}
</style> 