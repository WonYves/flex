# flex
主要为flex布局 学习css时做的支付宝小案例

![_J3P%T~Z(){67X~{`TV@_C3](https://user-images.githubusercontent.com/113281531/193458249-1bc99099-a2cc-452b-b0f8-4bdc86b6f0d3.png)


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="font/iconfont.css">
    <style>
        *{
            margin: 0;
            padding: 0;
        }
        .box{
            height: 1425px;
            width: 955px;
            display: flex;
            margin: auto;
            flex-direction: column;

            /* background-color: violet; */
        }
        /* header设置部分 */
        header{
            height: 124px;
            background-color: #242a3a;
            display: flex;

        }

        header i{
            width: 116px;
            height: 124px;
            line-height: 124px;
            text-align: center;
            font-size: 50px;
            color: white;
        }
        header span{
            flex: 1;
            line-height: 124px;
            font-size: 40px;
            color: white;
        }


        /* fotter设置部分 */
        footer{
            height: 128px;
            /* background: pink; */
            display: flex;
            /* background: green; */
            justify-content: space-around;
            align-items: center;
            /* border-top: 1px solid gray; */
        }
        footer div{
            flex: 1;
            background: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            color: #abacae;

        }
        .box footer div:hover{
            color: #35b3e6;
        }
        footer div i{
            font-size: 60px;
            text-align: center;
        }
        footer div span{
            font-size: 27px;
            text-align: center;
        }


        /* footer div i[class="iconfont icon-zhifubao"]{
            color: #06a8e9;
        }
        .zhifubao{
            color: #06a8e9;
        } */
        /* section设置部分 */
        section{
            flex: 1;
            background: #f4f5f9;
        }
        .main1{
            display: flex;
            height: 283px;
            background: #242a3a;
            justify-content: space-around;
            align-items: center;
        }
        .main1 div{
            width: 109px;
            height: 172px;
            /* background: pink; */
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            color: white;
        }
        .main1 div i{
            font-size: 105px;
        }
        .main1 div span{
            font-size: 36px;
            text-align: center;
        }
        .main2{
            display: flex;
            height: 640px;
            width: 955px;
            /* background: yellow; */
            flex-wrap: wrap;
        }
        .main2 div{
            width: 25%;
            height: 213px;
            display: flex;
            background: white;
            border: 1px solid #ececec;
            box-sizing: border-box;
            justify-content: center;
            flex-direction: column;
        }
        .main2 div i{
            font-size: 65px;
            text-align: center;
            color: #fbb45a;
        }
        .main2 div span{
            font-size: 30px;
            text-align: center;
        }
        .main2 div i[class="iconfont icon-bianji"]{
            color: #35b3e6;
        }
        /* 属性选择器权重没有后代选择器高 */
        .src{
            margin-top: 20px;
            background-repeat: no-repeat;
            /* border-top: 1px solid gray; */
            background-size: 100%;
        }

    </style>
</head>
<body>
    <div class="box">
        <header>
            <i class="iconfont icon-zixun"></i>
            <span>账单</span>
            <i class="iconfont icon-user"></i>
            <i class="iconfont icon-fangdajing"></i>
            <i class="iconfont icon-jia"></i>
        </header>
        <section>
            <div class="main1">
                <div>
                    <i class="iconfont icon-zanting3"></i>
                    <span>扫一扫</span>
                </div>
                <div>
                    <i class="iconfont icon-zhifu-01"></i>
                    <span>付款</span>
                </div>
                <div>
                    <i class="iconfont icon-zhuanhuan"></i>
                    <span>卡券</span>
                </div>
                <div>
                    <i class="iconfont icon-shoucang1"></i>
                    <span>咻一咻</span>
                </div>
            </div>
            <div class="main2">
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>信用卡还款</span>
                </div>
                <div>
                    <i class="iconfont icon-bianji"></i>
                    <span>记账本</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>股票</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>理财小工具</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>淘宝</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>游戏充值</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>亲密付</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>机票火车票</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>手机充值</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>转账</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>口碑外卖</span>
                </div>
                <div>
                    <i class="iconfont icon-qiaquan"></i>
                    <span>阿里旅行</span>
                </div>
            </div>
            <div class="src">
                <img src="./1.png" alt="">
            </div>
        </section>
        <footer>
            <div>
                <i class="iconfont icon-zhifubao"></i>
                <span class="zhifubao">支付宝</span>
            </div>
            <div>
                <i class="iconfont icon-tianbiao"></i>
                <span>口碑</span>
            </div>
            <div>
                <i class="iconfont icon-pengyouquan"></i>
                <span>朋友圈</span>
            </div>
            <div>
                <i class="iconfont icon-user"></i>
                <span>我的</span>
            </div>
        </footer>
    </div>
</body>
</html>

