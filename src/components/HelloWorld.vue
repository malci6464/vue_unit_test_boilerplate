<template>
  <div>
    <input v-model="name" />
    <button @click="formatMsg">Show message</button>
    <p>{{message}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      name: '',
      message: ''
    }
  },
  methods: {
    formatMsg () {
      this.message = `Hello ${this.name}`
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
