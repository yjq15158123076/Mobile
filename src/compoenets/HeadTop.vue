<template>
    <div>
        <div class="main">
            <div class="header-wrap-y">
                <div class="header-normal-y">
                    <div class="logo-wrap-y">
                        <router-link to="/home">
                        <img src="../images/HomeMobile/1.png" alt="logo" class="logo-y">
                        </router-link>
                        <span class="slogan-y">创作你的创作</span>
                    </div>
                    <div class="header-download-y">
                        免费下载&nbsp;>
                    </div>

                </div>
            </div>
        </div>

    </div>

</template>

<style scoped>

    *{
        padding: 0;
        margin: 0;
    }

    body{
        font-family: -apple-system,SF UI Text,Arial,PingFang SC,Hiragino Sans GB,Microsoft YaHei,WenQuanYi Micro Hei,sans-serif;
        font-size: 0.14rem;
        font-weight: 400;
        line-height: 0.16rem;
    }

    .main{
        width: 3.75rem;
        margin: 0 auto;
    }

    .header-normal-y{
        z-index: 10;
        position: fixed;
        left: 0;
        right: 0;
        top: 0;
        padding: 0.03rem 0.18rem;
        font-size: 0;
        background-color: #fff;
        box-shadow: 0 2px 4px rgba(0,0,0,.1);
        height: 0.48rem;
    }

    .logo-wrap-y{
        height: 100%;
        float: left;
    }

    .logo-y{
        width: 0.56rem;
        height: 0.42rem;
        vertical-align: middle;
    }

    .slogan-y{
        line-height: 0.2rem;
        vertical-align: middle;
        margin-left: 0.12rem;
        display: inline-block;
        font-size: 0.16rem;
        color: #333;
    }

    .header-download-y{
        position: absolute;
        padding: 0.12rem 0.15rem;
        right: 0;
        top: 0;
        font-size: 0.16rem;
        color: #ea6f5a;
        line-height: 1.6;
    }

</style>


<script>

</script>