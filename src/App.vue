<template>
<div id="app">
  <p>{{ fullname }}</p>
  <input v-model="fullname">
</div>
</template>

<script>
  export default{
    data: function(){
      return{
        fullname: 'Your Full Name!'
      }
     
    }
  }
</script>

