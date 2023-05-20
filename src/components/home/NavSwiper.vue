<template>
    <div class="nav-swiper">
        <div class="main">
            <div class="t">
                <div class="l">
                    <ul class="items">
                        <li class="item">HTML/CSS</li>
                        <li class="item">TypeScript</li>
                        <li class="item">ReactJS</li>
                        <li class="item">Javascript</li>
                        <li class="item">Vue</li>
                        <li class="item">Java</li>
                    </ul>
                </div>
                <div class="r">
                    <el-carousel height="370px">
                        <el-carousel-item v-for="item in 4" :key="item">

                        </el-carousel-item>
                    </el-carousel>
                </div>
            </div>
            <div class="b">
                <div class="item">
                    <el-icon :size="60" color="teal">
                        <Opportunity />
                    </el-icon>
                    <div class="content">
                        <h4>初级课程</h4>
                        <span>入门见效快</span>
                    </div>
                </div>
                <div class="item">
                    <el-icon :size="60" color="teal">
                        <Opportunity />
                    </el-icon>
                    <div class="content">
                        <h4>初级课程</h4>
                        <span>入门见效快</span>
                    </div>
                </div>
                <div class="item">
                    <el-icon :size="60" color="teal">
                        <Opportunity />
                    </el-icon>
                    <div class="content">
                        <h4>初级课程</h4>
                        <span>入门见效快</span>
                    </div>
                </div>
                <div class="item">
                    <el-icon :size="60" color="teal">
                        <Opportunity />
                    </el-icon>
                    <div class="content">
                        <h4>初级课程</h4>
                        <span>入门见效快</span>
                    </div>
                </div>
                <div class="item">
                    <el-icon :size="60" color="teal">
                        <Opportunity />
                    </el-icon>
                    <div class="content">
                        <h4>初级课程</h4>
                        <span>入门见效快</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { Opportunity } from '@element-plus/icons-vue'
</script>

<style scoped lang="scss">
.nav-swiper {
    width: 100%;
    height: 600px;
    padding: 50px 0;
    background-image: linear-gradient(to top, #fff 0%, #accbee 100%);

    .main {
        width: 1080px;
        height: 500px;
        margin: 0 auto;

        .t {
            display: flex;
            height: 370px;
            border-radius: 11px 11px 0 0;

            .l {
                padding: 35px 0;
                width: 220px;
                height: inherit;
                background-color: #211e2d;

                .items {
                    .item {
                        text-align: center;
                        line-height: 50px;
                        color: #ccc;
                        font-size: 18px;
                        height: 50px;
                        cursor: pointer;
                    }

                    .item:hover {
                        color: #211e2d;
                        background-image: linear-gradient(to left, #211e2d 0%,  #7b9abe 100%);
                    }
                }
            }

            .r {
                width: 860px;
                // height: inherit;
            }
        }

        .b {
            height: 130px;
            display: flex;
            justify-content: space-between;
            background-color: white;

            .item {
                width: 216px;
                display: flex;
                justify-content: center;
                margin: 35px 0;
                h4 {
                    font-weight: bold;
                }

                .content {
                    height: 60px;
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                }
            }
        }
    }
}
</style>