<template>
  <div id="wrapper">
    <div class="header">
      <h1>hello m8 {{ test }}</h1>
    </div>

    <div class="container">
      <div class="input">
        <textarea placeholder="Enter JSON to compare!"></textarea>
      </div>
      <div class="input-compare-btn">
        <button @click="test11">compare</button>
      </div>
      <div class="input">
        <textarea placeholder="Enter JSON to compare!"></textarea>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      test: "haha",
    };
  },
  methods: {
    test11() {
      console.log("test");
    },
  },
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

textarea {
  display: block;
  overflow-x: hidden;
  overflow-y: auto;
  padding: 5px 5px;
  width: 400px;
  height: 400px;
  resize: none;
}

.container {
  width: 100%;
}

.input {
  display: inline-block;
  vertical-align: middle;
}

.input-compare-btn {
  display: inline-block;
  padding: 0 20px;
  vertical-align: middle;
}

.input-1,
.input-2 {
  width: 400px;
  height: 400px;
}
</style>
