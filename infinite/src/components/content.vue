<template>
  <div class="content">
    <navheader></navheader>
    <header>{{ content }}</header>
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
      content: '神展开内容'
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
</style>
