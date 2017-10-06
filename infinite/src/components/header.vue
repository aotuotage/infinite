<template>
  <div class="content">
    <header>
     <div class="container-fluid">
       <div class="nvaOne">
       	<div class="navtitle col-xs-6 col-md-4">
        	<h3>神展开</h3>
        </div>
        <div class="">
           <button class="navbar-toggle collapsed" type="button" data-toggle="collapse" data-target=".navbar-collapse" v-on:click="onToggle">
	          <span class="sr-only">Toggle navigation</span>
	          <span class="icon-bar"></span>
	          <span class="icon-bar"></span>
	          <span class="icon-bar"></span>
          </button>
        </div>
       </div>
	    <nav v-show="Toggle" class="navList">
	      <ul>
	      	<li>首页</li>
	      	<li>我的</li>
	      	<li>第三</li>
	      	<li>第四</li>
	      </ul>
	    </nav>
     </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'content',
  data () {
    return {
      head: '神展开头部',
      Toggle: false
    }
  },
  methods: {
    onToggle: function () {
      this.Toggle = !this.Toggle
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container-fluid{
	padding: 0;
}
.nvaOne{
	background-color: rgba(0,0,0,0.1);
	height: 4rem;
}
.navtitle h3{
   color: rgba(63,63,63,0.5);
   margin: 0rem;
   line-height: 4rem;
   font-weight: 600;
}
.navbar-toggle{
	background:rgba(63,63,63,0.5);
}
.icon-bar{
	background-color: #fff;
}
.navList{
	background-color: rgba(63,63,63,0.5);
}
.navList ul{
	padding: 0;
}
.navList ul li{
    color: #fff;
    line-height: 2.5rem;
    list-style-type: none;
    font-weight: 600;
    padding-left: 1rem;
}
</style>
