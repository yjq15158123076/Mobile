<template>
 <div class="main-y">
    <div class="top-part-y">
        <img src="../images/Son5/1.png" alt="" class="background-img">
        <div class="main">
            <img src="../images/Son5/2.png" alt="">
            <div class="slogan">
                <h3>创作你的创作</h3>
                <h6>一个优质创作社区</h6>
            </div>
            <a href="javascript:;" class="link-group-y">iOS 下载</a>
        </div>
        <img src="../images/Son5/3.png" alt="" class="phone-img-y">
    </div>

    <div class="middle-part-y" v-for="item in cartsList">
        <h3 v-text="item.title"></h3>
        <h6 v-text="item.content"></h6>
        <img :src="item.img" alt="" >
    </div>

    <div class="bottom-part-y">
        <img src="../images/Son5/8.png" alt="">
        <div class="tu-y">
            <img src="../images/Son5/9.png" alt="">
            <div class="cm">
                <h3>创作你的创作</h3>
                <h6>一个优质创作社区</h6>
            </div>
            <a href="javascript:;" class="link-group-y">iOS 下载</a>
            <a href="javascript:;" class="more router-link-active">去看看热门文章&nbsp;></a>
        </div>
    </div>
 </div>
</template>


<style scoped>
    .main-y{
        text-align: center;
        overflow: hidden;
        width: 3.75rem;
        height: auto;
        margin: 0 auto;
    }

    .top-part-y{
        position: relative;
       margin-bottom: 0.2rem;
        height: 6.67rem;
    }

    .background-img{
        width: 100%;
    }

    .main{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-2.6rem);
        z-index: 3;
    }
    
    .main img{
        margin-top: 0.2rem;
        width: 1rem;
        height: 1rem;
    }

    .slogan>h3{
        font-size: 0.24rem;
        font-weight: 400;
    }

    .slogan>h6{
        font-size: 0.15rem;
        font-weight: 300;
    }

    .link-group-y{
        background-color: #6dacf4;
        width: 2.40rem;
        padding: 0.13rem 0;
        display: block;
        color: #fff;
        border-radius: 0.04rem;
        font-size: 0.18rem;
        line-height: 0.23rem;
        margin:0.2rem auto 0;
    }

    .phone-img-y{
        position: absolute;
        left: 50%;
        bottom: 0;
        transform: translate(-50%);
        width: 80%;
        z-index: 2;
    }

    .middle-part-y{
        border-bottom: 0.01rem solid #f0f0f0;
        padding: 0.60rem 0 0.30rem;
    }

    .middle-part-y>h3{
        font-size: 0.24rem;
        font-weight: 400;
    }
    .middle-part-y>h6{
        padding: 0.10rem 0.30rem 0.25rem;
        line-height: 0.25rem;
        font-size: 0.15rem;
        font-weight: 300;
    }

    .middle-part-y>img{
        padding-bottom: 0.15rem;
        width: 100%;
    }

    .bottom-part-y{
        padding: 0.40rem 0;
    }

    .bottom-part-y>img{
        width: 100%;
    }

    .tu-y{
        margin: -1.2rem 0 0.20rem;
    }
    
    .tu-y>img{
        width: 0.64rem;
        height: 0.64rem;
        vertical-align: middle;
    }

    .cm{
        display: inline-block;
        margin-left: 0.15rem;
        text-align: left;
        vertical-align: middle;
    }

    .cm>h3{
        font-size: 0.24rem;
        font-weight: 400;
    }

    .cm>h6{
        font-size: 0.15rem;
        font-weight: 300;
    }

    .more{
        display: block;
        margin-top: 0.15rem;
        font-size: 0.15rem;
        color: #999
    }


</style>


<script>

    export default {
        data(){
            return{
                cartsList:[
                    {
                        title:"轻松创作精美图文",
                        content:"简单优雅的设计，可以一次上传多张图片、实时保存、多端同步，使创作分享更方便快捷",
                        img:"./src/images/Son5/4.png"
                    },
                    {
                        title:"多元化的创作社区",
                        content:"一篇短文、一首诗、一幅画，在这里，你的创作将得到全世界的赞赏",
                        img:"./src/images/Son5/5.png"
                    },
                    {
                        title:"百万创作者在简书相遇",
                        content:"在简书，仍有数百万创作者在坚持产出优质创作，有数千万读者在用心交流创作；众多精彩创作，只在简书看得到",
                        img:"./src/images/Son5/6.png"
                    },
                    {
                        title:"自由地交流和沟通",
                        content:"自由地交流和沟通",
                        img:"./src/images/Son5/7.png"
                    }
                ]
            }
        }
    }

</script>