<template>
    <div class="main-y">
        <div class="novel-info-y">
            <img src="../images/Son41/1.webp" alt="" class="cover-y">
            <img src="../images/Son41/2.webp" alt="" class="background-y">

            <div class="info-y">
                <a href="javascript:;" class="gz-y">&nbsp;+&nbsp;关注</a>
                <div class="title-y">相思引（连载故事）</div>
                <a href="javascript:;" class="author-y">
                    <img src="../images/Son41/3.webp" alt="" class="avatar-y">
                <span class="name-y">东篱若尘</span>
                </a>
                <div class="meta-y">
                    14.3万字 · 6826阅读 · 42人关注
                </div>
            </div>
        </div>

        <div class="intros-y" @click="down">
            爱情，是文学作品永恒的主题，历史，在许多人眼里是枯燥而乏味的，但如果以一个个或凄美或悲壮的爱情故事来了解历史，或许就完全不一样了。所以，本故事集就是选取了大家或熟知或陌生的爱情故事，以细腻的历史细节描写，让读者在感怀于主角的爱情悲剧时，也了解了历史的面貌。
        </div>
        <div class="group">
            <img src="../images/Son41/4.jpg" alt="">
            <a href="javascript:;">历史</a>
            <a href="javascript:;">古风</a>
            <a href="javascript:;">言情</a>
            <a href="javascript:;">付费连载</a>
        </div>
        <hr>
        <a href="javascript:;" class="new">
            <img src="../images/Son41/5.jpg" alt="">
            <span class="time-y">2018-01-08 10:58</span>
            <p>【历史】相思引——风起于末逆水寒（6）</p>
        </a>
        <hr>
        <div class="book-chapters-header-y">
            <span class="mume-y">目录(共40篇)</span>
        </div>
        <div class="book-chapters-y">
            <ul>
                <li class="chapter-y" v-for="item in cartsList">
                    <div class="part-y" v-text="item.count"></div>
                    <a href="javascript:;" class="content-y">
                        <span class="read-y" v-text="item.content"></span>
                        <div class="zt-y">
                            <span class="ls-y" v-text="item.history"></span>
                        </div>
                        <div class="xx-y">
                            <span v-text="item.one"></span>
                            <span v-text="item.two"></span>
                            <span v-text="item.three"></span>
                        </div>
                    </a>
                </li>
                <li class="chapter-y" v-for="item in cartsList1">
                    <div class="part-y" v-text="item.count"></div>
                    <a href="javascript:;" class="content-y">
                        <span class="read-y read-y1" v-text="item.content"></span>
                        <div class="zt-y">
                            <span class="ls-y" v-text="item.history"></span>
                        </div>
                        <div class="xx-y">
                            <span v-text="item.one"></span>
                            <span v-text="item.two"></span>
                            <span v-text="item.three"></span>
                        </div>
                    </a>
                </li>
            </ul>
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
</template>


<style scoped>
.main-y{
    width: 3.75rem;
    height: auto;
    margin: 0 auto;
    padding-left: 0.18rem;
    padding-right: 0.18rem;
}

    .novel-info-y{
        padding: 0.25rem 0.18rem 0;
        overflow: hidden;
        position: relative;
        margin: 0 -0.18rem;
    }

.novel-info-y:after{
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background-color: rgba(0,0,0,.2);
}
    
    .cover-y{
        float: left;
        margin-bottom: -0.03rem;
        width: 0.90rem;
        height: 1.20rem;
        border-radius: 0.04rem;
        box-shadow: 0 4px 10px rgba(0,0,0,.2);
    }

    .background-y{
        position: absolute;
        left: 0;
        top: 0;
        z-index: -1;
        width: 100%;
        height: 100%;
        filter: blur(0.4rem);
        transform: scale(1.5);
    }

    .info-y{
        margin-left: 1.05rem;
    }

    .gz-y{
        display: inline-block;
        float: right;
        margin: 0 0 0.40rem 0.10rem;
        padding: 0 0.05rem;
        height: 0.24rem;
        line-height: 0.22rem;
        font-size: 0.13rem;
        text-align: center;
        border-radius: 0.03rem;
        border: 0.01rem solid #fff;
        background-color: transparent;
        color: #fff;
    }

    .title-y{
        margin-top: 0;
        font-size: 0.20rem;
        line-height: 1.3;
        color: #fff;
    }

    .author-y{
        display: block;
        margin-top: 0.10rem;
        /*height: 0.24rem;*/
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;
    }

    .avatar-y{
        width: 0.24rem;
        height: 0.24rem;
        border-radius: 50%;
        vertical-align: middle;
        display: inline-block;
        float: left;
    }

    .name-y{
        margin-left: 6px;
        font-size: 15px;
        color: #fff;
        vertical-align: middle;
        float: left;
    }

    .meta-y{
        margin: 12px 0 15px;
        font-size: 12px;
        color: #fff;
    }

    .intros-y{
        padding: 0.18rem 0;
        font-size: 0.14rem;
        line-height: 1.5;
        color: #333;
        height: 0.65rem;
        overflow: hidden;
    }

    .group{
        margin-top: -0.40rem;
        padding-bottom: 0.18rem;
        padding-top: 0.5rem;
        overflow: hidden;
    }

.group>img{
    float: left;
    padding-top: 0.05rem;
    margin-right: 0.1rem;
    width: 0.2rem;
    height: 0.2rem;
}

    .group>a{
        display: inline-block;
        margin: 0 0.06rem 0.06rem 0;
        padding: 0.06rem 0.14rem;
        font-size: 0.12rem;
        border-radius: 0.15rem;
        color: #333;
        background-color: #f5f5f5;
        float: left;
    }

    hr{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        border-width: 0;
        height: 0.1rem;
        background-color: #f5f5f5;
    }

    .new{
        display: block;
        padding: 0.15rem 0;
    }

    .new>img{
        float: left;
        width: 0.22rem;
        height: 0.2rem;
    }

    .time-y{
        font-size: 0.12rem;
        color: #999;
        float: right;
        display: block;
        line-height: 0.25rem;
    }

    .new>p{
        margin-right: 1rem;
        font-size: 0.16rem;
        color: #333;
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;
    }

    .book-chapters-header-y{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        height: 0.46rem;
        border-bottom: 0.01rem solid;
        padding: 0.10rem 0.18rem;
        border-color: #eaeaea;
        overflow: hidden;
    }

    .mume-y{
        font-size: 0.14rem;
        font-weight: 700;
        color: #545454;
        padding-left: 0.07rem;
        border-left: 0.03rem solid #ea6f5a;
        float: left;
    }

    .book-chapters-y{
        background-color: #fff;
        height: 100%;
    }
    .chapter-y{
        border-bottom: 0.01rem solid #f0f0f0;
        position: relative;
        padding: 0.18rem 0;
        overflow: hidden;
    }

    .part-y{
        height: 100%;
        width: 0.30rem;
        color: #b1b1b1;
        font-size: 0.17rem;
        line-height: 0.24rem;
        float: left;
    }

    .content-y{
        overflow: hidden;
        display: block;
    }

    .read-y{
        float: right;
        background-color: rgba(218,158,85,.1);
        color: #da9e55;
        display: block;
        width: 0.44rem;
        height: 0.24rem;
        border-radius: 0.12rem;
        font-size: 0.12rem;
        text-align: center;
        line-height: 0.24rem;
    }
    
    .read-y1{
        background-color: #da9e55;
        color: #fff;
    }

    .zt-y{
        width: 2.65rem;
        line-height: 0.21rem;
        height: 0.42rem;

    }

    .ls-y{
        font-size: 0.15rem;
        color: #2f2f2f;
        float: left;
    }

    .xx-y{
        color: #999;
        font-size: 0.12rem;
        line-height: 0.20rem;
        margin-top: 0.04rem;
    }

    .xx-y>span{
        color: #999;
        font-size: 0.12rem;
        line-height: 0.20rem;
    }

    .top-title-y{
        padding: 0.15rem 0.18rem;
        font-size: 0.14rem;
        font-weight: 700;
        color: #545454;
        margin-left: -0.18rem;
        margin-right: -0.18rem;
    }

    .top-title-y>span{
        padding-left: 0.07rem;
        border-left: 0.03rem solid #ea6f5a;
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
            down(){
                var height=document.getElementsByClassName("intros-y")[0];
                height.style.height="1.45rem";
                window.event? window.event.cancelBubble = true : e.stopPropagation();
            },
            up(){
                var height=document.getElementsByClassName("intros-y")[0];
                height.style.height="0.65rem";
            }

        },
        mounted(){
            document.addEventListener("click",this.up)
        },
        data(){
            return{
                cartsList:[
                    {
                        count:"1",
                        content:"试读",
                        history:"【历史】相思引——宁负如来不负卿（1）",
                        one:"字数 3515 · ",
                        two:"阅读 820 · ",
                        three:"11-15 12:18"
                    },
                    {
                        count:"2",
                        content:"试读",
                        history:"【历史】相思引——宁负如来不负卿（2）",
                        one:"字数 3237 · ",
                        two:"阅读 272 · ",
                        three:"11-16 09:34"
                    },
                    {
                        count:"3",
                        content:"试读",
                        history:"【历史】相思引——宁负如来不负卿（3）",
                        one:"字数 3449 · ",
                        two:"阅读 341 · ",
                        three:"11-17 10:17"
                    }
                ],
                cartsList1:[
                    {
                        count:"4",
                        content:"购买",
                        history:"【历史】相思引——宁负如来不负卿（4）",
                        one:"字数 3503 · ",
                        two:"阅读 273 · ",
                        three:"11-18 09:55"
                    },
                    {
                        count:"5",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（1）",
                        one:"字数 3129 · ",
                        two:"阅读 227 · ",
                        three:"11-19 11:16"
                    },
                    {
                        count:"6",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（2）",
                        one:"字数 3756 · ",
                        two:"阅读 253 · ",
                        three:"11-20 14:46"
                    },
                    {
                        count:"7",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（3）",
                        one:"字数 3322 · ",
                        two:"阅读 273 · ",
                        three:"11-21 10:52"
                    },
                    {
                        count:"8",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（4）",
                        one:"字数 3865 · ",
                        two:"阅读 125 · ",
                        three:"11-22 8:43"
                    },
                    {
                        count:"9",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（5）",
                        one:"字数 3643 · ",
                        two:"阅读 225 · ",
                        three:"11-23 12:09"
                    },
                    {
                        count:"10",
                        content:"购买",
                        history:"【历史】相思引——似是故人来（6）",
                        one:"字数 3590 · ",
                        two:"阅读 399 · ",
                        three:"11-24 17:02"
                    }
                ],
                cartsList2:[
                    {
                        img:"src/images/Son41/6.png",
                        title:"寸土芳园",
                        content:"3354369阅读"
                    },
                    {
                        img:"src/images/Son41/7.png",
                        title:"图集",
                        content:"33543阅读"
                    },
                    {
                        img:"src/images/Son41/8.png",
                        title:"风景",
                        content:"3352369阅读"
                    },
                    {
                        img:"src/images/Son41/9.png",
                        title:"人生旅行",
                        content:"1254363阅读"
                    },
                    {
                        img:"src/images/Son41/10.png",
                        title:"湖景",
                        content:"339769阅读"
                    },
                    {
                        img:"src/images/Son41/11.webp",
                        title:"寻虎文学社群",
                        content:"37517阅读"
                    },
                ]
            }

        }

    }
</script>