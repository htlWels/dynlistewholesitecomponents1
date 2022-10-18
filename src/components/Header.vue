<template>
  <header>
    <h1>HTL Wels / {{ msg }}</h1>
    <h2>JavaScript / DOM-Manipulation / Dynamic List</h2>
    <hr />
  </header>
</template>

<script>
import { ref } from 'vue';

export default {
  props: {
    msg: { type: String, required: true },
  },
  setup() {
    const count = ref(0);

    // expose to template and other options API hooks
    return {
      count,
    };
  },

  mounted() {
    //console.log(this.count); // 0
  },
};
/*
const props = defineProps({
  msg: { type: String, required: false },
});
*/
</script>

<style></style>
