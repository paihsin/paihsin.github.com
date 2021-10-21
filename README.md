<!DOCTYPE html>
<html>
<head>
<title>personal_music.html</title>

<meta name="keywords" content="keyword1,keyword2,keyword3">
<meta name="description" content="this is my page">
<meta name="content-type" content="text/html; charset=UTF-8">

<!--<link rel="stylesheet" type="text/css" href="./styles.css">-->
<style type="text/css">
*{border:0;margin: 0;padding: 0}
body{
  background-image:url('image/element.jpg');
  background-size:cover;
}
label { 
    color:white; 
} 
/* div main */
.main{
  padding: 50px 0px 0px 30px;
}
/* bar  */
.musicBoxFooter a input[type='range']{
  -webkit-appearance: none;
  border-radius:20px;
  cursor: pointer;
  position: relative;
  top:-5px;
  width: 120px;
  background:url('music_img/track.png')  no-repeat;
  background-size:0% 100%;
}
/* bar roller */
.musicBoxFooter input[type='range']::-webkit-slider-thumb {
	-webkit-appearance: none;
}
/* bar  */
.musicBoxFooter a input[type='range']::-webkit-slider-runnable-track {
	height: 12px;
    border-radius: 10px; /*round coner*/
    box-shadow: 0 1px 1px #def3f8, inset 0 .125em .125em #0d1112; /*shadow*/
}
.musicBoxFooter input[type='range']:focus {
	outline: none;
}
.musicBoxFooter a input[type=range]::-webkit-slider-thumb {
    -webkit-appearance: none;
    height: 12px;
    width: 12px;
    margin-top: 0px; /*使滑块超出轨道部分的偏移量相等*/
    background: #ffffff; 
    border-radius: 50%; /*外观设置为圆形*/
    border: solid 0.125em rgba(205, 224, 230, 0.5); /*设置边框*/
    box-shadow: 0 .125em .125em #3b4547; /*添加底部阴影*/
    opacity:0.01;
}
/* musicbox */
.musicBox{
   width: 290px;
   height:144px;
   background-color: #404040;
   border-radius: 12px;
   box-shadow: 2px 2px black;
}

/* musicbox head */
.musicHeader{
   height: 40px;
   line-height: 60px;
   text-align: left;
   padding: 0px 20px;
}
.musicHeader button{
   display: inline-block;
   width: 25px;
   height:25px;
   outline: 0;
   cursor: pointer;
}
/* box top */
.boxAllshow{
   width: 130px;
   line-height: 20px;
   background-color: #36c;
   font:15px 'PMingLiU';
   color:#fff;
   border-radius: 5px;
   position:absolute;
   left:245px;
   top:45px;
}
.DonTLike{
   position:absolute;
   left:380px;top:60px;
   font:14px 'PMingLiU';
   width: 120px;
   height:30px;
   line-height: 30px;
   background-color: #36c;
   color:#fff;
   border-radius: 5px;
}

/* box body */
.musicBoxBody{
   height: 70px;
   padding: 0px 10px; 
}
.musicBoxBody img{
   border-radius: 70px;
   cursor: pointer;
}
.musicBoxBody div{
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    max-width: 160px;
   display: inline-block;
   color:white;
   font-family: 'PMingLiU';
   font-size:14px;
   margin-left: 15px;
   position: relative;
   top:-12px;
}
.musicBoxBody div p{
   display: block;
   height:16px;
   padding-left:15px;
   overflow: hidden;
}
/* box footer */
.musicBoxFooter{
   padding: 10px 0px 10px 10px;
   position: relative;
}
.musicBoxFooter button{
   display: inline-block;
   width: 20px;
   height:20px;
   background-color: #ccc;
   outline: 0;
   cursor: pointer;
}
/* sound range div */
.soundRange{
   position:relative;
   top:-58px;
   left:176px;
   
   width: 90px;
   height:20px;
   line-height:18px;
   background-color: #666;
   border-radius: 3px;
   transform: rotate(-90deg);
   -ms-transform: rotate(-90deg);		
   -webkit-transform: rotate(-90deg);
   -o-transform: rotate(-90deg);		
   -moz-transform: rotate(-90deg);
   z-index: 0;
}

/* sound range */
.soundRange input[type='range']{
   width:60px;
   margin-left:25px; 
   -webkit-appearance: none;
   border-radius:10px;
   cursor: pointer;
   background:url('music_img/track.png')  no-repeat;
   background-size:0% 100%;
}
.soundRange>input[type='range']::-webkit-slider-runnable-track {
	height: 10px;
    border-radius: 10px; 
    box-shadow: 0 1px 1px #def3f8, inset 0 .125em .125em #0d1112; 
}
/* -------------------volune silde---------------------- */
.soundRange input[type=range]::-webkit-slider-thumb {
    -webkit-appearance: none;
    height: 12px;
    width: 12px;
    margin-top: 0px; 
    background: #ffffff; 
    border-radius: 50%; 
    border: solid 0.125em rgba(205, 224, 230, 0.5); 
    box-shadow: 0 .125em .125em #3b4547; 
}

.musicBoxFooter p{
   position: absolute;
   top:-5px;
   right:0px;
   font:15px 'Microsoft JhengHei';
   background-color: #fff;
   border-radius: 3px;
}
/* collect box */
.collect{
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    max-width: 300px;
   width: 280px;
   height:340px;
   padding:10px 0px;
   background-color: #404040;
   border-radius: 12px;
   box-shadow: 1px 2px black;
   font:16px 'PMingLiU';
   overflow: auto;
}
.collect ul{
   list-style-type: none;
}
.collect ul li{
   height:30px;
   line-height: 30px;
   color:#22CF72;
   border-radius: 12px;
   cursor: pointer;
   overflow: hidden;
   border-bottom: 1px solid #88f; 
   transition:background 1s linear;
   }
.collect ul li img{
   position: relative;
   left:10px;
   top:3px;
   width: 15px;
   height:15px;
   cursor: pointer;
}
.collect ul li a{
   display: inline-block;
   width: 150px;
   padding-left: 20px;
}
.collect ul li:HOVER {
	background-color: #B6C6D5;
	color:#a11;
}
/* show ch music */
.allShow{
   padding:10px 0px;
   position:absolute;
   right:670px;
   top:50px;
   width: 300px;
   height:483px;
   background-color: #404040;
   border-radius: 5px;
   box-shadow: 1px 2px black;
   font:16px 'PMingLiU';
   overflow: auto;
}
.allShow ul{
   list-style-type: none;
}

.allShow ul li{
   height:30px;
   line-height: 30px;
   color:#22CF72;
   border-radius: 12px;
   cursor: pointer;
   overflow: hidden;
   border-bottom: 1px solid #88f; 
   transition:background 1s linear;
   }
.allShow ul li a{
   display: inline-block;
   width: 160px;
   padding-left: 10px;
}
.allShow ul li i{
   margin-left: 15px;
}
.allShow ul li:HOVER {
	background-color: #B6C6D5;
	color:#a11;
}
	/*all show en*/

.allShowen{
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    max-width: 300px;
   padding:10px 0px;
   position:absolute;
   right:350px;
   top:50px;
   width: 300px;
   height:483px;
   background-color: #404040;
   border-radius: 5px;
   box-shadow: 1px 2px black;
   font:16px 'PMingLiU';
   overflow: auto;
}

.allShowen ul{
   list-style-type: none;
}

.allShowen ul li{
   height:30px;
   line-height: 30px;
   color:#22CF72;
   border-radius: 12px;
   cursor: pointer;
   overflow: hidden;
   border-bottom: 1px solid #88f; 
   transition:background 1s linear;
   }
.allShowen ul li a{
   display: inline-block;
   width: 160px;
   padding-left: 10px;
}
.allShowen ul li i{
   margin-left: 15px;
}
.allShowen ul li:HOVER {
	background-color: #B6C6D5;
	color:#a11;
}
/**/
	/*all show jp*/

.allShowjp{
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    max-width: 300px;
   padding:10px 0px;
   position:absolute;
   right:10px;
   top:50px;
   width: 320px;
   height:483px;
   background-color: #404040;
   border-radius: 5px;
   box-shadow: 1px 2px black;
   font:16px 'PMingLiU';
   overflow: auto;
}

.allShowjp ul{
   list-style-type: none;
}

.allShowjp ul li{
   height:30px;
   line-height: 30px;
   color:#22CF72;
   border-radius: 12px;
   cursor: pointer;
   overflow: hidden;
   border-bottom: 1px solid #88f; 
   transition:background 1s linear;
   }
.allShowjp ul li a{
   display: inline-block;
   width: 180px;
   padding-left: 10px;
}
.allShowjp ul li i{
   margin-left: 15px;
}
.allShowjp ul li:HOVER {
	background-color: #B6C6D5;
	color:#a11;
}

/* 滚动条样式 */
/* 设置滚动条的样式 */
::-webkit-scrollbar {
    width: 12px;
}
/* 滚动槽 */
::-webkit-scrollbar-track {
    -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
    border-radius: 10px;
    overflow: hidden;
}
/* 滚动条滑块 */
::-webkit-scrollbar-thumb {
    border-radius: 20px;
    background: rgba(255,227,132,0.5);
    -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.5);
}
::-webkit-scrollbar-thumb:window-inactive {
    background: rgba(255,0,0,0.4);
}
</style>
<script type="text/javascript" src="jQuery/jquery-1.6.4.min.js"></script>
<script type="text/javascript">
   $(function(){
      var musicList=["你的行李.mp3","飛鳥與蟬.mp3","星辰大海.mp3","四季予你.mp3","天黑請閉眼.mp3","太空人.mp3","不為誰而作的歌.mp3","你,好不好.mp3","晚安晚安.mp3","句號.mp3","歌頌者.mp3","我很好騙.mp3","家家酒.mp3","巴別塔慶典.mp3","年輪說.mp3","怎麼了.mp3","愛人錯過.mp3","愛情怎麼了嗎.mp3","我好嗎.mp3","歌頌者.mp3","炙愛.mp3","煙幕.mp3","直到我遇見了你.mp3","說好不哭.mp3","路過人間.mp3","連名帶姓.mp3","摩天動物園.mp3","魚仔.mp3","葉子.mp3","寂寞邊界.mp3"];
      var musicStar=["謝震廷","任然","黃霄雲","程響","顏志琳","吳青峰","林俊傑","周興哲","魏如萱","鄧紫棋","吳青峰","動力火車","家家","吳青峰","楊丞琳","周興哲","告五人","盧廣仲","梁靜茹","吳青峰","陳昕玥","陳昕玥","陳友廷","周杰倫","郁可唯","張惠妹","鄧紫棋","盧廣仲","阿桑","張棟樑"]
      var musicListen=["Forever After All.mp3","Cardigan.mp3","Memories.mp3","Shallow.mp3","YOU&I.mp3","Lost Cause.mp3","bad guy.mp3","lovely.mp3","Breathless.mp3","How Far I'll Go.mp3","Speechless.mp3","Flashlight.mp3","Skyscraper.mp3","Firework.mp3","Titanium.mp3","I Wrote a Song Using Only Hate Comments 2.mp3","Peaches.mp3","Hold On.mp3","Yummy.mp3","Lonely.mp3","Intentions.mp3","Purpose.mp3"];
      var musicStaren=["Luke Combs","Taylor Swift","Maroon 5","Lady Gaga,Bradley Cooper","J.R.A","Billie Eilish","Billie Eilish","Billie Eilish,Khalid","Shayne Ward","Alessia Cara","Naomi Scott","Jessie J","Demi Lovato","Madilyn Bailey","Madilyn Bailey","Madilyn Bailey","Justin Bieber","Justin Bieber","Justin Bieber","Justin Bieber","Justin Bieber","Justin Bieber"];
	  var musicListjp=["us.mp3","Prover.mp3","Who I Am.mp3","Tell me.mp3","Drown.mp3","The Love We've Made.mp3","夜に駆ける.mp3","群青.mp3","怪物.mp3","シャルル.mp3","蝶々結び.mp3","Ref rain.mp3","Rokutouseino Yoru.mp3","さよならの今日に.mp3","Remember the Days We're Talking Rubbish in the Twilight.mp3","貓.mp3"];
      var musicStarjp=["Milet","Milet","Milet","Milet","Milet","Milet","YOASOBI","YOASOBI","YOASOBI","バルーン","Aimer","Aimer","Aimer","Aimyon","Aimyon","DISH"];
	  var totallist=[musicList,musicListen,musicListjp];
	  var totalstarlist=[musicStar,musicStaren,musicStarjp];
	  var myAudio=document.getElementById("myAudio");
      myAudio.volume=document.getElementById("soundRange").value/100;
      var nowMusicNum=0;
	  var totalNum=29;
	  var totalNumen=21;
	  var totalNumjp=15;
      //default play first song 
      $("#myAudio source").attr("src","music/"+(musicList[nowMusicNum])+"");
      //display song info
      $(".musicInfo p:eq(0)").text(musicList[nowMusicNum]);/* 歌曲信息 */
      $(".musicInfo p:eq(1)").text(musicStar[nowMusicNum]);/* 歌手信息 */
	  //$(".listPlay").trigger("click");
	  randomTime1=setInterval(function(){
             if(myAudio.currentTime==myAudio.duration){
                 $(".musicNext2").trigger("click");
               }
            },100); 
	  $(".listtype").change(function() {
	  myAudio.pause();
         $(".musicStop").hide();
         $(".musicPlay").show();
	  	  var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype=="ch")
		{
		nowMusicNum=0;
		      //default play first song 
		$("#myAudio source").attr("src","music/"+(musicList[nowMusicNum])+"");
		//display song info
		$(".musicInfo p:eq(0)").text(musicList[nowMusicNum]);/* 歌曲信息 */
		$(".musicInfo p:eq(1)").text(musicStar[nowMusicNum]);/* 歌手信息 */
		myAudio.load()
		}
		if(listtype=="en")
		{
		nowMusicNum=0;
		      //default play first song 
		$("#myAudio source").attr("src","music/"+(musicListen[nowMusicNum])+"");
		//display song info
		$(".musicInfo p:eq(0)").text(musicListen[nowMusicNum]);/* 歌曲信息 */
		$(".musicInfo p:eq(1)").text(musicStaren[nowMusicNum]);/* 歌手信息 */
		myAudio.load();
		}
	  	if(listtype=="jp")
		{
		nowMusicNum=0;
		      //default play first song 
		$("#myAudio source").attr("src","music/"+(musicListjp[nowMusicNum])+"");
		//display song info
		$(".musicInfo p:eq(0)").text(musicListjp[nowMusicNum]);/* 歌曲信息 */
		$(".musicInfo p:eq(1)").text(musicStarjp[nowMusicNum]);/* 歌手信息 */
		myAudio.load()
		}
		if(listtype=="self")
		{
         var listLi=$(".collect ul li").length;
         nowMusicNum=0;
         if(listLi==0){/* no收藏 */
		 alert("收藏為空");
		 nameElement.value="ch";
		$("#myAudio source").attr("src","music/"+(musicList[nowMusicNum])+"");
		//display song info
		$(".musicInfo p:eq(0)").text(musicList[nowMusicNum]);/* 歌曲信息 */
		$(".musicInfo p:eq(1)").text(musicStar[nowMusicNum]);/* 歌手信息 */
		myAudio.load()
         }else{

               var musicSrc=$(".collect ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowListliNum).children("span").text())
               myAudio.load();
         } 
		}
		});
	     /* click play button */
      $(".musicPlay").click(function(){
         $(this).hide();
         $(".musicStop").show();
         myAudio.play();
         /* ------------------同步進度條-------------------- */
         setInterval(function(){
             var myAudio=document.getElementById("myAudio");   //
             var musicRange=document.getElementById("musicRange");  //進度條
             var ValueTime=(myAudio.currentTime/myAudio.duration)*100;
             document.getElementById("musicRange").value=ValueTime;
             musicRange.style.backgroundSize=ValueTime+"% 100%";},1000); 
      });
      $(".musicStop").click(function(){
         $(this).hide();
         $(".musicPlay").show();
         myAudio.pause();
      });
      
      /* 按上一首 */
      $(".musicPrev").click(function(){
         nowMusicNum--;
         
         if(nowMusicNum<0){
         nowMusicNum=totalNum;
         }
         $("#myAudio source").attr("src","music/"+(musicList[nowMusicNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicList[nowMusicNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStar[nowMusicNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
      });
      //random按上一首
      $(".musicPrev2").click(function(){
         var randomNum=Math.random();
		var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype =="ch")
		{
         var randomMusicNum=randomNum*musicList.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicList[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicList[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStar[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="en")
		{
         var randomMusicNum=randomNum*musicListen.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicListen[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListen[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStaren[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="jp")
		{
         var randomMusicNum=randomNum*musicListjp.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicListjp[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListjp[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStarjp[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="self")
		{
		 var listLi=$(".collect ul li").length;
         var randomMusicNum=randomNum*listLi;
         var nowPlayNum=Math.floor(randomMusicNum);
          var musicSrc=$(".collect ul li").eq(nowPlayNum).children("a").text();
         $("#myAudio source").attr("src","music/"+musicSrc+"");
               
          $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowPlayNum).children("a").text())
         $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowPlayNum).children("span").text())
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
      });
      /* 列表循環下的上一首 */
      
      var nowListliNum=0;
      $(".musicPrev3").click(function(){
		nowListliNum--;
	    var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype =="self")
		{
         var listLi=$(".collect ul li").length;
         if(listLi==0){/* no收藏 */
			alert("收藏為空")
         }else{
            if(nowListliNum<=-1){
               nowListliNum=listLi-1;
               }
               var musicSrc=$(".collect ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowListliNum).children("span").text())
         }
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="cn")
		{
            if(nowListliNum<=-1){
               nowListliNum=totalNum;
               }
         
         $("#myAudio source").attr("src","music/"+(musicList[nowListliNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicList[nowListliNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStar[nowListliNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="en")
		{
            if(nowListliNum<=-1){
               nowListliNum=totalNumen;
               }
         
         $("#myAudio source").attr("src","music/"+(musicListen[nowListliNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListen[nowListliNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStaren[nowListliNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="jp")
		{
            if(nowListliNum<=-1){
               nowListliNum=totalNumjp;
               }
         
         $("#myAudio source").attr("src","music/"+(musicListjp[nowListliNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListjp[nowListliNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStarjp[nowListliNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
      });
      
      /* click下一首按紐 */
      $(".musicNext").click(function(){
         nowMusicNum++;
         var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype =="ch")
		{
         if(nowMusicNum>totalNum){
         nowMusicNum=0;
         }
         
         $("#myAudio source").attr("src","music/"+(musicList[nowMusicNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicList[nowMusicNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStar[nowMusicNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		 if(listtype =="en")
		{
         if(nowMusicNum>totalNumen){
         nowMusicNum=0;
         }
         
         $("#myAudio source").attr("src","music/"+(musicListen[nowMusicNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListen[nowMusicNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStaren[nowMusicNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="jp")
		{
         if(nowMusicNum>totalNumjp){
         nowMusicNum=0;
         }
         
         $("#myAudio source").attr("src","music/"+(musicListjp[nowMusicNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListjp[nowMusicNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStarjp[nowMusicNum]);/* 歌手信息 */
         
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="self")////
		{
		var listLi=$(".collect ul li").length;
         if(nowMusicNum>listLi){
         nowMusicNum=0;
         }
          var musicSrc=$(".collect ul li").eq(nowMusicNum).children("a").text();
         $("#myAudio source").attr("src","music/"+musicSrc+"");
               
          $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowMusicNum).children("a").text())
         $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowMusicNum).children("span").text())
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
      });
      //random next
      
      $(".musicNext2").click(function(){
         var randomNum=Math.random();
		var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype =="ch")
		{
         var randomMusicNum=randomNum*musicList.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicList[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicList[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStar[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="en")
		{
         var randomMusicNum=randomNum*musicListen.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicListen[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListen[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStaren[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="jp")
		{
         var randomMusicNum=randomNum*musicListjp.length;
         var nowPlayNum=Math.floor(randomMusicNum);
         $("#myAudio source").attr("src","music/"+(musicListjp[nowPlayNum])+"");/* 歌曲链接 */
         $(".musicInfo p:eq(0)").text(musicListjp[nowPlayNum]);/* 歌曲信息 */
         $(".musicInfo p:eq(1)").text(musicStarjp[nowPlayNum]);/* 歌手信息 */      
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
		if(listtype =="self")
		{
		 var listLi=$(".collect ul li").length;
         var randomMusicNum=randomNum*listLi;
         var nowPlayNum=Math.floor(randomMusicNum);
          var musicSrc=$(".collect ul li").eq(nowPlayNum).children("a").text();
         $("#myAudio source").attr("src","music/"+musicSrc+"");
               
          $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowPlayNum).children("a").text())
         $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowPlayNum).children("span").text())
         myAudio.load();
         $(".musicPlay").trigger("click");
		 }
      });
      
      //list next
      $(".musicNext3").click(function(){
	  var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
		if(listtype =="self")
		{
         var listLi=$(".collect ul li").length;
         nowListliNum++;
         if(listLi==0){/* no收藏 */
		 alert("收藏為空")
         }else{
            if(nowListliNum>=listLi){
               nowListliNum=0;
               }
               var musicSrc=$(".collect ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".collect ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".collect ul li").eq(nowListliNum).children("span").text())
               myAudio.load();
               $(".musicPlay").trigger("click");
         } 
		 }
		 if(listtype =="ch")
		{
         var listLi=$(".allShow ul li").length;
         nowListliNum++;
         if(listLi==0){/* no收藏 */
		 alert("收藏為空")
         }else{
            if(nowListliNum>=listLi){
               nowListliNum=0;
               }
               var musicSrc=$(".allShow ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".allShow ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".allShow ul li").eq(nowListliNum).children("span").text())
               myAudio.load();
               $(".musicPlay").trigger("click");
         } 
		 }
		 		 if(listtype =="en")
		{
         var listLi=$(".allShowen ul li").length;
         nowListliNum++;
         if(listLi==0){/* no收藏 */
		 alert("收藏為空")
         }else{
            if(nowListliNum>=listLi){
               nowListliNum=0;
               }
               var musicSrc=$(".allShowen ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".allShowen ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".allShowen ul li").eq(nowListliNum).children("span").text())
               myAudio.load();
               $(".musicPlay").trigger("click");
         } 
		 }
		 if(listtype =="jp")
		{
         var listLi=$(".allShowjp ul li").length;
         nowListliNum++;
         if(listLi==0){/* no收藏 */
		 alert("收藏為空")
         }else{
            if(nowListliNum>=listLi){
               nowListliNum=0;
               }
               var musicSrc=$(".allShowjp ul li").eq(nowListliNum).children("a").text();
               $("#myAudio source").attr("src","music/"+musicSrc+"");
               
               $(".musicInfo p:eq(0)").text($(".allShowjp ul li").eq(nowListliNum).children("a").text())
               $(".musicInfo p:eq(1)").text($(".allShowjp ul li").eq(nowListliNum).children("span").text())
               myAudio.load();
               $(".musicPlay").trigger("click");
         } 
		 }
      });
      
         /* 点击音量切换到静音 */
         $(".musicSound").click(function(){
            $(this).hide()
            $(".musicMute").show();
            myAudio.muted=true;
            document.getElementById("soundRange").value=0;
            myAudio.volume=0;
         })
         /* 点击静音切换到音量 */
         $(".musicMute").click(function(){
            $(this).hide()
            $(".musicSound").show();
            myAudio.muted=false;
            document.getElementById("soundRange").value=40;
            myAudio.volume=0.4;
         })
         /* 鼠标悬浮在音量图标上时显示音量条 */
         $(".musicMute,.musicSound,.soundRange").hover(function(){
            $(".soundRange").toggle();
         })
         
         /* 改变音量 */
         $(".soundRange input[type='range']").mousemove(function(){
             myAudio.volume=document.getElementById("soundRange").value/100;
             if(myAudio.volume==0){
                $(".musicSound").hide();
                $(".musicMute").show();
             }else{
                $(".musicSound").show();
                $(".musicMute").hide();
             }
         });
         /* 在静音下改变音量后变为非静音状态 */
         $(".soundRange input[type='range']").change(function(){
             myAudio.muted=false;
         })
         
         /* 收藏音乐 */
         $(".likeThis").click(function(){
             //$(".musicInfo p:eq(0)").text()   //歌曲信息
             //$(".musicInfo p:eq(1)").text()   //歌手信息
             $(".collect").fadeIn(1000);
             if(window.confirm("確定收藏?")){
                  $(".collect ul").append("<li><img src='musicBox/remove.png'><a>"+$(".musicInfo p:eq(0)").text()+"</a><span>"+$(".musicInfo p:eq(1)").text()+"</span></li>");        
             }else{
                  $(".DonTLike").animate({"opacity":"1"},400).delay(1500).animate({"opacity":"0"},400);
             }
         });
         //显示是否删除收藏夹音乐提示
         $(".likeThis").hover(function(){
            $(".boxAllshow").text("收藏正在播放music").toggle();
         })
         /* 删除此音乐 */
         $(".collect ul li img").live('click',function(){
            if(window.confirm("確定刪除?")){
                $(this).parent().remove();
            }
         })
         //是否删除所有收藏
         $(".removeAll").click(function(){
            if(window.confirm("清空收藏?")){
                $(".collect ul").empty();
                $(".collect").fadeOut(1000);
            }
         })
         //show是否删除收藏
         $(".removeAll").hover(function(){
            $(".boxAllshow").text("刪除收藏").toggle();
         })
         /* 收藏list click play */
         $(".collect ul li").live('click',function(){
		 var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
			nameElement.value="self";
            var musicSrc=$(this).children("a").text();
            $("#myAudio source").attr("src","music/"+musicSrc+"");
            
            $(".musicInfo p:eq(0)").text($(this).children("a").text())
            $(".musicInfo p:eq(1)").text($(this).children("span").text())
            
            myAudio.load();
            $(".musicPlay").trigger("click");
         });
         /* 点击显示全部音乐时 */
         $(".allMusicShow").toggle(function(){
            $(".allShow").fadeIn(1000);
         },function(){
            $(".allShow").fadeOut(1000);
         })
	 $(".allMusicShowen").toggle(function(){
            $(".allShowen").fadeIn(1000);
         },function(){
            $(".allShowen").fadeOut(1000);
         })
		 	 $(".allMusicShowjp").toggle(function(){
            $(".allShowjp").fadeIn(1000);
         },function(){
            $(".allShowjp").fadeOut(1000);
         })
         //mouse hover show
         $(".allMusicShow").hover(function(){
            $(".boxAllshow").text("顯示中文歌庫").toggle();
         })
		 $(".allMusicShowen").hover(function(){
            $(".boxAllshow").text("顯示英文歌庫").toggle();
         })
	   		 $(".allMusicShowjp").hover(function(){
            $(".boxAllshow").text("顯示日文歌庫").toggle();
         })
         /* click show ch list */
         $(".allShow ul li").live('click',function(){
		 		var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
			nameElement.value="ch";
            var musicSrc=$(this).children("a").text();
			nowListliNum=musicList.indexOf(musicSrc);
            $("#myAudio source").attr("src","music/"+musicSrc+"");
            
            $(".musicInfo p:eq(0)").text($(this).children("a").text())
            $(".musicInfo p:eq(1)").text($(this).children("span").text())
            
            myAudio.load();
            $(".musicPlay").trigger("click");
         });
		 /* click all en list to play */
		$(".allShowen ul li").live('click',function(){
				 		var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
			nameElement.value="en";
            var musicSrc=$(this).children("a").text();
			nowListliNum=musicListen.indexOf(musicSrc);
            $("#myAudio source").attr("src","music/"+musicSrc+"");           
            $(".musicInfo p:eq(0)").text($(this).children("a").text())
            $(".musicInfo p:eq(1)").text($(this).children("span").text())
            myAudio.load();
            $(".musicPlay").trigger("click");
         });
		 		 /* click all jp list to play */
		$(".allShowjp ul li").live('click',function(){
				 		var nameElement = document.getElementById("listtype");
		var listtype = nameElement.value;
			nameElement.value="jp";
            var musicSrc=$(this).children("a").text();
			nowListliNum=musicListjp.indexOf(musicSrc);
            $("#myAudio source").attr("src","music/"+musicSrc+"");           
            $(".musicInfo p:eq(0)").text($(this).children("a").text())
            $(".musicInfo p:eq(1)").text($(this).children("span").text())
            myAudio.load();
            $(".musicPlay").trigger("click");
         });
         for(var i=0;i<totalNum+1;i++){
                (function(k){
                    $(".allShow ul").append("<li><i>"+(i+1)+".</i><a>"+totallist[0][i]+"</a><span>"+totalstarlist[0][i]+"</span>")
                })(i)
            }
		for(var i=0;i<totalNumen+1;i++){
                (function(k){
                    $(".allShowen ul").append("<li><i>"+(i+1)+".</i><a>"+totallist[1][i]+"</a><span>"+totalstarlist[1][i]+"</span>")
                })(i)
            }
		for(var i=0;i<totalNumjp+1;i++){
                (function(k){
                    $(".allShowjp ul").append("<li><i>"+(i+1)+".</i><a>"+totallist[2][i]+"</a><span>"+totalstarlist[2][i]+"</span>")
                })(i)
            }
			var randomTime1,listTime;
/*------------ 点击随机播放    切换到    单曲循环     以及悬浮显示的提醒   ---------------*/
         $(".randomPlay").click(function(){//inTurn
            $(".MusicPlayStyle").hide().eq(1).show();
            $(".randomP").show();       //将数组中的歌曲   随机取得数据然后  单曲循环  播放
            $(".inTurn").hide();          
            $(".listP").hide();
            //清除随机播放切换到下一首的定时器
            clearInterval(randomTime1);
            //给音乐播放器添加loop属性   使其单曲循环
            $("#myAudio").attr("loop","loop");
         })
         $(".randomPlay").hover(function(){
            $(".musicBoxFooter p").text("Random play").toggle();
         })
-/* ----------点击单曲循环  切换到  列表循环   以及悬浮显示的提醒 ------------*/
         $(".onlyOnePlay").click(function(){//listP
            $(".MusicPlayStyle").hide().eq(2).show();
            $(".randomP").hide();
            $(".inTurn").hide();
            $(".listP").show();         //将收藏夹中的的歌曲   循环  播放
            //切换到列表循环时要去除loop属性,不让其单曲循环
            $("#myAudio").removeAttr("loop");
            //添加定时器,按照列表循环播放
            listTime=setInterval(function(){
             if(myAudio.currentTime==myAudio.duration){
                 $(".musicNext3").trigger("click");
             }
             },100);
         })
         $(".onlyOnePlay").hover(function(){
            $(".musicBoxFooter p").text("Single cycle").toggle();
         })
/*----------- 点击列表循环  切换到  顺序播放   以及悬浮显示的提醒 ----------*/
         $(".listPlay").click(function(){//inTurn
            $(".MusicPlayStyle").hide().eq(0).show();
            $(".randomP").show();      //将数组中的歌曲  取得数据然后  循环  播放
            $(".inTurn").hide();
            $(".listP").hide();
            //清除列表循环的定时器  下一首
            clearInterval(listTime);
            
            /* 顺序播放的定时器 */
            randomTime1=setInterval(function(){
             if(myAudio.currentTime==myAudio.duration){
                 $(".musicNext2").trigger("click");
               }
            },100); 
         })
         $(".listPlay").hover(function(){
            $(".musicBoxFooter p").text("list cycle").toggle();
         })
		 $(".musicBoxBody img").hover(function(){
            $(".boxAllshow").text("Show/Hide 收藏list").toggle();
         })

 	    $(".musicBoxBody img").click(function(){
			if($(".collect").is(":hidden")){
                $(".collect").fadeIn(1000);
            }else{
                $(".collect").fadeOut(500);
            }
         });
    })

    
    /* ------------------同步進度-------------------- */ 
     function nowPlay(){
        var musicRange=document.getElementById("musicRange");
        musicRange.style.backgroundSize=musicRange.value+"% 100%";
        myAudio.currentTime=musicRange.value*myAudio.duration/100;
     }
</script>
</head>

	<div class="main">
		<!-- 存放播放器 -->
		<div>
			<audio id="myAudio">
			   <source>
			</audio>
		</div>
		<div class="musicBox" style="opacity:0.9;">
		     <div class="musicHeader">
		          <div class="boxAllshow" style="display: none;white-space: nowrap;">
		                                            
		          </div>
				
  <label for="playlisttype">play list</label>
  <select class="listtype" id="listtype">
    <option value="ch">中文</option>
    <option value="en">英文</option>
    <option value="jp">日文</option>
    <option value="self">收藏</option>
  </select>


		          <button class="allMusicShow" style="background:url('musicBox/send.png') center no-repeat;"></button>
				  <button class="allMusicShowen" style="background:url('musicBox/send2.png') center no-repeat;"></button>
				  <button class="allMusicShowjp" style="background:url('musicBox/send3.png') center no-repeat;"></button>
				  <button class="removeAll" style="background: url('musicBox/remove.png') center no-repeat;"></button>
		          <button class="likeThis" style="background:url('musicBox/like.png') center no-repeat;"></button>
		          <div class="DonTLike" style="opacity:0;z-index: 10;">
		                                              已取消該收藏...
		          </div>
		     </div>
		     <div class="musicBoxBody">
		          <img src="musicBox/personal.png" width="70px" height="70px">
		          <div class="musicInfo">
		                                         歌曲信息:
		              <p style="background: url('musicBox/musicInfo.png') 0px 3px no-repeat;cursor: default;"></p>
		              <p style="background: url('musicBox/musicStar.png') 0px 3px no-repeat;cursor: default;"></p>
		          </div>
		     </div>
		     <div class="musicBoxFooter">
		         <!-- 数组顺序 --><button class="inTurn musicPrev" style="display:none;background: url('musicBox/musicPrev.png') center no-repeat;"></button>
		         <!-- 列表顺序 --><button class="listP musicPrev3" style="display:none;background: url('musicBox/musicPrev.png') center no-repeat;"></button>
		         <!-- 数组随机 --><button class="randomP musicPrev2" style="background: url('musicBox/musicPrev.png') center no-repeat;"></button>
		               <button class="musicStop" style="background: url('musicBox/musicStop.png') center no-repeat;display: none;"></button>
		               <button class="musicPlay" style="background: url('musicBox/musicPlay.png') center no-repeat;"></button>
		         <!-- 数组顺序 --><button class="inTurn musicNext" style="display:none;background: url('musicBox/musicNext.png') center no-repeat;"></button>
		         <!-- 列表顺序 --><button class="listP musicNext3" style="display:none;background: url('musicBox/musicNext.png') center no-repeat;"></button>
		         <!-- 数组随机--><button class="randomP musicNext2" style="background: url('musicBox/musicNext.png') center no-repeat;"></button>
		               	
		               <a style="height:10px;border-radius:10px;background-color: #fff;display: inline-block;"><input id="musicRange" type="range" onchange="nowPlay()"></a>
		               
		               <button class="musicSound" style="position:relative;z-index:2;background: url('musicBox/musicSound.png') center no-repeat;"></button>
		               <button class="musicMute" style="position:relative;z-index:2;background: url('musicBox/musicMute.png') center no-repeat;display: none;"></button> 
		               <button class="MusicPlayStyle randomPlay" style="background: url('musicBox/随机播放.png') center no-repeat;"></button>
		               <button class="MusicPlayStyle onlyOnePlay" style="background: url('musicBox/单曲循环.png') center no-repeat;display: none;"></button>
		               <button class="MusicPlayStyle listPlay" style="background: url('musicBox/列表循环.png') center no-repeat;display: none;"></button>
		               <button class="MusicPlayStyle orderPlay" style="background: url('musicBox/顺序播放.png') center no-repeat;display: none;"></button>
		               <p style="display: none;"></p>
		               <div class="soundRange" style="display: none">
		                    <input type="range" id="soundRange">
		               </div>
		     </div>
		</div>
		<div class="collect" style="display: none;">
		    <ul>
		        
		    </ul>
		</div>
		<div class="allShow" style="display: none;">
		   <ul>
		      
		   </ul>
		</div>
			<div class="allShowen"style="display: none;">
		   <ul>
		      
		   </ul>
		</div>
					<div class="allShowjp"style="display: none;">
		   <ul>
		      
		   </ul>
		</div>
	</div>
</body>
</html>
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
