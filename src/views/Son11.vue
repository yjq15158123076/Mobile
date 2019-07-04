<template>
    <div>

        <div class="header-y">
            <div class="mune-y" @click="ml">
                <img src="../images/Son11/1.jpg" alt="">
                目录
                <div class="yc-y">
                    <div class="ml-y">
                        目录(共99篇)
                    </div>
                    <ul>
                        <li v-for="item in cartsList" class="li-y">
                            <div class="part-y" v-text="item.count"></div>
                            <a href="javascript:;">
                                <div class="info-y" v-text="item.title">
                                </div>
                                <div class="liang" v-text="item.content">
                                </div>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="book-info-y">
                <img src="../images/Son11/2.png" alt="">
                <span class=" person-y">普通人需要了解的100个心理常识</span>
            </div>
        </div>

     <div class="wk-y">


        <div class="main-y">
            <h1 class="zt-y">100个心理常识 | 一份来自简书大学堂的福利包</h1>
            <div class="article-y">
                <a href="javascript:;" class="aaa-y">
                    <img src="../images/Son11/3.png" alt="">
                    <div>
                        <span>简书大学堂</span>
                        <span class="yg-y">
                        <img src="../images/Son11/4.png" alt="">
                        简书员工
                    </span>
                    </div>
                </a>
            </div>
        </div>

        <div class="img-page-y">
            <img src="../images/Son11/5.jpg" alt="">
        </div>
        <h4>本期课程暂停售卖，已购买同学可继续回听~</h4>
         <p class="zy-y">本专栏合计共100节心理学故事，旨在简单明了的向大家传达积极向上的心理暗示，让生活不再是黑白两种颜色。</p>

         <div class="next-y">
             <a href="javascript:;">
                 <div class="text-y">
                     <p>下一章 ></p>
                     <span>100个心理常识 | 001：怎样对待讨厌的人？</span>
                 </div>
             </a>
         </div>

         <div class="support-author-y">
             <div class="buy-tips-y">
                 <p>立即拿下整部连载</p>
                 <ul>
                     <li>永久获得所有文章</li>
                     <li>免费收到将来的文章更新</li>
                     <li>立省￥8899902.00</li>
                 </ul>
             </div>
             <a class="btn-y1">拿下整部￥999999.00</a>
             <a class="btn-y2">仅购买本篇￥99999.00</a>
         </div>
         <hr>

         <div class="top-title-y">
             <span>更多精彩连载</span>
         </div>
         <div class="novels-group-y">
             <a href="javascript:;" class="novel-y" v-for="item in cartsList2">
                 <img :src="item.img" alt="" class="covers-y">
                 <div class="js-y" v-text="item.title"></div>
                 <div class="views-count-y" v-text="item.content"></div>
             </a>

         </div>

     </div>




    </div>
</template>

<style scoped>

    .header-y{
        padding-left: 0.18rem;
        padding-right: 0.18rem;
        vertical-align: middle;
        position: fixed;
        left: 0;
        top: 0;
        width: 100%;
        height: 0.46rem;
        border-bottom: 0.01rem solid #f0f0f0;
        z-index: 11;
        background-color: #fff;
    }

    .mune-y{
        float: right;
        font-size: 0.14rem;
        padding-top: 0.15rem;
        color: #333;
        position: relative;
    }
    .mune-y>img{
        width: 0.16rem;
        height: 0.14rem;
    }

    .yc-y{
        position: absolute;
        top: 0;
        left: 0.75rem;
        width: 2.5rem;
        height:7rem ;
        background-color: #d2d2d2;
        transition: all 0.5s;
        overflow: scroll;
    }

    .ml-y{
        width: 3rem;
        height: 0.46rem;
        border-bottom: 0.01rem solid;
        padding: 0.10rem 0.18rem;
        border-color: #eaeaea;
        font-size: 0.14rem;
        font-weight: 700;
        color: #545454;
        position: fixed;
        background-color:#D2D2D2;
    }

    .yc-y>ul{
        margin-left: 0.15rem;
        padding: 0.46rem 0.10rem 0.60rem 0;

    }
    .yc-y>ul>li{
        line-height: 0.30rem;
        border-bottom: 0.01rem solid #f0f0f0;
        padding: 0.18rem 0
    }

    .part-y{
        height: 100%;
        width: 0.30rem;
        color: #b1b1b1;
        font-size: 0.17rem;
        line-height: 0.24rem;
        float: left;
    }


    .li-y>a{
        /*overflow: hidden;*/
        display: block;
        font-size: 0.15rem;
        color: #2f2f2f;
    }

    .info-y{
        padding-right: 0.10rem;
        line-height: 0.21rem;
        max-height: 0.42rem;
    }

    .liang{
        color: #999;
        font-size: 0.12rem;
        line-height: 0.20rem;
        margin-top: 0.04rem;
    }

    .book-info-y{
        display: block;
        overflow: hidden;
        margin-right: 0.60rem;
    }
    
    .book-info-y>img{
        width: 0.17rem;
        height: 0.23rem;
        vertical-align: middle;
        margin-top: 0.11rem;
        margin-right: 0.05rem;
        float: left;
    }

    .person-y{
        display: block;
        margin-top: 0.12rem;
        margin-left: 0.07rem;
        font-size: 0.14rem;
        color: #333;
    }


    .wk-y{
        padding-left: 0.18rem;
        padding-right: 0.18rem;
    }

    .main-y{
        padding-top: 0.52rem;
        padding-left: 0.18rem;
        padding-right: 0.18rem;

    }

    .zt-y{
        margin: 0.15rem 0;
        font-size: 0.30rem;
        font-weight: 700;
        font-family: -apple-system,SF UI Display,Arial,PingFang SC,Hiragino Sans GB,Microsoft YaHei,WenQuanYi Micro Hei,sans-serif;
        line-height: 1.4;
        color: #2f2f2f;
    }

    .article-y{
        margin-bottom: 0.20rem;
        font-size: 0.13rem;
        color: #b1b1b1;
    }

    .aaa-y>img{
        width: 0.34rem;
        height: 0.34rem;
        border-radius: 0.17rem;
        float: left;
        margin-right: 0.05rem;
        margin-top: -0.08rem;
    }

    .aaa-y>span{
        font-size: 0.16rem;
        font-weight: 700;
        line-height: 0.16rem;
        color: #484848;
        margin-top: 0.1rem;
    }
    .yg-y>img{
        width: 0.20rem;
        height: 0.20rem;
        vertical-align: middle;
    }

    .img-page-y{
        margin: 0 0 0.25rem;
        text-align: center;
    }
    
    .img-page-y>img{
        width: 3.39rem;
    }

    h4{
        margin: 0 0 0.15rem;
        font-weight: 700;
        line-height: 1.7;
        text-rendering: optimizelegibility;
        color: #2f2f2f;
        font-size: 0.20rem;
    }

    .zy-y{
        margin-top: 0.5rem;
        margin-bottom: 0.18rem;
        font-size: 0.16rem;
    }

    .next-y{
        margin: 0.50rem 0 0.20rem;
        border-radius: 0.06rem;
        overflow: hidden;
        height: 0.82rem;
        border: 1px solid #e5e5e5;
        font-size: 0;
        position: relative;
        background-color: #f5f5f5;
    }

    .next-y>a{
        display: inline-block;
        width: 100%;
        height: 100%;
        position: relative;
    }

    .text-y{
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 100%;
    }

    .text-y>p{
        font-size: 0.16rem;
        text-align: center;
        color: #333;
    }

    .text-y>span{
        margin-top: 0.05rem;
        padding: 0 0.50rem;
        font-size: 0.12rem;
        color: #999;
        text-align: center;
        line-height: 0.15rem;
        display: -webkit-box;
    }

    .support-author-y{
        padding: 0.20rem 0;
        text-align: center;
        overflow: hidden;
    }

    .buy-tips-y{
        width: 2rem;
        margin: 0 auto;
    }

    .buy-tips-y>p{
        font-size: 0.18rem;
        font-weight: 500;
        line-height: 0.25rem;
        margin-bottom: 0.12rem;
        color: #2f2f2f;
        padding: 0 0.10rem;
    }

    .buy-tips-y>ul{
        text-align: left;
        margin-left: 0.30rem;
        margin-bottom: 0.15rem;
    }

    .buy-tips-y>ul>li{
        line-height: 0.24rem;
        font-size: 0.13rem;
        color: #555;
        list-style:circle inside;
    }

    .btn-y1{
        margin-bottom: 0.17rem;
        padding: 0.08rem 0.48rem;
        font-size: 0.14rem;
        display: inline-block;
        height: 0.40rem;
        line-height: 0.28rem;
        color: #fff;
        background-color: #da9e55;
        width: 2.50rem;
        border-radius: 0.04rem!important;
        float: left;
        text-align: center;
        margin-left: 0.4rem;
    }

    .btn-y2{
        margin-bottom: 0.17rem;
        padding: 0.08rem 0.48rem;
        font-size: 0.14rem;
        display: inline-block;
        height: 0.40rem;
        line-height: 0.28rem;
        color: #ea6f5a!important;
        border: 0.01rem solid #ea6f5a;
        background-color: #fff;
        width: 2.50rem;
        border-radius: 0.04rem!important;
        float: left;
        margin-left: 0.4rem;
    }

    hr{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        border-width: 0;
        height: 0.10rem;
        background-color: #f5f5f5;

    }

    .top-title-y{
        overflow: hidden;
    }

    .top-title-y>span{
        font-size: 0.14rem;
        padding-left: 0.07rem;
        margin-top: 0.1rem;
        border-left: 0.03rem solid #ea6f5a;
        float: left;
    }

    .novels-group-y{
        overflow-x: auto;
        height: auto;
        white-space: nowrap;

    }

    .novel-y{
        padding-left: 0.20rem;
        display: inline-block;
        padding: 0 0.12rem 0.18rem 0;
        vertical-align: top;
    }

    .covers-y{
        width: 0.90rem;
        height: 1.20rem;
        border-radius: 0.04rem;
        font-size: 0;
        /*display: block;*/
    }

    .js-y{
        width: 0.90rem;
        font-size: 0.14rem;
        font-weight: 700;
        color: #333;
        line-height: 0.16rem;
        padding-top: 0.1rem;
        -webkit-line-clamp: 2;
    }

    .views-count-y{
        margin-top: 0.06rem;
        font-size: 0.13rem;
        color: #999;
    }









</style>


<script>


    export default {
        methods:{
            ml(){
                var yc=document.getElementsByClassName("yc-y")[0];
                yc.style.left="-1.75rem";
                window.event? window.event.cancelBubble = true : e.stopPropagation();
            },
            up(){
                    var yc=document.getElementsByClassName("yc-y")[0];
                    yc.style.left="0.75rem";
            }
        },
        mounted(){
            document.addEventListener("click",this.up)
        },
        data(){
            return{
                cartsList:[
                    {
                        count:"99",
                        title:"100个心理常识 | 001：怎样对待讨厌的人？",
                        content:"字数 1808 · 阅读 7645 · 06-11 00:16"
                    },
                    {
                        count:"98",
                        title:"100个心理常识 | 002:为什么说忠言逆耳？",
                        content:"字数 2020 · 阅读 878 · 06-11 00:16"
                    },
                    {
                        count:"97",
                        title:"100个心理常识 | 003:一千次无助会导致麻木",
                        content:"字数 2049 · 阅读 1878 · 06-11 02:46"
                    },
                    {
                        count:"96",
                        title:"100个心理常识 | 004:一见钟倩可以持续多久？",
                        content:"字数 1953 · 阅读 551 · 06-11 02:47"
                    },
                    {
                        count:"95",
                        title:"100个心理常识 | 005:如何高效学习？",
                        content:"字数 2643 · 阅读 1551 · 06-11 02:47"
                    },
                    {
                        count:"94",
                        title:"100个心理常识 | 006:如何高效学习？",
                        content:"字数 1895 · 阅读 240 · 06-11 02:47"
                    },
                    {
                        count:"93",
                        title:"100个心理常识 | 007:社会懈怠效应",
                        content:"字数 1594 · 阅读 123 · 06-11 02:48"
                    },
                    {
                        count:"92",
                        title:"100个心理常识 | 008:你是一个情绪化的人吗？",
                        content:"字数 1276 · 阅读 133 · 06-11 02:48"
                    },
                    {
                        count:"91",
                        title:"100个心理常识 | 009:胆汁质",
                        content:"字数 2212 · 阅读 108 · 06-11 02:48"
                    },

                ],
                cartsList2:[
                    {
                        img:"src/images/Son11/6.webp",
                        title:"好书推荐",
                        content:"2568阅读"
                    },
                    {
                        img:"src/images/Son11/7.webp",
                        title:"华之魂",
                        content:"82213阅读"
                    },
                    {
                        img:"src/images/Son11/8.webp",
                        title:"梦幻泡影",
                        content:"25343阅读"
                    },
                    {
                        img:"src/images/Son11/9.webp",
                        title:"霖山木屋",
                        content:"15159阅读"
                    },
                    {
                        img:"src/images/Son11/10.webp",
                        title:"以夜为眼抒情",
                        content:"178733阅读"
                    },
                    {
                        img:"src/images/Son11/11.webp",
                        title:"画魂",
                        content:"288647阅读"
                    }
                ]
            }
        }

    }

</script>