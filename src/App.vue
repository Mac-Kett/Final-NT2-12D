<template>
  <div id="app" class="container-fluid mt-3">
    <div class="jumbotron">
      <Input />
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Input from "./componentes/Input.vue";

export default {
  name: "App",
  components: {
    Input,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>
#app {
}

h1 {
  color: orange;
}

.jumbotron {
  padding: 32px !important;
}

hr {
  color: #222;
}
</style>
