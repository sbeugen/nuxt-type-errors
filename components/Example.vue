<template>
    <NumberDisplay :num="count" @some-event="logSomeEvent"/>
</template>
<script setup lang="ts">
const count = ref<number>(1);

function logSomeEvent(id: number) {
    console.log(id)
}
</script>
