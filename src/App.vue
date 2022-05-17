<template>
  <div id="wrapper">
    <div class="header">
      <h1>hello m8 {{ test }}</h1>
    </div>

    <div class="input">
      <div class="container">
        <div class="input">
          <input
            class="input-1"
            type="text"
            placeholder="Enter JSON to compare"
          />
        </div>
        <div class="input-compare-btn">
          <button>compare</button>
        </div>
        <div class="input">
          <input
            class="input-2"
            type="text"
            placeholder="Enter JSON to compare"
          />
        </div>
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

.container {
}

.input {
  display: inline-block;
}

.input-compare-btn {
  display: inline-block;
  padding: 0 20px;
}

.input-1,
.input-2 {
  width: 400px;
  height: 400px;
}
</style>
