<template>
    <div class="course">
        <div class="head">
            <div class="hot">Hot</div>
            <div class="text">新上好课</div>
        </div>
        <div class="items">
            <div class="item" v-for="i in 8">
                <el-image :src="imgSrc"></el-image>
                <div class="content">
                    <h4 class="head">Vue3项目实战</h4>
                    <div class="info">终极·99人报名</div>
                    <div class="price">¥ 99.99</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
let imgSrc = "https://oss.xuexiluxian.cn/xiaoluxian-vcr/cefb077be73d48028358f09b0459a779.png"
</script>

<style scoped lang="scss">
.course {
    width: 1080px;
    margin: 0 auto;

    .head {
        height: 26px;
        display: flex;
        line-height: 26px;

        .hot {
            background-color: hotpink;
            border-radius: 12px;
            padding: 0 12px;
            color: white;
        }

        .text {
            margin-left: 12px;
        }

        .text::after {
            content: '';
            display: inline-block;
            width: 76px;
            height: 10px;
            border-radius: 5px;
            background-color: rgba(orange, 0.3);
            z-index: -1;
            position: relative;
            top: 6px;
            left: -65px;
        }
    }

    .items {
        margin-top: 20px;
        margin-bottom: 50px;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        .item {
            width: 250px;
            margin-bottom: 16px;
        }
    }
}
</style>