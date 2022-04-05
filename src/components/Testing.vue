<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        <img v-bind:src="imgsrc" width="100" height="100" />
        <div v-html="htmlcontent"></div>
    </div>
</template>
<script>
export default {
  name: 'Testing',
  data () {
    return {
      msg: 'Welcome to Your testing',
      imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/220px-Vue.js_Logo_2.svg.png',
      htmlcontent: '<h2>testing</h2>'
    }
  }
}
</script>
