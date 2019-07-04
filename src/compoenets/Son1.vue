<template>
<div>
   <HeadTop></HeadTop>

    <div class="main-y">
        <div class="collection-info-y">
            <img src="../images/Son1/1.png" alt="" class="tu-y">
            <div class="summary">
                <div class="name-y">简书大学堂精选好课</div>
                <div class="desc-y">
                    <a href="javascript:;">简书大学堂</a>
                    编，92篇文章，2.0万人关注
                </div>
                <div class="intro-y" @click="down">简书大学堂出品，必属精品！关注简书大学堂官方微信公众号：jianshuIT 做第一个知道内部消息的人
                    专题将收录所有简书大学堂精选优质课程，根据课程介绍操作即可报名。
                    点击链接，进入专属积分商城直接购买：
                    <a href="">https://www.jianshu.com/duiba/product</a>
                </div>
                <a href="javascript:;" class="btn-y">关注</a>
            </div>
        </div>
        <hr>
        <ul class="flow-list-sort-y" style="height: 0.5rem">
            <li>
                <router-link to="/son1">最新收录</router-link>
            </li>
            <li>
                <router-link to="/son2">最新评论</router-link>
            </li>
            <li>
                <router-link to="/son3">热门</router-link>
            </li>
        </ul>
        <div class="flow-list-y">

            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/2.webp" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>细读完以下15篇小说，你会开始知道经典是什么</h6>
                        <p class="ppp-y">“成为小说家”为系列课程，目前上线的是课程的第一阶段。 本阶段课程共分叙述者、人物、情节、对话、情绪与意境五大板块...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                         15.22
                    </span>
                    <span>行距版君</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        1
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       54
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/15.png" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>写小说，其实并不难</h6>
                        <p class="ppp-y">很多人的心里，都藏着一个成为小说家的梦想。可同时，这似乎又是个难以企及的梦想。 有的人，绞尽脑汁，却构思不出一个精彩有趣的故事，于是，还没等真正...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       32.9
                    </span>
                    <span>行距版君</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        33
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                      56
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/16.jpg" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>为什么很多人难以决定自己的人生？</h6>
                        <p class="ppp-y">文 /道长是名思维贩子 你好，我是程驿
                            。我郑重地邀请你，加入我的思维课程。 你可能在想
                            ，思考就是我们的本能，任何一个人都会，为什么我们还要学习呢...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       10.6
                    </span>
                    <span>简书大学堂</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        54
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       683
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/17.png" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>想要英语口语好，你就得这么发音啊，大宝贝儿！</h6>
                        <p class="ppp-y">亲爱的大家，我是斯诺，本诺从英国留学归来获得金融+英
                            语同声传译双硕士，一直
                            在简书的更新的英语学习相关的内容，并受到邀请成为简书签约作者。 18岁...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                         16.4
                    </span>
                    <span>                       斯诺姑娘
</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        81
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       531
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <router-link to="/son11">
                             <img src="../images/Son1/18.jpg" alt="">
                        </router-link>
                    </span>
                    <div class="nr-y">
                        <router-link to="/son11">
                        <h6>一份来自简书大学堂的赠送课程</h6>
                        </router-link>
                        <p class="ppp-y">说在前面的： 这个专栏，是简书大学堂的17年的年度回馈课
                            程。 100节人人都要了解的心理学常识=9.9元 原价199
                            旨在简单明了的向大家传达积...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                      16.4
                    </span>
                    <span>简书大学堂</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        63
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       110
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/19.jpg" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>无戒365天极限挑战营（报名截止）</h6>
                        <p class="ppp-y">如果我告诉你， 一年365天， 每天听一次写作微课， 每天倒逼自己写一
                            篇文章， 你敢不敢来挑战自己？ 如果我告诉你， 有人坚持日更3个月， 获得...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       5.8
                    </span>
                    <span>无戒</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        632
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       774
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/20.jpg" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>为什么那么多人都学英语，但是没有成效？（报名截止）</h6>
                        <p class="ppp-y">一秒钟读完全文： 方法不对！ 这正呼应了一句广为流传的心灵鸡汤：
                            你只是看上去十分努力。 诺仔收到过不少关于英语问题的私信，其中本诺最不想回答的...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       3.2
                    </span>
                    <span>斯诺姑娘</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        33
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       591
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/21.jpg" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>年轻人，只有读书才能逆袭？趁着年轻多读点书吧</h6>
                        <p class="ppp-y">文：安梳颜、阿肆 间歇性踌躇满志，
                            持续性混吃等死， 这是现在很多人的常态，
                            他们一遍又一遍地抱怨生活，却从没想过原因。 他们永远都活在压抑的氛...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       1.0
                    </span>
                    <span>安梳颜</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        183
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       2142
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/22.png" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>简书上，你想要的干货，这里全部都有</h6>
                        <p class="ppp-y">文/学堂菌 嗯，我就是一个卖课的小哥儿。老板指哪儿，我
                            打哪儿。 最近寻思着感恩节也到了，把大学堂里的干货课都给大家伙儿备上
                            吧。 有需要的请戳如下...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       64.0
                    </span>
                    <span>简书大学堂</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        24
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       109
                    </span>

                </div>

            </div>
            <div class="box-y">
                <a href="javascript:;" class="aaa-y">
                    <span class="wrap-y">
                        <img src="../images/Son1/23.jpg" alt="">
                    </span>
                    <div class="nr-y">
                        <h6>你比新来的同事到底差在哪了？</h6>
                        <p class="ppp-y">“少给我弄这些花里胡哨的，没有数据你这就是猜！”
                            第N次策划案被老板甩一脸后，看着新来的小杨次次一稿过，小李留下了无
                            助的泪水。 早已经拜托了公司...</p>
                    </div>
                </a>
                <div class="oneline-y">
                     <span>
                        <img src="../images/Son1/4.jpg" alt="">
                       1.8
                    </span>
                    <span>简书大学堂</span>
                    <span>
                        <img src="../images/Son1/5.jpg" alt="">
                        26
                    </span>
                    <span>
                        <img src="../images/Son1/6.jpg" alt="">
                       118
                    </span>

                </div>

            </div>


        </div>


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

    .collection-info-y{
        padding: 0.20rem 0 0.15rem;
        min-height: 1.12rem;
    }

    .tu-y{
        width: 0.72rem;
        height: 0.72rem;
        border-radius: 0.07rem;
        border: 0.01rem solid #ddd;
        margin-right: 0.13rem;
        float: left;
    }

    .summary{
        overflow: hidden;
    }

    .name-y{
        margin-right: 0.05rem;
        font-size: 0.19rem;
        font-weight: 700;
        display: inline-block;
        vertical-align: middle;
        line-height: 1.3;
        color: #484848;
        float: left;
    }

    .desc-y{
        font-size: 0.14rem;
        color: #969696;
        padding: 0.1rem 0 0.1rem;
        float: left;
    }

    .desc-y>a{
        color:#3194d0;
    }

    .intro-y{
        float: left;
        font-size: 0.12rem;
        line-height: 0.20rem;
        color: #484848;
        height: 0.4rem;
        overflow: hidden;
    }

    .intro-y>a{
        color:#3194d0;
    }

    .btn-y{
        width: 100%;
        margin: 0.12rem 0;
        background-color: #42c02e;
        border: 0.01rem solid #42c02e;
        color: #fff;
        height: 0.40rem;
        display: inline-block;
        border-radius: 0.04rem;
        text-align: center;
        padding: 0.06rem 0;
        font-size: 0.16rem;
        float: left;
    }

    hr{
        margin-left: -0.18rem;
        margin-right: -0.18rem;
        border-width: 0;
        height: 0.10rem;
        background-color: #f5f5f5;
    }

    .flow-list-sort-y{
        margin: 0 -0.18rem;
        list-style: none;
        border: 0.01rem solid #f0f0f0;
        border-right: none;
        border-left: none;
    }

    .flow-list-sort-y>li{
        position: relative;
        display: inline-block;
        width: 27.333%;
        margin: -0.01rem 0;
        padding: 0.15rem 0;
        text-align: center;
        font-size: 0.14rem;
        color: #999;
        float: left;
    }

    .flow-list-sort-y>li:nth-child(1){
        color: #ea6f5a;
    }

    .flow-list-sort-y>li:nth-child(1):after{
        content: "";
        position: absolute;
        bottom: 0;
        left: 50%;
        margin-left: -0.28rem;
        width: 0.56rem;
        border-bottom: 0.02rem solid #ea6f5a;
    }

    .flow-list-y{
        width: 100%;
        height: auto;
    }

    .box-y{
        position: relative;
        width: 100%;
        word-wrap: break-word;
        padding: 0.15rem 0.18rem;
        margin: 0 -0.18rem;
        box-sizing: content-box;
        border-bottom: 0.01rem solid;
        border-color: #f0f0f0;
        font-size: 0;
    }

    .box-y:before{
        content: "";
        clear: both;
        display: table;
    }

    .box-y:after{
        content: "";
        clear: both;
        display: table;
    }

    .aaa-y{
        margin-top: 0.06rem;
        display: block;
        padding-right: 0.95rem;
    }

    .wrap-y{
        position: absolute;
        top: 50%;
        right: 0.15rem;
        margin-top: -0.40rem;
        border-radius: 0.03rem;
        width: 0.80rem;
        height: 0.80rem;
    }

    .wrap-y img{
        width: 100%;
        height: 100%;
        display: block;
    }

    .nr-y{
        overflow: hidden;
    }

    .nr-y h6{
        font-size: 0.18rem;
        font-weight: 700;
        color: #333;
        overflow: hidden;
        line-height: 0.25rem;
    }

    .nr-y>p{
        margin-top: 0.06rem;
        font-size: 0.13rem;
        color: #999;
        line-height: 0.19rem;
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;
    }

    .oneline-y{
        margin-top: 0.08rem;
        line-height: 0.22rem;
        padding-right: 0.95rem;
    }

    .oneline-y>span>img{
        width: 0.15rem;
        height: 0.15rem;
    }

    .oneline-y span {
        margin-right: 0.10rem;
        font-size: 0.12rem;
        color: #b1b1b1;
    }







</style>

<script>
    import HeadTop from "./HeadTop.vue";
    export default {
        components: {
            HeadTop
        },
        methods:{
            down(){
                var height=document.getElementsByClassName("intro-y")[0];
                height.style.height="1.2rem";
                window.event? window.event.cancelBubble = true : e.stopPropagation();
            },
            up(){
                var height=document.getElementsByClassName("intro-y")[0];
                height.style.height="0.4rem";
            }

        },
        mounted(){
            document.addEventListener("click",this.up)
        },
    }
</script>