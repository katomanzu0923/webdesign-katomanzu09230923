<template>
<div>
	<h1>Future</h1>
	<div class="ly">
		<div class="ttl">
			将来像
		</div>
		<div class="cont">
			<p>UIデザイナーとして活躍したいと考えています。もちろんデザイナーとして使いやすい、離脱率を防ぐデザインを作成するのはもちろんですが、言語のかべによって生じる障壁をなくすデザインを設計したいと考えています。</p>
		</div>
	</div>
	<div @click="open()" class="que">なぜか?</div>
	<transition name="first">
		<div class="ly" v-if="a == 'b'">
		<div class="cont">
			<p>UIデザイナーとして活躍したいと考えています。もちろんデザイナーとして使いやすい、離脱率を防ぐデザインを作成するのはもちろんですが、言語のかべによって生じる障壁をなくすデザインを設計したいと考えています。</p>
		</div>
		</div>
	</transition>
</div>
</template>

<script>
export default {
	data(){
		return{
			a:'a'
		}
	},
	methods:{
		open(){
			this.a = 'b'
		}
	}
}
</script>

<style scoped lang="scss">
$maincolor:#080040;
$basecolor:rgb(245, 244, 255);
$conttxtclr:grey;
.first-enter-active{
  transition: all 3s ease;
}
.first-enter {
	opacity: 0;
}
.first-enter-to{
	opacity: 1;
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
	padding: 0 20px;
	width: 50%;
}
.ly{
	background: $maincolor;
	width: 50%;
	margin: 5px 25%;
	border: 3px white solid;
}
.que{
	text-align: center;
	margin: 50px 0;
}
.ttl{
	background: white;
	color:$basecolor;
	width: 50%;
	margin: -2% 35% 0 25%;
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

</style>