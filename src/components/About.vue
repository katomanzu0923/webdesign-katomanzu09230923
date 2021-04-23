<template>
	<div>
		<img class="mainimg" :src="mainImg">
		<p class="non">My Profile</p>
		<div class="ly">
			<div class="bl">
				<div @click="change(0)" :class="[tab==1? 'a':'b']">学生時代</div>
				<div @click="change(1)" :class="[tab==2? 'a':'b']">大学院時代</div>
				<div @click="change(2)" :class="[tab==3? 'a':'b']">新卒就活</div>
				<div @click="change(3)" :class="[tab==4? 'a':'b']">現在</div>
			</div>
			<div v-if="tab == 1" class="cont">
				非進学校で成績不良のため卒業困難者そんな状況の中有名大学を目指す。<br>
				浪人期間を経ても願いは叶わず同志社大学へ。<br>
				そんなこんなで始まった大学生活では早稲田大学への交換留学を契機にサークルの広報として活躍。動画や写真撮影、新入生の広報の改善といった活動で活躍。</div>
			<div v-if="tab == 2" class="cont">
				次なるキャリアは都市計画の研究の道。<br>
				学生時代に大学院時代の経済的負担を考え、卒業後の入学を決め一旦大学を卒業。<br>
				2019年の３月まで大学院へ受験をするも失敗。キャリアを広告代理店業務に変更し４月から新卒就活を開始。
			</div>
			<div v-if="tab == 3" class="cont">
				学生時代の広報としての活動を軸に広告業界を志望。<br>
				就職活動進める中で徐々にWeb開発への関心が高まる。<br>そして2020年の２月に新卒就活を諦め力をつけるために就職活動を停止し、金銭的負担から来る時間の負担を減らすための2020年の６月まで停止。
			</div>
			<div v-if="tab == 4" class="cont">
				2020年の8月から就職活動再始動。<br>
				webエンジニアかwebデザイナーか迷うもwebエンジニアへのキャリアを選択。<br>
				Progate,Techcamp,udemyなどで学習を行い１０月より就職活動を開始。<br>
				就職活動開始後も力をつけるため様々な学習や開発を行なってきたが、その中でwebデザイナーの魅力にかたむがたちweb designerへのキャリアを含み方向修正し、現在にいたる。
			</div>
		</div>
	</div>
</template>

<script>
	export default {
  data(){
    return{
			tab:1,
			mainImg: require('@/assets/karitop.png'),
    }
  },
  methods: {
    change(num){
			if(num == 0)
			{
				this.tab = 1
			}
			else if(num == 1)
			{
				this.tab = 2
			}
			else if(num == 2)
			{
				this.tab = 3
			}
			else if(num == 3)
			{
				this.tab = 4
			}
		}
	}
}
</script>

<style scoped>
p{
	font-size: 50px;
	font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro';
	text-align: center;
	margin: 200px 0;
}
.p{
	position: absolute;
	font-size: 50px;
	width: 60%;
	left: 20%;
	top: 90%;
	font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro';
	text-align: center;
	margin: 0 auto;
}
img{
	top: 10%;
	left: 0;
	z-index: -1;
	width: 100%;
	height: auto;
}
.non{
	margin: 200px 0 0 0;
}
.ly{
	background: white;
	width: 70%;
	margin: 10% 15%;
	color: blue;
}
.bl{
	display: flex;
	justify-content: space-evenly;
}
.a{
	color: #080040;
	border-bottom:3px #080040 solid;
	width: 24%;
	text-align: center;
	padding: 5px 0 5px 0;
	font-size: 40px;
}
.b{
	color:rgb(163, 165, 255);
	border-bottom:3px rgb(163, 165, 255) solid;
	width: 24%;
	text-align: center;
	padding: 5px 0 5px 0;
	font-size: 40px;
}
.cont{
	padding: 20px 5px 20px 5px;
	font-size: 20px;
	color: grey;
}

</style>