<template>
  <div id="myapp">
    {{count}}
    <br>
    {{$store.getters.doubleCount}}
    <button @click="$store.commit('add')">count++</button>
    <button @click="$store.dispatch('increment')">count--</button>
  </div>
</template>
<script>
export default {
  name: "mypage",
  data() {
    return {};
  },
  computed: {
    count() {
      return this.$store.state.count;
    }
  }
};
</script>

