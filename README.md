<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0,maximum-scale=1.0, user-scalable=no,viewport-fit=cover" />
		<title></title>
		<style>
			*{padding: 0;margin: 0;border: 0px;box-sizing: border-box;}
			body{font-family: "microsoft yahei";font-size: 14px;line-height: 1.3;color: #333;}
			ul,li{list-style: none;}
			a{text-decoration: none;}
			
			.header{padding-top: 30px;padding-bottom: 30px;background: #7ddf6c;position: relative;}
			.header .menu{display: none;}
			.header ul{display: flex;border: 1px solid red;width: 45%;justify-content: space-around;}
			.header ul li a{font-size: 20px;color: #fff;transition: color 0.5s;}
			.header ul li a:hover{color: #000;transition: color 0.5s;}
			.header ul li:first-child a{color: #000;}
			.header .logo{position: absolute;right: 10%;top: 0;border: 1px solid red;z-index: 2;}
			.header .logo img{width: 100%;height: auto;}
	
			.banner{width: 100%;min-height: 680px;background: url(img/banner.jpg) no-repeat;border: 1px solid red;background-size: cover;position: relative;}
			.banner .banner-intro{width: 30%;padding: 30px;background: rgba(255, 255, 255, 0.7);position: absolute;right: 20px;bottom: 30%;}
			.banner .banner-intro h3{font-size: 16px;color: #159400;font-family: 'Droid Serif', serif;}
			.banner .banner-intro p{font-size: 16px;line-height: 1.4;padding-top: 16px;padding-bottom: 30px;}
			.banner .banner-intro a{background: #159400;color: #fff;padding: 7px 15px;transition: background 0.5s;}
			.banner .banner-intro a:hover{background: #6cd79c;}
			
			.main{background-color:#FFFDD2 ;padding:80px 0 ;}
			.main h3{text-align: center;color: #159400;font-size: 28px;font-weight: normal;letter-spacing: 2px;margin-bottom: 20px;}
			.main .main-content{display: flex;}
			.main .main-content>div{width: 50%;border: 1px solid green;}
			.main .main-content>div:nth-child(1){margin-right: 50px;}
			.main .main-content>div:nth-child(1) img{width: 100%;height: auto;display: block;}
			.main .main-content .main-content-text .mission{display: flex;justify-content: space-around;margin-bottom: 18px;}
			.main .main-content .main-content-text .mission .mission-pic{width: 15%;;border: 1px solid green;}
			.main .main-content .main-content-text .mission .mission-pic img{width: 100%;}
			.main .main-content .main-content-text .mission .mission-text{width: 80%;border: 1px solid red;}
			.main .main-content .main-content-text .mission .mission-text .mission-title{font-size: 26px;color: #7ddf6c}
			.main .main-content .main-content-text .mission .mission-text p{font-size: 16px;margin-top: 16px;}
			
			.footer{font-size: 14px;padding: 18px 0;color: #fff;background-color: #7ddf6c;text-align: center;}
			
			
			@media screen and (max-width:1200px) {
					.banner{min-height: 460px;}
					.banner .banner-intro{width: 40%;bottom: 20%;padding: 20px;}	
			}
			
			@media screen and (max-width:992px) {
				.header ul{width: 60%;}
				.header ul li a{font-size: 18px;}
				.header .logo{width: 15%;}
				.banner .banner-intro{width: 40%;bottom: 20%;/* padding: 20px; */}	
			}
			
			@media screen and (max-width:768px) {
				.header ul{width: 70%;}
				.header ul li a{font-size: 16px;}
				.header .logo{width: 15%;}	
				.banner .banner-intro{width: 50%;bottom: 20%;padding: 20px;}
				.main .main-content .main-content-text .mission .mission-text .mission-title{font-size: 22px;}
				.main .main-content .main-content-text .mission .mission-text p{font-size: 13px;margin-top: 10px;}
			}
			
			@media screen and (max-width:640px) {
				.header ul{display: none;}
				.header .menu{display: block;position: absolute;top: 15px;left: 20px;}
				.header .logo{width: 15%;}	
				.banner .banner-intro{width: 55%;bottom: 20%;padding: 15px;}
				.banner .banner-intro p{font-size: 13px;padding-top: 10px;padding-bottom: 20px;}
				
				.main{padding: 30px 0;}
				.main .main-content{flex-direction: column;}
				.main .main-content>div{width: 100%;}
				.main h3{font-size: 28px;}
				.main .main-content>div:nth-child(1){margin-bottom: 20px;}
				.main .main-content .main-content-text .mission .mission-text .mission-title{font-size: 20px;}
				.main .main-content .main-content-text .mission .mission-text p{margin-top: 8px;}
			}
		</style>
	</head>
	<body>
		<div class="header">
			<img src="img/menu.png" class="menu"/>
			<ul>
				<li><a href="">首页</a></li>
				<li><a href="">全球问题</a></li>
				<li><a href="">解决方案</a></li>
				<li><a href="">关于我们</a></li>
				<li><a href="">联系我们</a></li>
			</ul>
			<div class="logo">
				<img src="img/logo.png">
			</div>
			
		</div>
		<div class="banner">
			<div class="banner-intro">
				<h3>爱护需要行动</h3>
				<p>爱护森林吧！行动起来吧！蛮砍乱伐森林是人类的愚蠢行为，再不要做这种危害子孙后代的事了。我们一定要保护好现有的森林资源！谨防森林火灾再次发生！</p>
				<a href="">了解更多</a>
			</div>
		</div>
		
		<div class="main">
			<h3>我们的使命</h3>
			<div class="main-content">
				<div class="main-content-pic">
					<img src="img/mission_img.jpg"/>
				</div>
				<div class="main-content-text">
					<div class="mission">
						<div class="mission-pic">
							<img src="img/i1.gif"/>
						</div>
						<div class="mission-text">
							<div class="mission-title">治理污染</div>
							<p>将环境保护纳入国民经济与社会发展计划和年度计划，在经济发展 中防治环境污染和生态破坏。</p>
						</div>
					</div>
					<div class="mission">
						<div class="mission-pic">
							<img src="img/i2.gif"/>
						</div>
						<div class="mission-text">
							<div class="mission-title">垃圾分类</div>
							<p>关心垃圾分类，特别是可回收垃圾，进行回收再生，减少对森林树木的采集砍伐</p>
						</div>
					</div>
					<div class="mission">
						<div class="mission-pic">
							<img src="img/i3.gif"/>
						</div>
						<div class="mission-text">
							<div class="mission-title">节能低碳</div>
							<p>开始低碳生活吧，节能减排，减少对资源的浪费，并还自己一片蓝天！</p>
						</div>
					</div>
				</div>
			</div>
			
		</div>
		
		<div class="footer">
			&copy; 2016 itcast. All Rights Reserved | Design by 传智播客
		</div>
	</body>
</html>
