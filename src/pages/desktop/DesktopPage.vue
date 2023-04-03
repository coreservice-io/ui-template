<script setup>
import DesktopLayout from "../../layouts/desktop/DesktopLayout.vue";
</script>
<template>
    <DesktopLayout>
        <form class="space-y-8 divide-y divide-gray-200 divide-gray-200">
            <div>
                <h1 class="text-2xl leading-6">Desktop appx</h1>
                <p class="mt-3">This is a page where you can implement your desktop</p>
            </div>
            <div class="pt-5 lg:grid lg:grid-cols-3 lg:gap-4">
                <div>
                    <label for="username" class="flex">Input example</label>
                    <p>detail:</p>
                </div>
                <div class="lg:col-span-2 mt-2">
                    <div class="input-wrap">
                        <div class="prefix">http://</div>
                        <input type="text" name="company-website" id="company-website" class="rounded pl-14"
                            placeholder="www.example.com" />
                    </div>
                </div>
            </div>
        </form>
    </DesktopLayout>
</template>