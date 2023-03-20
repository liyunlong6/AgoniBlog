<template>
    <div class="tags-container">
        <div class="text-tags">
            <p>TAGS</p>
            <div class="line"></div>
        </div>
        <div class="tags">
            <div class="tag-item" v-for="tag in tags" :key="tag">
                <span class="name">&ensp;#{{ tag.name }}</span>
                <span class="count">&ensp;{{ tag.count }} </span>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const tags = ref([{ name: "spring", count: 1 }, { name: "springboot", count: 2 }, { name: "C++", count: 5 }, { name: "Java", count: 34 }])
</script>

<style lang="less" scoped>
.tags-container {
    width: 100%;
    border: 1px solid black;
    height: auto;
    border-radius: 15px;
    background: #212121;
    margin-top: 50px;

    .text-tags {
        color: white;
        font-size: 30px;
        margin-left: 30px;
        margin-top: 30px;

        p {
            padding: 0;
            margin: 0;
        }

        .line {
            width: 70px;
            height: 3px;
            background-image: linear-gradient(135deg, #F6CEEC 10%, #D939CD 100%);
            margin-left: 5px;
        }
    }

    .tags {
        margin-top: 30px;
        display: flex;
        flex-wrap: wrap;
        // justify-content: space-evenly;

        .tag-item {
            width: 46%;
            height: 20px;
            margin-bottom: 10px;
            margin-left: 10px;
            border-radius: 5px;
            height: 25px;
            color: rgb(190, 190, 190);
            display: flex;
            transition: all 0.3s;

            .name {
                display: flex;
                background: #141414;
                align-items: center;
                border-top: 1px solid black;
                border-left: 1px solid black;
                border-bottom: 1px solid black;
                border-top-left-radius: 10px;
                border-bottom-left-radius: 10px;
            }
            .count{
                display: flex;  
                width: 35px;
                color: #d31d8a;     
                background: #1C1C1C;           
                border-top: 1px solid black;
                border-right: 1px solid black;
                border-bottom: 1px solid black;
                border-top-right-radius: 10px;
                border-bottom-right-radius: 10px;
            }
        }

        .tag-item:hover{
            cursor: pointer;
            
            .name, .count{
                background: #212121;
            }
        }
    }
}
</style>