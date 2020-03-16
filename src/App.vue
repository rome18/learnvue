<template>
<div id="app">
  <p>{{ fullname }}</p>
  <input v-model="fullname">
</div>
</template>

<script>
  var app = new Vue({
    el: '#app',
    data: {
      fullname: 'Your Full Name!'
    }
  })
</script>

