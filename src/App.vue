<template>
<div class="body">
  <Header v-on:change01="Change01()" v-on:change02="Change02()" v-on:change03="Change03()" v-on:change04="Change04()" v-on:change05="Change05()" class="fix"></Header>
  <About v-if="tab== 1" class="body01"></About>
  <Skill v-if="tab== 2" class="body02"></Skill>
  <Works v-if="tab == 3">{{tab}}</Works>
  <Future v-if="tab == 4">aa</Future>
  <Contact v-if="tab == 5"></Contact>
  {{tab}}
</div>
</template>

<script>
import 'normalize.css'
import Header from './components/Header.vue'
import About from './components/About.vue'
import Skill from './components/Skill.vue'
import Works from './components/Works.vue'
import Future from './components/Future.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  data(){
    return{
      tab:1
    }
  },
  components: {
    Header,
    About,
    Skill,
    Works,
    Future,
    Contact
  },
  methods: {
    Change01(){
      this.tab = 1
    },
    Change02(){
      this.tab = 2
    },
    Change03(){
      this.tab = 3
    },
    Change04(){
      this.tab = 4
    },
    Change05(){
      this.tab = 5
    }
  }
}
</script>

<style>
body{
  color: white;
}
.fix{
  position: absolute;
  position: fixed;
  z-index: 1;
  top: 10%;
}
.body01{
  z-index: 1;
}

.body02{
  z-index: 2;
}
</style>
