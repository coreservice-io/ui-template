<script setup>

import SidebarLayout from "../../../layouts/sidebar/SidebarLayout.vue";
import { ref } from 'vue';

import Multiselect from '@vueform/multiselect'

let input_tags = ref(['tag1', 'tag2']);
</script>

<template>
  <SidebarLayout>
    <div class="space-y-8 divide-y divide-gray-200 divide-gray-200">
      <div>
        <h1 class="text-2xl leading-6">Examples of input tags</h1>
        <p class="mt-3"> </p>
      </div>

      <div class="pt-5 lg:grid lg:grid-cols-3 lg:gap-4">
        <div>
          <label for="username" class="flex">Simple input with tags</label>
          <p>tags:{{ input_tags }}</p>
        </div>
        <div class="mt-2">
          <Multiselect v-model="input_tags" :createOption="true" :options="input_tags" :searchable="true" mode="tags" noResultsText="" />
        </div>
      </div>


    </div>
  </SidebarLayout>
</template>
