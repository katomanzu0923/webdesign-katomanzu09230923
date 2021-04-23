<template>
<div>
	<h1>Works</h1>
	<div class="ly">
		<div class="ttl">
			Webサイト集
		</div>
		<div class="cont">
			<div class="cont-card">
				<img class="mimg" src="@/assets/ramne.png"/>
				<p>WASEDA University-ramen</p>
				<button @click="up()">作品ページへ</button>
			</div>
			<div class="cont-card">
				<img class="img" src="@/assets/interview.png"/>
				<p>Interview-Practice</p>
				<button @click="up()">作品ページへ</button>
			</div>
			<div class="cont-card">
				<img class="img" src="@/assets/train.png"/>
				<p>Train-Ticket</p>
				<button @click="up()">作品ページへ</button>
			</div>
			<div class="cont-card">
				<img class="img" src="@/assets/kaki.png"/>
				<p>EC-Persimmon</p>
				<button @click="up()">作品ページへ</button>
			</div>
		</div>
	</div>
	<div class="ly">
		<div class="ttl">
			バナー集{{num}}
		</div>
		<div class="cont"> 
			<div class="cont-card">
				<img class="img" :src="leftImg">
			</div>
			<div class="cont-card">
				<img class="mainimg" :src="mainImg">
			</div>
			<div class="cont-card">
				<img class="img" :src="rightImg">
			</div>
		</div>
		<div class="button">
			<div type="button" @click="dlc()" :class="[num == 0? 'arrow_left_out': 'arrow_left']" v-if="yan"></div>
			<div :class="[num == 1? 'onCircle': 'circle']">1</div><div :class="[num == 2? 'onCircle': 'circle']">2</div><div :class="[num == 3? 'onCircle': 'circle']">3</div><div class="arrow" @click="clc()" v-if="is_right"></div>
		</div>
	</div>
</div>
</template>

<script>
export default {
	data(){
		return{
			a:'a',
			show:true,
			num:1,
			nums:0,
			ba_name:'first',
			mainImg: require('@/assets/sozai1.png'),
			leftImg: require('@/assets/sozai02.png'),
			rightImg: require('@/assets/sozai03.png'),
			yan:false,
			is_right:true,
			Data:{
				stb01: [
					require('@/assets/sozai1.png'),
					require('@/assets/sozai02.png'),
					require('@/assets/sozai03.png'),
				],
				stb02: [
					require('@/assets/sozai04.png'),
					require('@/assets/sozai05.png'),
					require('@/assets/sozai06.png'),
				],
				stb03: [
					require('@/assets/sozai07.png'),
					require('@/assets/sozai08.png'),
					require('@/assets/sozai09.png'),
				],
			}
		}
	},
	methods:{
		up(){
			this.a = 'b'
		},
		clc(){
			this.num +=1
			if(this.num ==2){
				this.mainImg = this.Data.stb01[0]
				this.leftImg = this.Data.stb01[1]
				this.rightImg = this.Data.stb01[2]
				this.ba_name = 'second'
				this.yan = true
			}
			else if(this.num == 3){
				this.mainImg = this.Data.stb03[0]
				this.leftImg = this.Data.stb03[1]
				this.rightImg = this.Data.stb03[2]
				this.ba_name = 'third'
				this.is_right = false
			}
		},
		dlc(){
			this.num -=1
			if(this.num == 1){
				this.mainImg = this.Data.stb02[0]
				this.leftImg = this.Data.stb02[1]
				this.rightImg = this.Data.stb02[2]
				this.ba_name = 'first'
				this.yan = false
			}
			else if(this.num == 2)
			{
				this.mainImg = this.Data.stb01[0]
				this.leftImg = this.Data.stb01[1]
				this.rightImg = this.Data.stb01[2]
				this.ba_name = 'second'
				this.yan = true
				this.is_right = true
			}
		}
	}
}
</script>

<style scoped lang="scss">
$maincolor:#080040;
$conttxtclr:grey;
$subcolor:#BBB6DE;
$basecolor:rgb(245, 244, 255);

h3{
	margin: 0 10px;
	padding: 0;
	font-size: 10px;
}

.arrow_left{
  position: relative;
  display: inline-block;
  padding-left: 10px;
}

.arrow_left_out{
  position: relative;
  display: inline-block;
  padding-left: 10px;
}

.arrow_left::before{
  content: '';
  width: 10px;
  height: 10px;
  border: 0px;
  border-top: solid 2px $basecolor;
  border-right: solid 2px $basecolor;
  -ms-transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  transform: rotate(225deg);
  position: absolute;
  top: 50%;
  left: 0;
  margin-top: -4px;
}

.arrow_left_out::before{
  content: '';
  width: 10px;
  height: 10px;
  border: 0px;
  border-top: solid 2px $basecolor;
  border-right: solid 2px $basecolor;
  -ms-transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  transform: rotate(225deg);
  position: absolute;
  top: 50%;
  left: 0;
  margin-top: -4px;
}

.arrow{
  position: relative;
  display: inline-block;
  padding-left: 20px;
}

.arrow::before{
  content: '';
  width: 10px;
  height: 10px;
  border: 0px;
  border-top: solid 2px $basecolor;
  border-right: solid 2px $basecolor;
  -ms-transform: rotate(45deg);
  -webkit-transform: rotate(45deg);
  transform: rotate(45deg);
  position: absolute;
  top: 50%;
  left: 0;
  margin-top: -4px;
}
h1{
	font-size: 50px;
	font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro';
	text-align: center;
}
h2{
	text-align: center;
	border-bottom: 0.5px solid #080040;
	font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro';
	margin: 0 0 ;
	padding: 5px 0 5px 0;
}
h3{
	text-align: center;
	font-size: 16px;
}
p{
	color: $conttxtclr;
	margin: 0;
	text-align: center;
}
.p{
	color: $conttxtclr;
	margin: 0 50px;
	text-align: center;
}
.button{
	width: 60%;
	margin: 30px 20%;
	display: flex;
	justify-content: center;
}
button{
	width: 70%;
	display: inline-block;
	margin: 10px 15%;
}
.img{
	width: 100%;
	height: 80%;
}

.mimg{
	width: 50%;
	margin: 0 25%;
	height: 80%;
}
.mainimg{
	width: 100%;
	height: 80%;
}
.ly{
	background: $maincolor;
	width: 80%;
	margin: 100px 10%;
	border: 5px white solid;
}
.ttl{
	background: white;
	color: $basecolor;
	width: 30%;
	margin: -2% 35% 0 35%;
	text-align: center;
	font-size: 35px;
	-webkit-text-stroke-width: 0.5px;
	-webkit-text-stroke-color:$maincolor;
}
.cont-card{
	position: relative;
	margin: 5% 5%;
	width:20%;
	background: $maincolor;
}
.cont{
	display:flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.onCircle {
  width: 20px;
	margin: 0 1%;
	background-color:$basecolor;
  border-radius: 50%; 
  text-align: center;
  line-height: 20px;
	padding: 3px;
	color: $maincolor;
}
.circle {
  width: 20px;
	margin: 0 1%;
  background-color:$basecolor;
	color: $subcolor;
  border-radius: 50%; 
  text-align: center;
  line-height: 20px;
	padding: 3px;
}

</style>