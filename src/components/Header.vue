<template>
	<div id="body">
		<p class="a">Portfolio for the Web designer</p>
		<div class="fix">
			<p @click="change(0)" :class="[btnCheck==0? 'el_btn01_is':'el_btn01_def']" v-on:mouseover="u(0)" v-on:mouseleave="out(0)">My Profile</p>
		<p @click="change(1)" :class="[btnCheck==1? 'el_btn02_is':'el_btn02_def']">Skill</p>
		<p @click="change(2)" :class="[btnCheck==2? 'el_btn03_is':'el_btn03_def']">Works</p>
		<p @click="change(3)" :class="[btnCheck==3?'el_btn04_is':'el_btn04_def']">Future</p>
		<p @click="change(4)" :class="[btnCheck==4? 'el_btn05_is':'el_btn05_def']">Contact</p>
		</div>
	</div>
</template>

<script>

export default {
	data(){
		return{
			btnCheck:0,
			leftImg:require('@/assets/ii.png'),
		}
	},
	methods: {
		change(num){
			if(num == 0)
			{
				this.btnCheck = 0
				this.$emit('change01')
			}
			else if(num ==1)
			{
				this.btnCheck = 1
				this.$emit('change02')
			}
			else if(num == 2)
			{
				this.btnCheck =2
				this.$emit('change03')
			}
			else if(num == 3)
			{
				this.btnCheck =3
				this.$emit('change04')
			}
			else if(num == 4)
			{
				this.btnCheck =4
				this.$emit('change05')
			}
		},
	}
}
</script>

<style scoped>


p{
	margin: 5px 20px;
	font-size: 20px;
	display: inline-block;
}

.a{
	left: 0;
	font-size: 30px;
	width: 30%;
	padding: 20px 0;
	font-family: 'ヒラギノ明朝 Pro W3', 'Hiragino Mincho Pro';
	border-bottom : 2px white solid;
}
#body{
	display:flex;
	justify-content:flex-start;
	list-style: none;
	flex-direction: column;
	position: absolute;
	background: transparent;
	left: 0;
	top: 0;
	width: 100%;
}
.el_btn01_is{
	color: white;
	display: inline-block;
	width: 6%;
}

.el_btn02_is{
	color: white;
	display: inline-block;
	width: 2.5%;
}

.el_btn03_is{
	color: white;
	display: inline-block;
	width: 4%;
}

.el_btn04_is{
	color: white;
	display: inline-block;
	width: 4%;
}

.el_btn05_is{
	color: white;
	display: inline-block;
	width: 5%;
}

.el_btn01_def{
	color: grey;
	display: inline-block;
	width: 6%;
}

.el_btn02_def{
	color: grey;
	display: inline-block;
	width: 2.5%;
}

.el_btn03_def{
	color: grey;
	display: inline-block;
	width: 4%;
}

.el_btn04_def{
	color: grey;
	display: inline-block;
	width: 4%;
}

.el_btn05_def{
	color: grey;
	display: inline-block;
	width: 5%;
}

.el_btn_def{
	color:grey;
}

.fix{
	display:flex;
	justify-content:flex-start;
	list-style: none;
	flex-direction: column;
	background: transparent;
	width: 100%;
}
</style>