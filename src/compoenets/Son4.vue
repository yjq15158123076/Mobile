<template>
   <div class="main-y">
       <p class="total-y">共为您找到284部该标签下的连载作品</p>
       <div class="clearfix-y">

           <div class="book-wrap" v-for="item in cartsList">
               <div class="book-y">
                   <span class="paid-badge" v-text="item.fq"></span>
                   <img :src="item.img" alt="" class="banner-y">
                   <div class="info-y">
                       <p class="title-y" v-text="item.title"></p>
                       <div class="user-panel">
                           <span>
                               <img :src="item.img1" alt="" class="avatar-y">
                               <span class="nickname-y" v-text="item.name"></span>
                           </span>
                           <span class="readit-y" v-text="item.liang"></span>

                       </div>

                   </div>
               </div>
           </div>
            <div class="book-wrapy">
               <div class="book-yy">
                   <span class="paid-badgey">付费</span>
                   <router-link to="/son41">
                   <img src="../images/Son4/22.webp" alt="" class="banner-yy">
                   </router-link>
                   <div class="info-yy">
                       <p class="title-yy">相思引（连载故事）</p>
                       <div class="user-panely">
                           <span>
                               <img src="../images/Son4/23.png" alt="" class="avatar-yy">
                               <span class="nickname-yy">东篱若尘</span>
                           </span>
                           <span class="readit-yy"> 6.8k阅读</span>
                       </div>
                   </div>
               </div>
           </div>


       </div>

   </div>
</template>


<style scoped>

    .main-y{
        width: 3.75rem;
        height: 11rem;
        margin: 0 auto;
        background-color: #f5f5f5;
        padding: 0.15rem 0.10rem;
    }

    .total-y{
        max-width: 9.60rem;
        margin: 0 auto 0.05rem;
        padding-left: 0.05rem;
        font-size: 0.12rem;
        color: #999;
    }

    .clearfix-y{
        position: relative;
        max-width: 9.60rem;
        height: 100%;
        margin: 0 auto;
    }

    .book-wrap{
        padding: 0.05rem;
        width: 33.33%;
        height:auto;
        float: left;
    }

    .book-y{
        width: 100%;
        height: auto;
        border-radius: 0.04rem;
        overflow: hidden;
        position: relative;
    }

    .paid-badge{
        position: absolute;
        top: 0;
        left: 0;
        width: 0.30rem;
        height: 0.15rem;
        background-color: #e2b882;
        font-size: 0.10rem;
        line-height: 0.15rem;
        color: #fff;
        text-align: center;
        z-index: 10;
        border-radius: 0 0 0.04rem 0;
    }

    .banner-y{
        display: block;
        width: 100%;
        height: 100%;
    }

    .info-y{
        height: 1rem;
    }

    .title-y{
        font-size: 0.17rem;
        margin: 0.06rem 0;
        color: #2f2f2f;
        overflow: hidden;
        text-overflow: ellipsis;
        line-height: 0.21rem;
        max-height: 0.42rem;
        box-sizing: content-box;
        white-space: normal;
    }

    .user-panel{
        position: relative;
        display: block;
        height: 0.24rem;
    }

    .avatar-y{
        position: absolute;
        left: 0;
        top: -0.01rem;
        display: block;
        width: 0.16rem;
        height: 0.16rem;
        border-radius: 50%;
    }

    .nickname-y{
        display: block;
        height: 0.28rem;
        width: 200%;
        font-size: 0.22rem;
        color: #999;
        transform: scale(.5);
        transform-origin: left top;
        margin-left:0.2rem;
    }

    .readit-y{
        display: block;
        height: 0.28rem;
        width: 200%;
        font-size: 0.22rem;
        color: #999;
        transform: scale(.5);
        transform-origin: left top;
    }




    .book-wrapy{
        padding: 0.05rem;
        width: 33.33%;
        height:auto;
        float: left;
    }

    .book-yy{
        width: 100%;
        height: auto;
        border-radius: 0.04rem;
        overflow: hidden;
        position: relative;
    }

    .paid-badgey{
        position: absolute;
        top: 0;
        left: 0;
        width: 0.30rem;
        height: 0.15rem;
        background-color: #e2b882;
        font-size: 0.10rem;
        line-height: 0.15rem;
        color: #fff;
        text-align: center;
        z-index: 10;
        border-radius: 0 0 0.04rem 0;
    }

    .banner-yy{
        display: block;
        width: 100%;
        height: 100%;
    }

    .info-yy{
        height: 1rem;
    }

    .title-yy{
        font-size: 0.17rem;
        margin: 0.06rem 0;
        color: #2f2f2f;
        overflow: hidden;
        text-overflow: ellipsis;
        line-height: 0.21rem;
        max-height: 0.42rem;
        box-sizing: content-box;
        white-space: normal;
    }

    .user-panely{
        position: relative;
        display: block;
        height: 0.24rem;
    }

    .avatar-yy{
        position: absolute;
        left: 0;
        top: -0.01rem;
        display: block;
        width: 0.16rem;
        height: 0.16rem;
        border-radius: 50%;
    }

    .nickname-yy{
        display: block;
        height: 0.28rem;
        width: 200%;
        font-size: 0.22rem;
        color: #999;
        transform: scale(.5);
        transform-origin: left top;
        margin-left:0.2rem;
    }

    .readit-yy{
        display: block;
        height: 0.28rem;
        width: 200%;
        font-size: 0.22rem;
        color: #999;
        transform: scale(.5);
        transform-origin: left top;
    }






</style>


<script>
    export default {
        data(){
            return{
                cartsList:[
                    {
                        fq:"付费",
                        img:"src/images/Son4/1.webp",
                        title:"跟我一起去留学",
                        img1:"src/images/Son4/2.jpg",
                        name:"搬来的救兵",
                        liang:"9.5k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/3.webp",
                        title:"拿下英语",
                        img1:"src/images/Son4/2.jpg",
                        name:"搬来的救兵",
                        liang:"11.4k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/4.webp",
                        title:"皇宫记",
                        img1:"src/images/Son4/5.jpeg",
                        name:"本公子",
                        liang:"11.9k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/6.webp",
                        title:"晖宗聊绘画",
                        img1:"src/images/Son4/7.jpg",
                        name:"晖宗聊绘画",
                        liang:"76.3k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/8.webp",
                        title:"【科幻】快乐星球Ⅴ",
                        img1:"src/images/Son4/9.png",
                        name:"冰镇火药",
                        liang:"19.3k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/10.webp",
                        title:"白话聊斋",
                        img1:"src/images/Son4/11.png",
                        name:"池风晓",
                        liang:"35.4k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/12.webp",
                        title:"人生逆转：小白理财奋斗记",
                        img1:"src/images/Son4/13.jpg",
                        name:"念伊伊",
                        liang:"56.2k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/14.webp",
                        title:"创业碎片",
                        img1:"src/images/Son4/15.jpg",
                        name:"简叔",
                        liang:"79.1k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/16.webp",
                        title:"职场PPT速成指南",
                        img1:"src/images/Son4/17.jpg",
                        name:"郑少PPT",
                        liang:"505.3k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/18.webp",
                        title:"朱砂泪",
                        img1:"src/images/Son4/19.png",
                        name:"许彧彧",
                        liang:"5k阅读"
                    },
                    {
                        fq:"付费",
                        img:"src/images/Son4/20.webp",
                        title:"西游前战 朱雀篇（上集）",
                        img1:"src/images/Son4/21.jpg",
                        name:"一鸣",
                        liang:"0阅读"
                    },
                ]
            }
        }
    }
</script>