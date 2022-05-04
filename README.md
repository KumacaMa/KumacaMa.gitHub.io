<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KumacaM的小窝awa!</title>
    <style>
        * {
            padding: 0;
            margin: 0;
        }

        body {
            background-color: rgb(255, 255, 255);
        }
        .shell{
            width: 100%;
            height: 100%;
            background-color: rgb(255, 255, 255);
            overflow: hidden;
        }
        .page{
            transform: translateX(-110%);
            position: absolute;
            width: 50%;
            height: 100%;
            transition: .5s;
            background-size: cover;
        }
        .button{
            display: block;
            width: 10%;
            color: rgb(255, 255, 255);
            font-size: 30px;
            border-bottom: #fff solid 4px;
            text-align: center;
            position: absolute;
            bottom: 10px;
            margin: 50px;
            left: calc(50% + (var(--i)*17%));
            z-index: 999;
            transition: .3s;
        }
        .page_content{
            box-sizing: border-box;
            height: 100%;
            padding: 50px;
            color: #FFF;
            position: absolute;
            left: 100%;
            display: none;
            animation-name: fade;
            animation-duration: .7s;
            animation-iteration-count: 1;
            opacity: 1;
        }
        @keyframes fade{
            0%{
                opacity: 0;
            }
            50%{
                opacity: 0;
                transform: translateY(-50px);
            }
            100%{
                opacity: 1;
                transform: translateY(0px);
            }
        }
        input{
            display: none;
        }
        input:checked+.page{
            transform: translateX(0px);
            transition: .4s;
        }
        input:checked+.page .page_content{
            width: 100%;
            display: block;
        }
        .page:nth-child(3){
            background-image: url('./1.jpeg');
        }
        .page:nth-child(3) .page_content{
            background-color: rgb(225,143,85);
        }

        .page:nth-child(6){
            background-image: url('./2.jpeg');
        }
        .page:nth-child(6) .page_content{
            background-color: rgb(177,90,96);
        }

        .page:nth-child(9){
            background-image: url('./3.jpeg');
        }
        .page:nth-child(9) .page_content{
            background-color: rgb(236,180,110);
        }
        .page h1{
            font-size: 70px;
        }
        .page p{
            font-size: 30px;
            padding: 10px;
            background-color: rgba(0, 0, 0, .3);
            border-radius: 10px;
            margin: 30px 0;
        }
        .page span{
            font-size: 26px;
            letter-spacing: 2px;
            color: rgb(56, 56, 56);
        }
        label:hover{
            cursor: pointer;
            border-bottom: solid 4px rgb(35, 35, 35);
        }
        
    </style>
</head>

<body>
    <div class="shell">
        <label for="button1" class="button" style="--i:0">介绍</label>
        <input type="radio" id="button1" name="page" checked>
        <div class="page">
            <div class="page_content">
                <h1>KumacaM!就是本人~</h1>
                <p>个人爱好：<BR>爱画画，爱听歌（吹爆Shirobon！）爱兽兽~<BR>UI/UX设计之类的o~</p>
                <span>
                    「画画不是完成任务，学美术只是从另一个角度看世界，
                    我不追求画的是否真实，因为画的像是照相机的工作，画面中的意境才是最重要的」
                    
                </span>
                <P>
                    个人资料：<BR>22岁~男性，身高189cm，喜欢白色~喜欢8bit歌曲。<BR>-QQ:1761719721(可以约稿，探讨哦~)<BR>-邮箱:1761719721@QQ.COM
                </P>
            </div>
        </div>


        <label for="button2" class="button" style="--i:1">开始</label>
        <input type="radio" id="button2" name="page">
        <div class="page">
            <div class="page_content">
                <h1>欢迎来到KumacaM的个人网站。</h1>
                <p>这里分享最近的动态以及作品哦~</p>
                <span><br><br><br><br>NOPE
                
                </span>
            </div>
        </div>


        <label for="button3" class="button" style="--i:2">关于</label>
        <input type="radio" id="button3" name="page">
        <div class="page">
            <div class="page_content">
                <h1>关于</h1>
                <span>
                此网站源代码是公开的，可以使用，只要在后面加上我的名字就可以了哦~   
                </span>
                <p>感谢GitHub平台给我展示的平台！谢谢！</p>
                
            </div>
        </div>
    </div>

</body>

</html>
