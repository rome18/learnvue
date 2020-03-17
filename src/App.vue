<template>
  <div>
    <div id="app">
      <h1 v-once> {{ judul }} </h1>
      <p>{{respon}}</p>
      <input type="text" v-on:input="changeTitle">
      <p>{{ sayHello() }} - <a v-bind:href="link">Google</a></p>
    </div>
  </div>
</template>

<script>
export default {
  data:()=>({
    judul:'Hello World!',
    respon: 'Hiii!',
    link: 'http://google.com'
  }), 
  methods: {
    changeTitle: function(event) {
      this.judul = event.target.value;
    },
    sayHello: function(){
      this.judul = 'Hi Deski';
      return this.judul;
    }
  }
}
</script>

