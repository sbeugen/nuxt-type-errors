<template>
    <h1 @click="emit('someEvent', props.num)">{{ props.num }}</h1>
</template>
<script setup lang="ts">
interface Props {
    num: number;
}

const props = defineProps<Props>();

const emit = defineEmits<{ (e: "someEvent", id: number): void }>();
</script>
