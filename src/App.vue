<template>
  <div
    class="w-full h-screen flex overflow-hidden justify-center items-center border text-green-500 text-3xl"
  >
    <LayoutPageVue></LayoutPageVue>
  </div>
</template>
<script>
import LayoutPageVue from "./components/LayoutPage.vue";
export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    LayoutPageVue,
  },
  methods: {},
  computed: {},
  mounted() {},
  watch: {},
};
</script>
<style scoped></style>
