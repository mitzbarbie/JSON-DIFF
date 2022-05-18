<template>
  <div id="wrapper">
    <div class="header">
      <h1>hello m8 {{ test }}</h1>
    </div>

    <div class="container">
      <div class="input">
        <textarea
          v-model="input1"
          type="string"
          placeholder="Enter JSON to compare!"
        ></textarea>
      </div>
      <div class="input-compare-btn">
        <button type="button" @click="getData">compare</button>
      </div>
      <div class="input">
        <textarea
          v-model="input2"
          type="string"
          placeholder="Enter JSON to compare!"
        ></textarea>
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
      input1: "",
      input2: "",
    };
  },
  // watch: {
  //   input1() {
  //     console.log(this.input1);
  //   },
  // },
  methods: {
    getData() {
      console.log(this.input1, this.input2);
      if (this.input1 !== this.input2) {
        alert("this is not same!");
      }
    },
    sameData() {
      // this.input1 = this.input2;
    },
  },
  components: {},
  // beforeCreate() {
  //   console.log("beforeCreate");
  // },
  // created() {
  //   console.log("created");
  // },
  // beforeMount() {
  //   console.log("beforeMount");
  // },
  // mounted() {
  //   console.log("mounted");
  // },
  // beforeUpdate() {
  //   console.log("beforeUpdate");
  // },
  // updated() {
  //   console.log("updated");
  // },
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
