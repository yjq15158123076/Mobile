<template>
    <div>
        <HeadTop></HeadTop>

        <div class="main-y">
            <div class="collection-recommended-y">
                <div class="top-title-y">
                    <span>热门专题1111</span>
                    &nbsp; &nbsp; &nbsp;
                    <!--<span class="collection-change-y">换一换</span>-->
                </div>
                <div class="flow-list-container-y">
                    <a href="javascript:;">美食</a>
                    <a href="javascript:;">漫画</a>
                    <router-link to="/son1">简书大学堂</router-link>
                    <router-link to="/son4">优选连载</router-link>
                    <router-link to="/son5">下载App</router-link>
                    <a href="javascript:;">娱乐圈</a>
                </div>
            </div>
            <hr>
            <ul class="flow-list-ul-y">
                <li class="note-flow have-img" v-for="item in cartsList">
                    <a href="javascript:;" class="content-y">
                        <span class="wrap-img">
                            <img :src="item.img" alt="">
                        </span>
                        <div class="summary-y">
                            <h6 class="title-y" v-text="item.title">
                            </h6>
                            <p class="abstract-y" v-text="item.content">
                            </p>
                        </div>
                    </a>
                    <div class="meta-y oneline">
                        <img :src="item.logo1" alt="" style="vertical-align: baseline;" >
                        <span v-text="item.one"></span>
                        <span v-text="item.two"></span>
                        <img :src="item.logo2" alt="" style="vertical-align: baseline;" >
                        <span v-text="item.three"></span>
                        <img :src="item.logo3" alt="" style="vertical-align: baseline;" >
                        <span v-text="item.four"></span>
                    </div>
                </li>
            </ul>
        </div>


    </div>
</template>

<style scoped>

    .main-y{
        width: 3.75rem;
        height: auto;
        margin: 0 auto;
        padding-left: 0.18rem;
        padding-right: 0.18rem;
        padding-top: 0.55rem;
    }

    .top-title-y{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        padding: 0.10rem 0.18rem;
        font-size: 0.14rem;
        font-weight: 700;
        color: #545454;
    }

    .collection-change-y{
        float: right;
        color: #888;
        font-size: 0.13rem;
        font-weight: 400;
        line-height: 1.75;
    }

    hr{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        border-width: 0;
        height: 0.10rem;
        background-color: #f5f5f5;
    }

    .flow-list-container-y{
        padding-bottom: 0.05rem;
        background-color: transparent;
        height: auto;
        overflow: hidden;
    }

    .flow-list-container-y>a{
        display: inline-block;
        padding: 0.02rem 0.10rem;
        margin: 0 0.12rem 0.12rem 0;
        font-size: 0.14rem;
        color: #ea6f5a;
        border-radius: 0.08rem;
        border: 0.01rem solid #ea6f5a;
        float: left;
    }

        /*.flow-list-container-y>a:after{*/
            /*content: "";*/
            /*position: absolute;*/
            /*top: 0;*/
            /*left: 0;*/
            /**/
            /*width: 200%;*/
            /*height: 200%;*/
            /*border-radius: 0.08rem;*/
            /*transform: scale(.5);*/
            /*transform-origin: left top;*/
        /*}*/

    .flow-list-ul-y{
        width: 100%;
        margin-top: 0;
        margin-bottom: 0;
        padding-left: 0;
    }

    .note-flow{
        position: relative;
        width: 100%;
        word-wrap: break-word;
        padding: 0.15rem 0.18rem;
        margin: 0 -0.18rem;
        box-sizing: content-box;
        border-bottom: 0.01rem solid;
        font-size: 0;
        border-color: #f0f0f0;
    }

    .content-y{
        padding-right: 0.95rem;
        margin-top: 0.06rem;
        display: block;
    }
    
    .wrap-img{
        width: 0.80rem;
        height: 0.80rem;
        position: absolute;
        top: 50%;
        right: 0.15rem;
        margin-top: -0.40rem;
        border-radius: 0.03rem;
    }

    .wrap-img>img{
        width: 100%;
        height: 100%;
        display: block;
    }

    .title-y{
        font-size: 0.18rem;
        font-weight: 700;
        color: #333;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        line-height: 0.25rem;
        max-height: 0.50rem;
        box-sizing: content-box;
        white-space: normal;
    }

    .abstract-y{
        margin-top: 0.06rem;
        font-size: 0.13rem;
        line-height: 1.5;
        color: #999;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        max-height: 0.38rem;
        box-sizing: content-box;
        white-space: normal;
    }

    .meta-y{
        padding-right: 0.95rem;
        margin-top: 0.08rem;
        line-height: 0.22rem;
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;
    }

    .meta-y>img{
        width: 0.12rem;
        height: 0.10rem;
    }

    .meta-y>span{
        margin-right: 0.08rem;
        font-size: 0.12rem;
        color: #b1b1b1;
        line-height:0.2rem;
    }



</style>
<script>

    import HeadTop from "./HeadTop.vue";
    export default {
        name: "Home",
        components: {
            HeadTop
        },
        data(){
            return{
                cartsList:[
                    {
                        img:'./src/images/HomeMobile/2.webp',
                        title:"吃糕点",
                        content:"大姑姐送来一块松糕，婆婆说“好西好（很好吃）”，让我切了吃。 我举着刀，正思量如何下手，老公说他来切，挽起袖子三下...",
                        one:"27.085",
                        two:"花盆里有棵小榕树",
                        three:"32",
                        four:"124",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/6.webp',
                        title:"踮脚尖可收肚腩！每天只需30秒就可减肚腩的瘦身法",
                        content:"即使瘦身成功，肚腩问题仍未解决。或者问题是可能肌肉的记忆问题。 其实大多数肌肉都会记住了肥胖时的形态，所以肚腩问题...",
                        one:"8.926",
                        two:"小狐的减肥日记",
                        three:"0",
                        four:"43",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/7.webp',
                        title:"阿拉为了主人的健康，把自己吃成小猪仔，行动不便的阿拉令人感动",
                        content:"编者按：养一只汪星人真的是人生一大幸事！在现在这个快节奏、压力倍增的社会下，大多数的上班族都有健康问题，尤其是精神...",
                        one:"7.821",
                        two:"陆三爱吃鱼",
                        three:"6",
                        four:"30",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/8.webp',
                        title:"懒人面包做法，不用揉面更不用揉出手膜，柔软拉丝，比买的还好吃",
                        content:"说到排面包，我们都会对它那大大的个头记忆犹新！有种一次吃过瘾的劲头呢！要知道排面包可是一款很棒的早餐呢！因为只用搭...",
                        one:"32.312",
                        two:"一勺美食",
                        three:"18",
                        four:"150",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/9.webp',
                        title:"200元起家2年赚300万",
                        content:"中大一名大三在校学生，却运用他的聪明才智和高EQ，两年就赚到这笔钱。他叫潘文伟，2007年刚来广州时，口袋里只有2...",
                        one:"3.622",
                        two:"知识云虚拟孵化育成总部",
                        three:"6",
                        four:"37",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/10.webp',
                        title:"日本青年解释：为什么日本娱乐节目这么疯狂，让中国人难以接受？",
                        content:"人物背景：上原丈二(Johji Uehara)，日本青年，毕业于德拉萨尔大学(Studied at De La S...",
                        one:"3.836",
                        two:"小小润仔",
                        three:"4",
                        four:"23",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    },
                    {
                        img:'./src/images/HomeMobile/11.webp',
                        title:"2019年，一起活成美丽高级的模样！",
                        content:"高级的幸福力是生活的智慧，会让生命实现由内到外的美好。活出高级感的人，对“里”不将就。——王薇华 文/俊英子 时光...",
                        one:"44.464",
                        two:"俊英子",
                        three:"22",
                        four:"280",
                        logo1:"./src/images/HomeMobile/3.png",
                        logo2:"./src/images/HomeMobile/4.png",
                        logo3:"./src/images/HomeMobile/5.png",
                    }

                ]
            }
        }
    }
</script>