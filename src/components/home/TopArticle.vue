<template>
    <div class="topArticle">
        <div class="img">
            <img src="./../../assets/static/1.jpg" alt="">
        </div>
        <div class="content">
            <div class="tags">
                <div class="tag-item" v-for="tag in tags" :key="tag">
                    <span># {{ tag }}</span>
                </div>
            </div>
            <div class="title">
                <span>{{ title }}</span>
            </div>
            <div class="desc">
                {{ desc }}
            </div>
            <div class="author">{{ author }}</div>
            <div class="time">share on {{ time }}</div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';
const tags = ref(["spring", "springboot"]);
const title = ref("docker入门");
const desc = ref("1.docker概述1.1 基本介绍 Docker 是一个开源的应用容器引擎，基于 Go 语言 并遵从 Apache2.0 协议开源。 Docker 可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。 容器是完全使用沙箱机制，相互之间不会有任何接口,更重要的是");
const author = ref("Agoni");
const time = ref("2022.3.12");
</script>

<style lang="less" scoped>
.topArticle { 
    display: flex;
    border: 1px solid black;
    color: rgb(190, 190, 190);
    transition: all 0.3s;


    .img {
        height: 100%;
        width: 50%;
        overflow: hidden;
        // border-top-left-radius: 20px;
        //     border-bottom-left-radius: 20px;
        border-radius: 20px;

        img {
            // height: 100%;
            width: 100%;
            pointer-events: none;
            
        }
    }

    .content {
        height: 100%;
        width: 50%;
        position: relative;

        .tags {
            position: absolute;
            display: flex;
            top: 30px;

            .tag-item {
                margin-right: 18px;
                font-size: 18px;
            }
        }

        .title {
            position: absolute;
            top: 80px;
            font-size: 35px;
            color: white;
        }

        .desc {
            position: absolute;
            top: 160px;
            width: 100%;
            height: 90px;
            line-height: 30px;
            font-size: 20px;
            display: -webkit-box;
            -webkit-box-orient: vertical;
            -webkit-line-clamp: 3;
            overflow: hidden;
        }

        .author {
            position: absolute;
            bottom: 40px;
        }

        .time {
            position: absolute;
            bottom: 40px;
            left: 100px;
        }
    }
}
.topArticle:hover{
    transform: scale(1.02);
}
</style>