<script setup>
import Multiselect from '@vueform/multiselect'
import SidebarLayout from "../../../layouts/sidebar/SidebarLayout.vue";
import { ref } from "vue";

const single_sel_options = [
    'Batman',
    'Robin',
    'Jack',
    'Joker',
]
let single_sel_value = ref(null);


const multi_sel_options = [
    'Batman',
    'Robin',
    'Jack',
    'Joker',
]
let multi_sel_value = ref(['Jack']);


const multi_sel_tag_options = [
    'Batman',
    'Robin',
    'Jack',
    'Joker',
]
let multi_sel_tag_value = ref(['Jack']);


</script>

<template>
    <SidebarLayout>
        <div class="space-y-8 divide-y divide-gray-200 divide-gray-200">
            <div>
                <h1 class="text-2xl leading-6">Single/Multi Select</h1>
                <p class="mt-3"></p>
            </div>

            <div class="pt-5 lg:grid lg:grid-cols-3 lg:gap-4">
                <div>
                    <label for="username" class="flex">Single select (normal size) </label>
                    <p>{{ value ? value : "not selected" }}</p>
                </div>

                <div class="lg:col-span-2 mt-1">
                    <Multiselect v-model="single_sel_value" :options="single_sel_options" mode="single" />
                </div>

            </div>
        </div>

        <div class="space-y-8 divide-y divide-gray-200 divide-gray-200">

            <div class="pt-5 lg:grid lg:grid-cols-3 lg:gap-4">
                <div>
                    <label for="username" class="flex">Single select (small size) </label>
                    <p>{{ multi_sel_value }}</p>
                </div>

                <div class="lg:col-span-2 mt-1 input-wrap sm">
                    <Multiselect v-model="multi_sel_value" :options="multi_sel_options" mode="multiple" />
                </div>

            </div>
        </div>


        <div class="space-y-8 divide-y divide-gray-200 divide-gray-200">

            <div class="pt-5 lg:grid lg:grid-cols-3 lg:gap-4">
                <div>
                    <label for="username" class="flex">Single select (large size) </label>
                    <p>{{ multi_sel_tag_value }}</p>
                </div>

                <div class="lg:col-span-2 mt-1 input-wrap sm">
                    <Multiselect v-model="multi_sel_tag_value"  :options="multi_sel_tag_options" mode="tags" />
                </div>

            </div>
        </div>


    </SidebarLayout>
</template>

