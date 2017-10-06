<template>
  <div class="content">
    <navheader></navheader>
    <div class="contentList">
      <div class="child col-xs-6 col-md-3">
        <div class="childElement">
          <h4 class="childTitle">
            {{title}}
          </h4>
          <p>作者：{{anthen}}</p>
        </div>
      </div>
      <div class="child col-xs-6 col-md-3">
        <div class="childElement">
          <h4 class="childTitle">
            {{title}}
          </h4>
          <p>发起者：{{anthen}}</p>
        </div>
      </div>
    </div>
    <navfooter></navfooter>
  </div>
</template>

<script>
import navheader from './header'
import navfooter from './footer'

export default {
  name: 'content',
  data () {
    return {
      content: '神展开内容',
      title: '从你的全世界路过',
      anthen: '张奥博'
    }
  },
  components: {navheader, navfooter}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.contentList:after{
  content: ".";
  visibility: hidden;
  display: block;
  height: 0;
  clear: both;
}
.childElement{
  position: relative;
  margin: 1rem;
  padding: 1rem;
  background-color:#B0C4DE;
  text-align: center;
  height: 13rem;
  color: #fff;
}
.childElement p{
  position: absolute;
  bottom: 1rem;
  text-align: center;
}
</style>
