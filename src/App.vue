<template>
  <div id="exercise">
    <p> VueJS is pretty cool - {{ name }} {{ age }}</p>
    <p>My Age times 3 is {{ age * 3 }}</p>
    <p>A Random Number between 0 to 1 {{ random() }}</p>
    <div>
      <img v-bind:src="image" style="width:100px;height:100px">
    </div>
    <div>
      <input type="text" v-bind:value="name">
    </div>
  </div>
</template>

<script>
export default {
  data:()=>({
    name: 'Romanos Albert Adhitya',
    age: 23,
    image: 'https://www.google.com/url?sa=i&url=https%3A%2F%2Funsplash.com%2Fimages%2Fanimals%2Fcow&psig=AOvVaw2h5--JgQiV-Za-JgXX5_W9&ust=1584505495591000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCIjTzYzVoOgCFQAAAAAdAAAAABAD'
  }),
  methods: {
    random:function() {
      return Math.random();
    }
  }
}
</script>

