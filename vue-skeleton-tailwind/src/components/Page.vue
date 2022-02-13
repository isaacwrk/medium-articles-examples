<template>
<div class="min-h-screen flex items-center justify-center bg-gradient-to-br from-green-300 to-green-400">
    <slot/>
</div>
</template>

<script lang='ts'>
import { defineComponent } from 'vue';

const Page = defineComponent({
});

export default Page;
</script>

<style>

</style>