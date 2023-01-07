<script setup lang="ts">
import { ref } from "vue";
import waterFallVue from "./components/waterFall.vue";

const name = ref("xm");

const log = (...args: any[]) => console.log(args);

const waterFall = ref<InstanceType<typeof waterFallVue>>();
</script>

<template>
	<div>父集</div>
	<hr />
	<waterFallVue ref="waterFall" @send="log" :title="name"></waterFallVue>
	waterFall?.name = {{ waterFall?.name }}
</template>

<style scoped>
div {
	margin: 10px;
}
</style>
