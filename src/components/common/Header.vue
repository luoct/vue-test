<template>
    <header>
        <div class="main">
            <div class="header-l">
                <img src="@/assets/logo.svg" height="50">
                <ul>
                    <li class="active">首 页</li>
                    <li>课 程</li>
                    <li>会 员</li>
                </ul>
            </div>
            <div class="header-r">
                <div class="search">
                    <input>
                    <el-icon :size="20">
                        <Search />
                    </el-icon>
                </div>
                <div class="shop">
                    <el-icon :size="24">
                        <ShoppingCart />
                    </el-icon>
                </div>

                <div class="login">
                    登陆/注册
                </div>
            </div>
        </div>
    </header>
</template>

<script setup lang="ts">
import { Search, ShoppingCart } from '@element-plus/icons-vue'
</script>

<style scoped lang="scss">
header {
    width: 100%;
    height: 80px;

    .main {
        width: 1080px;
        height: 80px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .header-l {
            display: flex;
            .active {
                position: relative;
                color: #3585ff;
            }
            .active::after {
                content: '';
                position: absolute;
                width: 50px;
                height: 2px;
                bottom: -10px;
                left: 0px;
                background-color: #3585ff;
            }
            ul {
                margin: 0 50px;
                width: 200px;
                display: flex;
                justify-content: space-between;
                align-items: center;
                
                li {
                    width: 50px;
                    text-align: center;
                    font-size: 16px;
                    font-weight: bold;
                    color: #808080;
                    cursor: pointer;
                }
            }
        }

        .header-r {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .search {
                background-color: #eee;
                padding: 5px 10px;
                display: flex;
                height: 40px;
                border-radius: 5px;

                input {
                    outline: none;
                    border: 0;
                    width: 160px;
                    background-color: #eee;
                }

                .el-icon {
                    height: 30px;
                    width: 30px;
                    border-radius: 5px;
                    cursor: pointer;
                }

                .el-icon:hover {
                    background-color: #fff;
                }
            }

            .shop {
                margin: 0 20px;
                height: 40px;
                width: 40px;
                border-radius: 5px;
                cursor: pointer;
                .el-icon {
                    height: 40px;
                    width: 40px;
                }
            }
            .shop:hover {
                background-color: #eee;
            }
            
        }
    }
}
</style>