<template>
    <div class="home-container">
        <Header class="header-container" />
        <div class="block">
            <TopArticle class="topArticle-container" />
            <div class="main">
                <div class="left-container">
                    <Articles class="articles-container" />
                </div>
                
                <div class="right-container">
                    <AuthorInfo />
                    <Tags />
                </div>
            </div>

        </div>
    </div>
</template>

<script setup>
import Header from '../components/home/Header.vue';
import TopArticle from '../components/home/TopArticle.vue';
import Articles from '../components/home/Articles.vue';
import Tags from '../components/home/Tags.vue';
import AuthorInfo from '../components/home/AuthorInfo.vue';


</script>

<style lang="less" scoped>
.home-container {

    .header-container {
        margin: 40px auto;
        color: aqua;
        margin-bottom: 60px;
    }

    .block {
        width: 80%;
        height: auto;
        margin: 0 auto;
        display: flex;
        flex-direction: column;

        .topArticle-container {
            border-radius: 20px;
            width: 100%;
            height: 400px;
            margin-bottom: 60px;
        }

        .main {
            width: 100%;
            display: flex;
            justify-content: space-around;
            .left-container{
                width: 78%;
                height: auto;

            }

            .right-container{
                width: 320px;
                height: auto;
                margin-top: 20px;

            }
        }

    }


}
</style>