<template>
  <div class="row">
      <basic/>
      <max/>
      <inline/> 
  </div>
</template>

<script>
 
import Basic from "./basic.vue";
import Max from "./max.vue";
import Inline from "./inline.vue";
 

export default {
  components: {
      Basic,
      Max,
      Inline
  },
};
</script>