##零基础学习写一个界面

第一次动手写一个小界面，没有html跟css的基础，今天琢磨了半天，成果在这，直接上图


![](http://7xtsii.com1.z0.glb.clouddn.com/QQ%E6%88%AA%E5%9B%BE20160717212234.jpg)

直接看源码，因为今天刚刚接触，有不对的地方请多多指教，源代码如下：
    
    `<html>
    <head>
    <style type="text/css">
    
    //定义各个块:主要的框框、大标题、文本框、按钮块
    div#content{background-color:#FFFFFF;height:650px;width:350px;margin-left: 13cm; margin-top:3cm;border-radius: 10px;}
    div#title{padding-left: 3cm;padding-top: 0.5cm;}
    div#text{padding-left: 0.5cm;padding-top: 0.5cm;}
    div#btns{padding-left: 0.5cm;padding-top: 0.5cm;}

    
    h4{padding-left: 0.5cm;}

    //声明文本框的一些样式属性
    .testStyle{
    width:300px;//宽
    height:40px;//高
    border-radius:5px; //圆角半径，达到文本框圆角效果
    text-align:center; //文本排列方式
    border-color:#DCDCDC; //边框颜色
    border: lgray solid thin;//边框样式

    }

    //声明按钮样式属性，达到凹凸效果
    input.ys{
    background-color:#2ECC71;//背景颜色
    color: #FFFFFF;//文字颜色
    border-radius: 6px;//圆角半径
    width:300px;
    height:45px;
    border-bottom:5px //底部边框
    solid #28BE68;    //边框是实线，设置颜色
    font-family:"宋体";  //设置字体
    font-size : 1.2em;   //字体大小
    }

    //鼠标悬浮于按钮上空改变颜色
    input.ys:hover{ 
    background-color:#55D88B; //改变颜色，高亮
    border-bottom:2px ;
    solid #28BE68;
    }
    </style>
    <title></title>
     </head>

    //<body>部分为页面可见部分
    <body bgcolor="#222222"> //背景颜色
    <div id="content">  //通过id可以找到对应的块的样式
      <div id="title">
        <h2>Open Agar</h2>  //标题
      </div>
      <div id="text">
        <input type="text"  placeholder="Enter your name here" class="testStyle" />  // placeholder设置hint,class表达样式
      </div>
      <br />
      <div id="btns">
       <input type="button" value="play" class="ys"></input>
      </div>
      <div id="btns">
        <input type="button" value="Spectate" class="ys" />
      </div>
      <div id="btns">
        <input type="button" value="Setting" class="ys" />
        <br />
      </div>
      <div>
        <h4>Gameplay</h4>

        //列表
        <ul style="font-size : 0.8em">
          <li>Move your mouse on the screen too move your character</li>
          <li>Eat food and other plysers in order to grow </br>your character(food respawns every time a players eats it)</li>
          <li>A player&#39;s mass is the number of food particles eaten.</li>
          <li>objective: Try to get fat and eat other players.</li>
        </ul>
      </div>
    </div>
    </body>
    </html>


主要设计思想：
灰黑色的背景有一个容器（框框），容器里面分成了几个块，分别定义每个块该有的属性。


早晨拿到这个界面也不知道从何下手，慢慢摸索还算是做出来了。继续努力!
