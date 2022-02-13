<template>
    <Page>
        <Suspense>
            <template #default>
                <Card/>
            </template>
            <template #fallback>
                <Skeleton/>
            </template>
        </Suspense>
    </Page>
</template>

<script lang='ts'>
import { defineComponent,reactive } from 'vue';


import Page from '@/components/Page.vue';
import Card from '@/components/Card.vue';
import Skeleton from "@/components/Skeleton.vue";

const Home = defineComponent({
    components:{
        Page,
        Card,
        Skeleton
    },

    setup(){
        const state = reactive({
            loading: true
        });

        const isLoading = () =>{
            setTimeout(()=>{
                state.loading;
            },200);
            return state.loading = false;
        };

        return{ isLoading };
    }
});

export default Home;
</script>

<style>

</style>
