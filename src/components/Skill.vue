<template>
<div class="body">
	<div>
		<h1>Web skill</h1>
		<div class="ly">
			<div class="ttl">
				Web Design Skill
			</div>
			<div class="cont"> 
				<div class="cont-card">
					<h2>Photo Shop</h2>
					<h3>習得したこと</h3>
					<p>学生時代はサークルで必要なポスターなどを作成し、就職活動中は複数のレイヤーを活かしたバナー制作に活かしています。</p>
					<h3>工夫したこと</h3>
					<p>本で最低限の知識をインプットしてから後は徹底的に真似るを繰り返しました。</p>
				</div>
				<div class="cont-card">
					<h2>Ilustraiter</h2>
					<h3>習得したこと</h3>
					<p>学生時代はサークルで必要なポスターなどを作成し、就職活動中は複数のレイヤーを活かしたバナー制作に活かしています。</p>
					<h3>工夫したこと</h3>
					<p>本で最低限の知識をインプットしてから後は徹底的に真似るを繰り返しました。</p>
				</div>
				<div class="cont-card">
					<h2>Adobe Xd</h2>
					<h3>習得したこと</h3>
					<p>Web開発の作成に必要なプロトタイプ作成を行なってきました。複数のプラグインやコンポーネントなどを活用し効率よく作成を行なっています</p>
					<h3>工夫したこと</h3>
					<p>本で最低限の知識をインプットしてudemyでの学習を進めました。</p>
				</div>
		</div>
		</div>
		<p class="exa" @click="us()">作例へ</p>
		{{a}}
	</div>
	<div>
		<div class="ly">
		<div class="ttl">
			Web Programing Skill
		</div>
		<div class="cont"> 
			<div class="cont-card">
				<h2>HTML</h2>
				<h3>習得したこと</h3>
				<p>私はhtmlでは積み木の法則aタグやボタンタグなどを理解することができました</p>
				<h3>工夫したこと</h3>
				<p>HTMLを学ぶ際に工夫したことはコードの可読性を高めることです。属性名を後で別の人が読んでもわかるようにする記述することによって再現性の高いコードを記述することができました</p>
			</div>
			<div class="cont-card">
				<h2>css</h2>
				<h3>習得したこと</h3>
				<p>私はCSSで学んだことはhtmlの装飾方法です。特にその中でもブレイクポインを用いたモバイル対応や擬似要素を用いた発展的な手法も積極的に取り入れ学習しました</p>
				<h3>工夫したこと</h3>
				<p>Cssを学ぶ際に工夫したことは記述を一つ一つ理解したことで。開発を行う中で複雑なcssを検索して見つけ記述していく中でこの記述はこの意味があると一つ一つコピペで終わらせずに理解に試みました。</p>
			</div>
			<div class="cont-card">
				<h2>Java  script</h2>
				<h3>習得したこと</h3>
				<p>私がjavascriptで学んだことは変数の定義の仕方からdomという概念まで基本的なことから非同期通信など幅広く学びました。</p>
				<h3>工夫したこと</h3>
				<p>Javascriptを学ぶ際に工夫したことは検証ツールを必ず用いたことです。イベントを発火するたびに要素が取れているかなど確認しJavascriptにおけるライフサイクルを理解することに執着しました</p>
			</div>
			<div class="cont-card">
				<h2>jQuery</h2>
				<h3>習得したこと</h3>
				<p>私はjqueryではjavascriptの簡易的で使いやすい運用を学び実践することができました</p>
				<h3>工夫したこと</h3>
				<p>jQueryを学ぶ際に工夫したことはJSFiddleを多用したことです。実装する前に毎回JSFiddleで動きを確認しどの要素に対してどのイベントを起こすのが適切か確認しながら導入を進めました</p>
			</div>
			<div class="cont-card">
				<h2>Vue.js</h2>
				<h3>習得したこと</h3>
				<p>私がVue.jsではモダンなフロント構築を学びました。componentや仮装dom、spaなど現在のフロント構築に必要な技術を学び、活かした記述を行いました</p>
				<h3>工夫したこと</h3>
				<p>Vue.jsを学ぶ際に工夫したことは仮想DOMの理解です。今後reactも学ぶ予定ですので両者に共通する仮想DOMの理解を徹底することに工夫しました</p>
			</div>
			<div class="cont-card">
				<h2>Ruby</h2>
				<h3>習得したこと</h3>
				<p>私がrubyで学んだことはobject思考のプログラム設計です。元々オブジェクト指向で作られrた言語であるためオブジェクト指向で理解しやすく、他のプログラミング言語にも考え方として応用できる考え方を学びました</p>
				<h3>工夫したこと</h3>
				<p>Rubyを学ぶ際に私が工夫したことはエラーとの向き合い方です。サーバサイドの言語なのでエラーと向き合う場面が多く、一つづつ何が読み込めてないか徹底的にエラーと向き合いました</p>
			</div>
		</div>
		</div>
	</div>
	<div>
		<h1>Other skill</h1>
		<div class="ly">
			<div class="ttl">
				動画編集
			</div>
			<div class="cont"> 
				<div class="cont-card">
					<h2>Photo Shop</h2>
					<h3>習得したこと</h3>
					<p>Premire proでは動画の編集、音楽との組み合わせ、文字入れなどを行いました。</p>
					<h3>工夫したこと</h3>
					<p>このエフェクトは見る人にどのような意味があるのか、全体の中でどのような働きが起きるのかといった事を工夫しました。</p>
				</div>
				<div class="cont-card">
					<h2>Ilustraiter</h2>
					<h3>習得したこと</h3>
					<p>After Effectsでは3Dやアニメーションの作成を行いました</p>
					<h3>工夫したこと</h3>
					<p>ショートカットの徹底した活用を工夫しました。15秒進むだけでもマウスだけでなくコマンドを用いることで効率の良い作成に取り組みました
					</p>
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
			a:'a'
		}
	},
	methods:{
		us(){
			alert('準備中です')
		}
	}
}
</script>

<style scoped lang="scss">
$maincolor:#080040;
$basecolor:rgb(245, 244, 255);
$conttxtclr:grey;
$subcolor:#BBB6DE;
.body{
	z-index: 10;
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
}
.ly{
	background: $maincolor;
	width: 80%;
	margin: 50px 10%;
	border: 5px white solid;
}
.exa{
	text-align: center;
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
  display:flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

/* afterを追加するだけ！！ */


.cont-card{
	background: white;
	margin: 2% 2%;
	color: #080040;
	width: 25%;
}
.cont::after{
	content:"";
  display: block;
  width:25%;
}


</style>