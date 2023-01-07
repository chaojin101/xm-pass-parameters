<script setup lang="ts">
import { ref } from "vue";

// const props = defineProps({
// 	title: {
// 		type: String,
// 		default: "adf",
// 	},
// 	age_: {
// 		type: Number,
// 		default: 1,
// 	},
// });
// console.log(props.title);

// ts

// const props = withDefaults(
// 	defineProps<{
// 		title: string;
// 		arr?: number[];
// 	}>(),
// 	{
// 		arr: () => [666],
// 	}
// );

// console.log(props.title);
// console.log(props.arr);

// const emit = defineEmits(["send"]);

defineExpose({
	name: "xm-name-expose",
});
</script>

<template>
	<div>子集</div>
	<!-- <div>name = {{ title }}</div>
	<div>arr = {{ arr }}</div> -->

	<!-- <button @click="emit('send', 'xm-emit')">给父组件传值</button> -->
</template>

<style scoped></style>
