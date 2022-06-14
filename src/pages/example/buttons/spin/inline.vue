<template>
  <div class="col-md-6 mt-3">
    <b-card header="Inline style">
      <div class="p-3">
        <p class="mb-0">inline spinbutton with  <code>inline</code>  attribute </p>
        <p>     
        this is a inline 
        <b-form-spinbutton  v-model="value"   class="mt-3 " inline  />
        demo
        </p>
      </div>  
    </b-card>
  </div>
</template>

<script>
import { BFormSpinbutton, BCard, BRow } from "bootstrap-vue";

export default {
  components: {
    BFormSpinbutton,
    BCard,
    BRow,
  },
  data: () => ({
    value: 1
  }),
};
</script>