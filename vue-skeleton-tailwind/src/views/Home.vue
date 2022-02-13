<template>
    <Page>

    </Page>
</template>

<script lang='ts'>
import { defineComponent } from 'vue';


import Page from '@/components/Page.vue';
import Card from '@/components/Card.vue';
import Skeleton from "@/components/Skeleton.vue";

const Home = defineComponent({
    components:{
        Page,
        Card,
        Skeleton
    }
});

export default Home;
</script>

<style>

</style>
