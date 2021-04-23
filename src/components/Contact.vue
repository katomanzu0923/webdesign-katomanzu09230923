<template>
<div>
	<div>
		<h1>Contact</h1>
	<div class="ly">
		<div class="ttl">
			Mail
		</div>
		<div>
			<div>
				<p>Your Name</p>
				<input v-model="name" placeholder="your name">
			</div>
			<div>
				<p>Your Addres</p>
				<input v-model="name" placeholder="farm@.co.jp">
			</div>
			<div>
				<p>contents</p>
				<textarea v-model="name" placeholder="ご用件をご記入ください"></textarea>
			</div>
			<div>
				<button @click="submit">submit</button>
			</div>
		</div>
	</div>
	</div>
	<div>
	<div class="ly">
		<div class="ttl">
			SNS
		</div>
		<div>
			<div class="icon">
				<img class="img" :src="leftImg" @click="up()">
				<img class="img" :src="centerImg" @click="up()">
				<img class="img" :src="rightImg" @click="up()">
			</div>
			<div>
			</div>
			<div>
			</div>
		</div>
	</div>
	</div>
</div>
</template>

<script>
export default {
	data(){
		return{
			a:'a',
			name:'',
			leftImg:require('@/assets/twi.png'),
			centerImg:require('@/assets/ins.png'),
			rightImg:require('@/assets/face.png'),
		}
	},
	methods:{
		up(){
			alert('ok')
		}
	}
}
</script>

<style scoped lang="scss">
$maincolor:#080040;
$basecolor:rgb(245, 244, 255);
$conttxtclr:grey;
$subcolor:#BBB6DE;
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
	color: white;
	text-align: center;
}
div{
	text-align: center;
}
button{
	margin: 20px 0;
}
.ly{
	background: $maincolor;
	width: 80%;
	margin: 10% 10%;
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
.cont{
	display: flex;
	justify-content: space-evenly;
}
.cont-card{
	background: white;
	margin: 5% 0;
	color: #080040;
}
.icon{
	display: flex;
	justify-content: center;
}
.img{
	margin: 5%;
	width: 6%;
}
</style>