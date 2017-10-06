<template>
    <footer>
      <div class="footer">
        {{ foot }}
      </div>
    </footer>
</template>

<script>
export default {
  name: 'content',
  data () {
    return {
      foot: '神展开备案号：没有'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer{
  height: 3rem;
  line-height: 3rem;
  text-align: center;
  background-color: rgba(0,0,0,0.1);
}
</style>
