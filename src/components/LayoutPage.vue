<template>
  <div class="w-[100vw] h-[100vh] border text-white text-3xl bg-gray-950">
    <div class="w-12/12 h-[10vh] bg-red-400">Sheharyar</div>
    <div class="w-12/12 h-[92vh] flex justify forder bg-gray-400">
      <div class="bg-gray-400 w-[5%] h-full flex shrink-0"></div>
      <div
        :class="
          toggleIn == true
            ? 'w-12/12 duration-500 flex-1'
            : ' duration-500 w-[75%]'
        "
        class="bg-gray-700 w-[75%] flex justify-end"
      >
        Sheharyar
      </div>
      <div
        class="bg-gray-400 flex w-[20%] shrink-0 h-[92vh] self-end"
        :class="
          toggleIn == true
            ? 'w-[0%] duration-500'
            : 'translate-x-0 duration-500'
        "
      >
        <div class="flex h-[92vh] items-center">
          <svg
            @click="toggler(toggleIn)"
            :class="toggleIn == true ? 'rotate-180 ml-[-24px]' : 'ml-[-15px]'"
            width="26"
            class="cursor-pointer"
            height="26"
            viewBox="0 0 26 26"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M16.2497 2.16732L9.74967 2.16732C4.33301 2.16732 2.16634 4.33399 2.16634 9.75065L2.16634 16.2507C2.16634 21.6673 4.33301 23.834 9.74968 23.834L16.2497 23.834C21.6663 23.834 23.833 21.6673 23.833 16.2507L23.833 9.75065C23.833 4.33399 21.6663 2.16732 16.2497 2.16732Z"
              fill="#323232"
            />
            <path
              d="M11.6349 9.1759L15.4482 13.0001L11.6349 16.8242"
              stroke="white"
              stroke-width="1.5"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </div>
        <div>
          <h1>Sheharyar</h1>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "LayoutPage",
  data() {
    return {
      toggleIn: false,
    };
  },
  components: {},
  methods: {
    toggler() {
      if ((this.toggleIn = !this.toggleIn)) {
        this.toggleIn = true;
        console.log("toggleIn is", this.toggleIn);
      } else {
        this.toggleIn = false;
        console.log("toggleIn is ", this.toggleIn);
      }
    },
  },
  computed: {},
  mounted() {},
  watch: {},
};
</script>
<style scoped></style>
